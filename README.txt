廢土戰隊 · Vault 13（PWA 版）

【安裝步驟】
1. 把整個資料夾內容上傳到任一 HTTPS 靜態空間（GitHub Pages、Netlify、Cloudflare Pages 皆可）。
2. 用手機或電腦瀏覽器開啟網址：
   - Android / Chrome / Edge：遊戲「☰ → 系統」頁會出現「📲 安裝到這台裝置」按鈕（或瀏覽器選單 → 安裝應用程式）。
   - iPhone / iPad：Safari 下方「分享」→「加入主畫面」。
3. 安裝後可離線遊玩（所有圖片與函式庫都已打包在資料夾內）。

【本機測試】在此資料夾執行：  python3 -m http.server 8000   然後開啟 http://localhost:8000
（直接雙擊 index.html 用 file:// 開啟時，瀏覽器會禁止精靈圖與 PWA，請務必用網址開啟。）

【更新遊戲】更換檔案後，請把 sw.js 內的 VER 改成新版號，已安裝的使用者才會拿到新版。

【檔案】
index.html            遊戲本體
manifest.webmanifest  安裝資訊（名稱、圖示、顏色）
sw.js                 離線快取
assets/atlas.png      精靈圖集（角色、怪物、物品、建築；CSS 取圖）
vendor/               three.js r128、rot.js 2.2.0（離線用）
icons/                App 圖示（192／512／maskable／iOS）
