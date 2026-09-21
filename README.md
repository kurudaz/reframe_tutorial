# Reframe（重構）簡易教學

這是一份可直接放到 GitHub Pages 的靜態 HTML 教學，包含三張步驟截圖與三支 GIF。手機、平板與電腦皆可閱讀，不需要安裝套件或執行建置。

## 本機閱讀

直接用瀏覽器開啟 `index.html`。請保留同層的 `assets` 資料夾。

如需透過本機伺服器預覽，可在此資料夾執行：

```sh
UV_CACHE_DIR="$PWD/.cache/uv" uv run --no-project --python 3.12 python -m http.server 8765 --bind 127.0.0.1
```

然後開啟 `http://127.0.0.1:8765`。

## 放到 GitHub Pages

1. 建立或開啟要使用的 GitHub repository。
2. 將這個資料夾內的 `index.html`、`assets` 資料夾、`.nojekyll` 放到 repository 根目錄並提交。不要只上傳 ZIP；也不要多包一層 `reframe-guide` 資料夾。
3. 到 repository 的 **Settings → Pages**。
4. 在 **Build and deployment → Source** 選 **Deploy from a branch**。
5. 選 **main**（或實際放檔案的分支），資料夾選 **/ (root)**，按 **Save**。
6. 發布完成後，Pages 設定畫面會顯示網站網址。

專案網站通常是 `https://帳號.github.io/repository名稱/`。所有圖片都使用相對路徑，可放在這類子路徑。也可放到既有 Pages 網站的子資料夾。

官方說明：https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site

## 動畫

- 三支 GIF 會循環播放，並提供暫停／播放按鈕。
- 系統啟用「減少動態效果」時，預設顯示靜態畫面，可自行按播放。
- GIF 1 的網頁副本降為 10 fps，維持原本約 4.4 秒的片長，以減少下載量。
- 原始截圖、GIF 與既有 PDF 均未修改。
- 網站不使用外部字型、分析追蹤或 CDN。
