# To do list
**一個使用 Node.js + Express 打造的To do list。資料庫採用MySQL**

## 產品功能如下：
 * 使用者可以註冊帳號，登入之後才能使用功能
 * 使用者可以新增一條待辦事項
 * 使用者可以瀏覽一條待辦事項
 * 使用者可以瀏覽全部待辦事項
 * 使用者可以修改待辦事項
 * 使用者可以刪除待辦事項


## 環境建置：
 1. MySQL2
 2. Node.js
 
## 使用者預設資料：
  * email: root@example.com
  * password: 12345678

## 下載方法：
 1. 打開終端機，Clone 此專案至本機電腦
 
```
git clone https://github.com/haru5386/todo-sequelize
```

2. 進入存放此專案的資料夾

```
cd todo-sequelize
```

3. 安裝 npm 套件，

```
npm install
```

4.  MySQL workbench，並建立資料庫

```
drop database if exists todo_sequelize;
create database todo_sequelize;
use todo_sequelize;
```

5. 建立資料庫欄位及種子資料

```
npx sequelize db:migrate
npx sequelize db:seed:all
```
6. 啟動網頁伺服器

```
npm run dev
```

7. 顯示`App is running on http://localhost:3000`
   表示成功進入
