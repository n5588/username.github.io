# CAD 看圖與測量工具 (手機 APP 安裝包)

本壓縮檔已包含完整的可離線執行 **PWA 網頁應用程式** 與 **Capacitor 原生封裝設定**，可透過以下兩種方式安裝至手機：

---

## 方式一：直接部署為手機可安裝 APP (PWA，支援 iOS 與 Android，免電腦編譯)

1. 將 `www/` 資料夾內的所有檔案（`index.html`、`manifest.json`、`sw.js`、`icon-192.png`、`icon-512.png`）上傳至任一支援 HTTPS 的免費靜態空間（例如 **GitHub Pages**、**Cloudflare Pages**、**Vercel** 或 **Netlify**）。
2. 使用手機瀏覽器開啟網址：
   - **iPhone (Safari)**：點擊底部「分享」按鈕 → 選擇「**加入主畫面**」。
   - **Android (Chrome)**：點擊右上角「⋮」→ 選擇「**安裝應用程式**」。
3. 安裝後即會在手機桌面產生專屬圖示，點擊可全螢幕開啟且支援完全離線看圖與測量。

---

## 方式二：打包成 Android APK / iOS IPA 原生安裝檔 (Capacitor)

若需產出 `.apk` 檔案直接傳給他人安裝，請在電腦執行以下指令：

```bash
npm init -y
npm install @capacitor/core @capacitor/cli @capacitor/android
npx cap add android
npx cap copy android
npx cap open android
```
開啟 Android Studio 後，點選上方選單 **Build → Build Bundle(s) / APK(s) → Build APK(s)** 即可產出可安裝的 `.apk` 檔。
