# 台北 101 互動模型（Three.js）

單一 `index.html`，Three.js 0.170.0 由 jsDelivr CDN 載入，不需建置。

功能：日夜／天氣、導覽、電梯、跨年煙火、阻尼器示意、LED 跑馬燈、合成音效、紀念明信片。

## 本機執行
需要用本機伺服器（模組與 importmap 不能用 file:// 開啟）：

    python3 -m http.server 8000
    # 開啟 http://localhost:8000

## 部署到 GitHub Pages
1. 在 GitHub 建立新 repository（例如 `taipei101`）
2. 上傳本資料夾所有檔案到 `main` 分支
3. Settings → Pages → Source 選 `Deploy from a branch` → Branch 選 `main` / `(root)` → Save
4. 約 1 分鐘後網址：`https://<你的帳號>.github.io/taipei101/`

或用指令：

    git init -b main && git add . && git commit -m "Taipei 101 Three.js"
    git remote add origin https://github.com/<你的帳號>/taipei101.git
    git push -u origin main
