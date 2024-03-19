# 參數的傳遞

##  定義參數名稱

我們可以從路由的`path`定義參數名稱，在參數名稱前加上冒號`:`，如`:id`, `:state`...等等。

```typescript
{
    path:'product', component:'ProductComponent', children:[
        { path:':id', component:'ProductDetailComponent'}
    ]
}
```

```html
<a routerLink="./product/1" (click)="goProduct(1)">產品1</a>
```

在 `product.component.ts`內使用`navigate()`或`navigateByUrl()`傳遞參數：

```typescript
constructor(private router:Router){}

goProduct(id:number){
    // 以路徑段陣列表示
    this.router.navigate(['/','product',id]);
    // 以字串表示
    this.router.navigateByUrl(`/product/${id}`);
}
```

---

##  接收參數值

在子路由 `product-detail.component.ts`內的`ngDoCheck()`獲取參數值。

```typescript
constructor(private route:ActivatedRoute){}

ngDoCheck(){
    let value=this.route.snapshot.paramMap.get('id');
    this.id=Number(value);
}

```