#  安裝相關工具

想要開始使用 Angular，需要先安裝會使用到的套件及工具：如Node.js、TypeScript、Angular CLI 與 Visual Studio Code。  

___

## 1. 安裝 Node.js

從 [Node.js 官方網站](https://nodejs.org/) 下載適合作業系統的版本。安裝完成後，可以在終端中運行以下命令來檢查 Node.js的安裝版本：

```bash
node -v
```

___

## 2. 安裝 TypeScript

使用 npm 管理器來安裝 TypeScript，在終端中執行以下命令：

```bash
npm install -g typescript
```

___

## 3. 安裝 Angular CLI

安裝最新版本：
```bash
npm install -g @angular/cli
```

安裝指定版本（15版）
```bash
npm install -g @angular/cli@15
```
|  參數    | 說明 |
| --------- | ----------- |
| -g    | 安裝在全域       |
| --save-dev | 只安裝在目前專案  |

___

## 4. 安裝 Visual Studio Code

從 [Visual Studio Code 官方網站](https://code.visualstudio.com/) 下載適用於作業系統的安裝程式。  
若在 VS Code 環境中遇到無法執行 PowerShell 腳本的問題時，輸入以下指令設定執行原則：

```bash
Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope CurrentUser
```