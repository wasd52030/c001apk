<div align="center">

<img src="docs/media/banner.svg" alt="c001apk — 讓酷安，輕一點。" width="100%">

# c001apk

**輕量的非官方酷安用戶端**

[![License: AGPL v3](https://img.shields.io/badge/License-AGPL_v3-607D8B?style=flat-square)](LICENSE)
[![Flutter](https://img.shields.io/badge/Flutter-3.47.7-02569B?style=flat-square&logo=flutter&logoColor=white)](docs/DEVELOPMENT.md)
[![Build](https://github.com/TG-Twilight/c001apk/actions/workflows/build.yml/badge.svg?branch=main)](https://github.com/TG-Twilight/c001apk/actions/workflows/build.yml)
![Platforms](https://img.shields.io/badge/平台-Android%20%7C%20Windows-486B78?style=flat-square)
![Status](https://img.shields.io/badge/狀態-持續維護中-6E8B74?style=flat-square)

[下載最新版](https://github.com/TG-Twilight/c001apk/releases/latest) · [回報問題](https://github.com/TG-Twilight/c001apk/issues) · [參與開發](docs/DEVELOPMENT.md)

</div>

## 關於

基於 [c001apk-flutter](https://github.com/bggRGjQaUbCoE/c001apk-flutter) 持續維護的非官方酷安用戶端，主要支援 Android 與 Windows。在輕量、簡體中文的瀏覽體驗上，加入 HDR／Live 實況圖片、液態玻璃、大螢幕閱讀和本機內容過濾，由於對『 android.permission.QUERY_ALL_PACKAGES 』權限的反感，特fork來ban掉該權限

## 特色功能

除了輕量瀏覽之外，也持續改善圖片瀏覽、內容閱讀和內容篩選的體驗。

| 功能 | 可以做什麼 |
| --- | --- |
| **HDR 圖片** | 在裝置與顯示條件支援的情況下呈現 HDR 高光；不支援 HDR 時則載入高畫質 SDR。支援儲存原始檔，也可開啟「我不想看 HDR」，讓靜態大圖一律使用高畫質 SDR。 |
| **Live 實況圖片** | 在大圖檢視器中播放實況圖片，支援自動播放一次、手動循環播放，以及儲存實況原始檔。 |
| **液態玻璃** | 頂部分類、懸浮導覽、搜尋和選單會隨背景內容呈現折射與色散效果，提供低／中／高／完整四種強度，也可以關閉。 |
| **悄悄關注** | 將感興趣的使用者加入本機名單，集中瀏覽其動態，無須向帳號發起關注操作；訪客也可使用本機關注功能。 |
| **貼文／文章儲存** | 將正文、作者、來源及部分留言匯出為 Markdown 或離線 HTML；HTML 可將圖片內嵌在同一個檔案中，方便離線閱讀與歸檔。 |
| **屏蔽傻逼內容** | 依照個人瀏覽偏好減少低俗內容的干擾。提供標準／嚴格兩種模式、話題與作者名單、文字規則、個人規則及訂閱更新；列表會靜默過濾，支援例外與暫時檢視。預設關閉，僅影響本機顯示。 |
| **桌面與大螢幕閱讀** | 動態牆會隨視窗寬度切換為一至四欄，閱讀時正文置中，右側可繼續瀏覽；支援即時縮放視窗、獨立捲動、鍵盤操作與滑鼠前進／後退側鍵。 |

同時保留動態／文章／留言瀏覽、內容搜尋、多帳號、訪客模式、本機收藏與瀏覽紀錄，以及明暗主題、閱讀字級和首頁分類自訂。

## 介面預覽

Android · M3E 標準介面（1.5.2，2026-11-08）

<p align="center">
  <img src="docs/media/screenshots/android-home-1.5.2.avif" width="31%" alt="Android M3E 首頁：標準頂部分類、動態列表與底部導覽列，關閉懸浮控制項">
  <img src="docs/media/screenshots/android-article-1.5.2.avif" width="31%" alt="Android M3E 圖文詳細頁：封面、正文與圖片">
  <img src="docs/media/screenshots/android-settings-1.5.2.avif" width="31%" alt="Android M3E 分類設定：外觀、關注、隱私、儲存空間與帳號管理">
</p>
<p align="center"><sub>Android · 首頁／圖文詳細頁／分類設定</sub></p>

<details>
<summary>Android · 開啟液態玻璃（1.5.2，點擊展開）</summary>

<p align="center">
  <img src="docs/media/screenshots/android-liquid-glass-1.5.2.avif" width="45%" alt="Android 深色主題下開啟液態玻璃：頂部分類列與底部懸浮導覽列折射背後的圖片內容">
  <img src="docs/media/screenshots/android-liquid-glass-follow-1.5.2.avif" width="45%" alt="Android 關注頁液態玻璃：使用者關注分類、搜尋按鈕與底部懸浮導覽列折射背後的內容">
</p>
<p align="center"><sub>Android · 液態玻璃：首頁／關注 · 2026-11-08</sub></p>

</details>

Windows · 1.5.2（2026-11-08）

<p align="center">
  <img src="docs/media/screenshots/windows-home-1.5.2.avif" width="96%" alt="Windows 桌面版首頁：液態玻璃懸浮側邊欄、頂部分類與三欄動態牆">
</p>
<p align="center"><sub>Windows · 懸浮導覽與三欄動態牆</sub></p>

<p align="center">
  <img src="docs/media/screenshots/windows-reading-1.5.2.avif" width="96%" alt="Windows 大螢幕閱讀：置中正文、右側作者卡片與繼續瀏覽動態牆">
</p>
<p align="center"><sub>Windows · 置中閱讀與右側繼續瀏覽</sub></p>

<p align="center">
  <img src="docs/media/screenshots/windows-settings-1.5.2.avif" width="96%" alt="Windows 分類設定：左側分類與右側外觀、懸浮控制項及液態玻璃選項">
</p>
<p align="center"><sub>Windows · 分類設定與寬視窗版面</sub></p>

## 下載與安裝

從本專案的 [Releases](https://github.com/TG-Twilight/c001apk/releases/latest) 下載正式完整版。本次 README 對應版本為 **1.5.2**，更新內容請參閱 [版本發行說明](https://github.com/TG-Twilight/c001apk/releases/tag/1.5.2-release)。

| 平台 | 安裝套件與支援情況 |
| --- | --- |
| **Android** | 提供 arm64-v8a、armeabi-v7a、x86_64，最低需求為 Android 7.0；多數近年的手機請選擇 arm64-v8a。 |
| **Windows** | 提供 x86_64 壓縮檔，解壓縮完整資料夾後執行 `c001apk.exe`，請保留同目錄下的 DLL 與 data 資料夾。 |
| **Linux** | 提供 x86_64 建置版本，實際執行體驗仍待驗證。 |
| **iOS** | 提供 arm64 未簽署 IPA，需自行簽署後安裝，實際執行體驗仍待驗證。 |

自行建置請參閱 [開發指南](docs/DEVELOPMENT.md)。

雲端建置套件可從 [Actions](https://github.com/TG-Twilight/c001apk/actions/workflows/build.yml) 的 Artifacts 下載，各平台、簽署與手動建置方式請參閱 [雲端建置指南](docs/CI.md)。

反覆遇到人機驗證時，可在引導流程或裝置設定中主動取得數盟 ID，也可參閱 [從官方酷安匯入裝置識別碼](docs/DEVICE_ID_IMPORT.md) 手動匯入。不會在啟動或返回前景時自動取得識別碼；取得或匯入裝置識別碼不保證能永久免除驗證。

## 使用說明

- **悄悄關注**：在設定中開啟後，長按使用者個人頁面的關注按鈕即可加入名單。名單僅儲存在本機，不會自動同步至帳號。
- **儲存貼文／文章**：在詳細頁面點選「儲存內容」，選擇 Markdown 或離線 HTML。儲存內容最多包含三則第一層留言，不包含全部留言、樓中樓或影片；圖片下載失敗時會提示確認。
- **內容過濾**：在「設定 → 內容屏蔽 → 屏蔽傻逼內容」中開啟。標準模式較為寬鬆，嚴格模式則包含標準規則並進一步加強過濾，誤判的可能性也較高；可調整分類、加入個人規則或暫時檢視。此功能不會呼叫帳號封鎖或檢舉 API。
- **液態玻璃**：在「設定 → 外觀與導覽」中開啟懸浮控制項與液態玻璃，並選擇效果強度。
- **HDR 與實況圖片**：「我不想看 HDR」只會改變靜態大圖的顯示方式，不影響實況播放、縮圖素材標示及原始檔儲存。

Android 套件名稱與其他實現不同，可與其他套件名稱的客戶端獨立安裝，帳號及本機資料不會自動遷移。

> [!NOTE]
> 部分內容仍受到登入、人機驗證和伺服器端 API 限制，驗證通過後的處理及部分帳號操作仍有待完善。

## 參與開發與致謝

歡迎提交 [Issue](https://github.com/TG-Twilight/c001apk/issues) 或 Pull Request。回報問題時請附上平台、版本、重現步驟及已去除敏感資訊的錯誤訊息；開發環境、專案目錄及檢查指令請參閱 [開發指南](docs/DEVELOPMENT.md)。

感謝 [bggRGjQaUbCoE/c001apk-flutter](https://github.com/bggRGjQaUbCoE/c001apk-flutter) 開放原始碼，以及 [daimiaopeng/coolapk-desktop](https://github.com/daimiaopeng/coolapk-desktop) 提供協定研究方面的參考。

感謝 [kongwufang](https://github.com/kongwufang) 透過 [PR #11](https://github.com/TG-Twilight/c001apk/pull/11) 貢獻數字聯盟裝置識別碼自動取得功能，以及配套的離線測試、實測紀錄與授權說明。

本專案沿用 [GNU AGPL v3](LICENSE) 授權條款，第三方來源與 MIT 授權資訊請參閱 [第三方聲明](docs/THIRD_PARTY_NOTICES.md)。本專案與酷安官方並無隸屬關係，酷安名稱、商標及服務內容均歸相應權利人所有。
