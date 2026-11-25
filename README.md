# STAR CATCH｜星星收集

這是一個可直接部署到 GitHub Pages 的靜態網站。遊戲不需要伺服器或資料庫；最高分與排行榜存在玩家自己的瀏覽器（localStorage）。

## 專案檔案

- `index.html`：網站結構、遊戲畫面與分享／QR Code 頁面
- `style.css`：網站樣式與手機版排版
- `game.js`：遊戲規則、操作、音效、分數與 QR Code 產生功能

## 免費發布到 GitHub Pages

1. 登入 GitHub，開啟 `kahe05824-cloud/banana` 儲存庫。
2. 進入 **Settings** → 左側 **Pages**。
3. 在 **Build and deployment** 的 **Source** 選 **Deploy from a branch**。
4. Branch 選 `main`，資料夾選 `/(root)`，按 **Save**。
5. 等待 GitHub Pages 完成發布。

網站網址通常是：

`https://kahe05824-cloud.github.io/banana/`

## 產生自己的 QR Code

1. 網站發布成功後，開啟網站的「分享／QR Code」分頁。
2. 貼上完整的 GitHub Pages 網址，例如 `https://kahe05824-cloud.github.io/banana/`。
3. 按「產生 QR Code」。
4. 按「下載 QR Code PNG」，把圖片存到自己的電腦或手機。

QR Code 直接編入你的 GitHub Pages 網址，不是短網址，也沒有隔天到期設定。只要 GitHub 帳號、儲存庫與 Pages 網站仍存在且網址不變，原本下載的 QR Code 就會繼續有效。

## 如何更新遊戲

修改檔案後，再到 GitHub 儲存庫上傳同名新檔案並提交。GitHub Pages 會自動重新部署。若瀏覽器仍顯示舊版，請強制重新整理。

## 功能與限制

- 電腦：使用鍵盤 ← → 或 A / D。
- 手機／平板：在遊戲畫面上左右拖曳。
- 漏接任何星星：立即結束。
- 碰到炸彈：立即結束（護盾道具可抵擋一次）。
- 藍色寶石：+5 分；護盾：短暫保護。
- 分數與排行榜存在「各玩家自己的瀏覽器」，不是所有訪客共用的線上排行榜。
- QR Code 產生器使用 QRCode.js CDN，因此產生 QR Code 時需要網路連線；遊戲核心本身不依賴這個程式庫。
- 網站使用 Google Fonts 與 QRCode.js 的 CDN；若要完全不依賴第三方 CDN，可把字型及 QRCode.js 程式庫下載後改成專案內的本機檔案。

## 重要

GitHub Pages 是免費靜態網站代管，不是對永久存續作保證。只要帳號與網站持續有效，網址及 QR Code 就能持續使用。
