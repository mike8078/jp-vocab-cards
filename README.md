# 日文單字卡（可發音＋測驗模式）

這是一個純前端的單頁應用（Single File）。支援：搜尋、洗牌、TTS 發音（ja‑JP / zh‑TW）、測驗模式（先顯示日文，點卡片翻面）。

## 使用方法（GitHub Pages）

1. 新增一個 GitHub 倉庫（例如：`jp-vocab-cards`）。
2. 上傳 `index.html` 到倉庫根目錄。
3. 到 **Settings → Pages**：
   - Source 選擇「Deploy from a branch」
   - Branch 選擇 `main`（或你使用的分支），資料夾選 `/ (root)`
   - 儲存後等 1～2 分鐘，頁面會出現在：`https://<你的帳號>.github.io/<倉庫名稱>/`
4. 用手機 Safari/Chrome 開啟，按「分享」→「加入主畫面」即可像 App 一樣使用。

## 自訂單字

- 打開 `index.html`，搜尋 `const DATA = [...]`，把裡面的物件陣列換成你自己的單字。
- 格式為：
```js
{{ 日文: "図書館", 假名: "としょかん", 中文意思: "圖書館" }}
```

## 注意事項

- 發音使用瀏覽器的 SpeechSynthesis。若沒有日文/中文語音，請在系統設定中安裝對應語音包，或改用支援的瀏覽器（Safari/Chrome）。
