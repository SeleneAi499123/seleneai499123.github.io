# 常用 CLI 指令

Angular CLI（Command Line Interface）是由 Angular 團隊提供的強大工具，用於簡化 Angular 應用程式的開發流程。它提供了各種命令，可快速搭建、構建、測試和部署 Angular 應用程式。

___

## 建立多專案工作區

同時開發多個 Angular 專案，共用 node_Module 資料夾，在其空間下新增的專案會放在 `project` 資料夾底下。

```bash
ng new my-workspace --create-application false
```

___

## 創建一個 Angular 專案

使用以下指令創建一個新的 Angular 專案：

```bash
ng new my-angular-app -s -S
```

|  參數    | 說明 |
| --------- | ----------- |
| --help    | 列出參數說明  |
| --routing    | 產生routing module  |
| --style    | 指定樣式表類型，如CSS  |
| -S    | 不會建立spec.ts測試檔  |
| -s | 可使用inline style  |

___

## 運行應用程式

輸入以下指令會默認在 `http://localhost:4200/` 上運行應用程式。

```bash
ng serve -o
```

|  參數    | 說明 |
| --------- | ----------- |
| --help    | 列出參數說明  |
| -o    | 在預設瀏覽器開啟  |
| --port    | 指定port位置  |
| --ssl | 使用https  |

___

## ng generate

Angular CLI 可以透過在命令列輸入以下指令來生成各種 `.ts` 檔案：

```bash
ng generate <schematic> <name> [options]
# 或者使用簡寫形式
ng g <schematic> <name> [options]
```

可用的 schematics 包括：

- component (c): 生成元件
- directive (d): 生成指令
- pipe (p): 生成管道
- service: 生成服務
- class (cl): 生成類別
- guard: 生成守門員
- interface (i): 生成介面
- enum: 生成枚舉
- module: 生成模組
- application (app): 生成專案



## 參考資料
> [Angular CLI 官方文檔](https://angular.io/cli)