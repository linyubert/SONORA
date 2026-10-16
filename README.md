# 音樂角 — SONORA｜GitHub Pages 直接上傳版

此資料夾是已建置完成的網站，不是需要 npm 編譯的原始碼。

## 部署步驟

1. 建議建立一個新的 GitHub 儲存庫，避免混入先前的原始碼和部署設定。
2. 解壓縮 ZIP，將 index.html、assets 資料夾、fonts 資料夾等所有內容上傳至儲存庫根目錄。不要直接上傳 ZIP，也不要多包一層資料夾。
3. 到 Settings → Pages → Build and deployment。
4. Source 選擇 Deploy from a branch。
5. Branch 選擇 main，資料夾選擇 / (root)，按 Save。
6. 等待 GitHub Pages 部署成功，從 Settings → Pages 提供的網址開啟網站。

這個版本不需要自行建立 GitHub Actions，也不需要執行 npm。
不要只上傳 index.html；assets 和 fonts 必須一起上傳。

如果沿用舊儲存庫，請先移除舊的 src、public、package.json、package-lock.json、vite.config.js，以及 .github/workflows/deploy.yml，再上傳本包並改為上述 branch 發布方式，避免舊工作流程覆蓋網站。保留與本網站無關的個人檔案。

## 上傳後根目錄應包含

- index.html
- assets/（建置後的 CSS 與 JavaScript）
- fonts/（手寫字型及授權）
- .nojekyll（略過 Jekyll；如果檔案選取器隱藏此檔，這個沒有底線資源名稱的版本仍可發布）
- README.md

## 注意事項

- 請透過 GitHub Pages 網址開啟，不要直接在本機雙擊 index.html，也不要使用 github.com 的檔案預覽頁面。
- GitHub Pages 的網址通常包含 GitHub 帳號名稱。
- 第一次播放聲音需要使用者先點擊畫面。
- Google 網頁字型需要網路；離線時會使用系統字型。本地「禹承老師」手寫字型包含在 fonts/。
- 部署成功但仍顯示舊畫面時，請重新整理或以無痕視窗確認。

此版本保留黃綠運動服小人物、桌墊取景、左下方「禹承老師」、音感鐘操作與手機版，標題為「音樂角 / THE LISTENING CORNER」。
