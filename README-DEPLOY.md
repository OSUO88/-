# 心理學派互動學習｜GitHub Pages 部署

這個資料夾可直接作為 GitHub 儲存庫根目錄。網站是靜態 HTML，部署後可透過 GitHub Pages 的 HTTPS 網址公開瀏覽。

## 首次部署

1. 在 GitHub 建立一個儲存庫，並選擇要使用的名稱。網站內容會公開；請先確認要發布的資料已適合公開。
2. 用 GitHub Desktop 複製該儲存庫到電腦。
3. 將本資料夾中的 `.github`、`assets`、`index.html`、`exam-content.js`、`.gitignore` 和本說明檔複製到剛複製的儲存庫根目錄。不要把整個「心理學派互動學習」資料夾再包成一層。
4. 在 GitHub 儲存庫的 **Settings → Pages → Build and deployment → Source** 選 **GitHub Actions**。
5. 在 GitHub Desktop 提交並推送到 `main` 分支。GitHub Actions 會自動部署；到 **Actions** 確認「Deploy site to GitHub Pages」工作流程成功。
6. 回到 **Settings → Pages** 開啟網站網址。GitHub Pages 網址使用 HTTPS；若頁面提供 **Enforce HTTPS** 選項，請勾選。

## 網站更新

修改 `index.html`、`exam-content.js` 或 `assets/dog-collection/` 後，提交並推送到 `main`，Pages 會再次部署。工作流程只發布這些執行網站需要的檔案；舊版 HTML 備份與未使用的 `assets/dog-rewards/` 不會放進網站成品。

如果之後改用自訂網域，需另外設定網域 DNS 與 HTTPS；本設定使用 GitHub 提供的 `github.io` 網址。