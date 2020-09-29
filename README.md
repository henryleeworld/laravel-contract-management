# Laravel 8 契約管理

在法律上要訂定契約，是以意思表示為之，意思表示可以用明示或默示的方式表達出來，除了少數法律設有強制或禁止規定的情況外，基本上交易雙方當事人都可以基於契約自由原則，自由形成契約內容，以規範雙方當事人間的法律關係。Laravel 8 契約管理主要是用 [QuickAdminPanel](https://quickadminpanel.com) 生成的，除了一些定制代碼，可依需求彈性改造的工具。

## 使用方式
- 把整個專案複製一份到你的電腦裡，這裡指的「內容」不是只有檔案，而是指所有整個專案的歷史紀錄、分支、標籤等內容都會複製一份下來。
```sh
$ git clone
```
- 將 __.env.example__ 檔案重新命名成 __.env__，如果應用程式金鑰沒有被設定的話，你的使用者 sessions 和其他加密的資料都是不安全的！
- 當你的專案中已經有 composer.lock，可以直接執行指令以讓 Composer 安裝 composer.lock 中指定的套件及版本。
```sh
$ composer install
```
- 產生 Laravel 要使用的一組 32 字元長度的隨機字串 APP_KEY 並存在 .env 內。
```sh
$ php artisan key:generate
```
- 執行 __Artisan__ 指令的 __migrate__ 來執行所有未完成的遷移，並執行資料庫填充（如果要測試的話）。
```sh
$ php artisan migrate --seed
```
- 執行安裝 Laravel Mix 引用的依賴項目，並執行所有 Mix 任務。
```sh
$ npm install && npm run dev
```
- 在瀏覽器中輸入已定義的路由 URL 來訪問，例如：http://127.0.0.1:8000。
- 你可以經由 `/login` 來進行登入，預設的電子郵件和密碼分別為 __admin@admin.com__ 和 __password__ 。
- 登入後可以經由 `/admin/contracts` 來進行契約管理。

----

## 畫面截圖
![](https://i.imgur.com/fs2Ooi5.png)
> 好的契約帶來好的合作開始，按照過往經驗，通常契約制定越詳細、越謹慎，代表雙方更重視合作的實質內容與未來發展遠景，同時也加強雙方合作的信任基礎，有一份好的契約，除了保障締約方之外，也可以有效避免將來訴訟的發生
