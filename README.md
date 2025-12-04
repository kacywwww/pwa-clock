# iPhone 6s Desktop Clock (PWA) 🕰️

[English](#english) | [中文說明](#chinese)

---

<a name="english"></a>
## English Description

A lightweight, low-power Progressive Web App (PWA) clock designed specifically to repurpose older iOS devices (e.g., iPhone 6s) as dedicated desktop clocks. 

It is optimized for **Legacy iOS versions (iOS 11+)**, ensuring compatibility where modern web standards might fail.

[**🔗 Live Demo**](https://kacywwww.github.io/pwa-clock/)

### ✨ Features

* **Dual Mode Display:**
    * **Digital:** Large, easy-to-read typeface with date and seconds.
    * **Analog:** Classic watch face with Roman/Arabic numerals, precise ticks, and a sweeping second hand.
* **Legacy Support (iOS 11 Ready):**
    * Codebase adapted for older Safari engines (Polyfilled `padStart`, ES5 syntax safety).
    * Works flawlessly on iPhone 6s running iOS 11 through iOS 15.
* **PWA & Offline First:**
    * Supports "Add to Home Screen" for a full-screen, app-like experience.
    * **Zero Network Dependency:** Runs completely offline via Service Worker caching (perfect for Airplane Mode).
* **Low Power Design:**
    * Pure black background (`#000000`) to minimize LCD backlight power consumption.
    * Efficient DOM updates.
* **User Experience:**
    * **State Persistence:** Remembers your last used mode (Digital/Analog) via LocalStorage.
    * **Floating Switch:** Discrete button to toggle modes, placed to avoid accidental touches.

### 📱 Installation & Usage

1.  Connect your iPhone to Wi-Fi.
2.  Open Safari and visit the [Demo Link](https://kacywwww.github.io/pwa-clock/).
3.  Tap the **Share** button (bottom center).
4.  Select **"Add to Home Screen"**.
5.  Launch the app from your home screen.
    * *Tip: Enable "Airplane Mode" and set Auto-Lock to "Never" for the best dedicated clock experience.*

### 🛠️ Technical Details

* **Stack:** Vanilla JavaScript, HTML5, CSS3.
* **Compatibility Fixes:**
    * Replaced `String.prototype.padStart()` with custom helper functions for iOS 11 support.
    * Removed `backdrop-filter` to prevent rendering artifacts on older GPUs.
    * Used `var` and standard function declarations for maximum JS engine compatibility.

### 📝 License

Distributed under the MIT License. See `LICENSE` for more information.

---

<a name="chinese"></a>
## 中文說明 (Chinese)

這是一個極輕量、低功耗的網頁時鐘 (PWA)，專為活化舊款 iOS 設備（如 iPhone 6s）而設計。

特別針對 **舊版 iOS (iOS 11+)** 進行了程式碼優化，解決了舊版 Safari 不支援現代語法的問題，讓舊手機能夠穩定地作為桌上時鐘使用。

[**🔗 線上預覽 (Live Demo)**](https://kacywwww.github.io/pwa-clock/)

### ✨ 功能特色

* **雙模式顯示切換：**
    * **數位模式 (Digital)：**大字體清晰顯示時間、日期與秒數。
    * **指針模式 (Analog)：** 模擬經典腕錶設計，包含精確刻度 (Ticks) 與掃秒指針。
* **舊系統相容 (iOS 11 Ready)：**
    * 針對舊版 WebKit 引擎優化（手動實作 `padStart`，使用高相容性 ES5 寫法）。
    * 在 iOS 11 至 iOS 15 的 iPhone 6s 上皆可完美運行。
* **PWA 離線支援：**
    * 支援「加入主畫面」功能，隱藏瀏覽器網址列，提供全螢幕體驗。
    * **完全離線執行：** 透過 Service Worker 快取核心檔案，開啟飛航模式也能運作。
* **低功耗設計：**
    * 純黑背景 (`#000000`) 降低 LCD 背光耗電。
    * 極簡化 DOM 操作，減少 CPU 喚醒。
* **使用者體驗：**
    * **狀態記憶：** 使用 LocalStorage 自動記憶您偏好的時鐘模式。
    * **防誤觸設計：** 右下角懸浮切換按鈕。

### 📱 安裝與使用

1.  將 iPhone 連上網路。
2.  使用 Safari 開啟 [專案網址](https://kacywwww.github.io/pwa-clock/)。
3.  點擊下方 **分享 (Share)** 按鈕。
4.  選擇 **「加入主畫面」(Add to Home Screen)**。
5.  回到主畫面點擊圖示開啟。
    * *建議：開啟「飛航模式」並將螢幕「自動鎖定」設為「永不」，以獲得最佳省電效果。*

### 🛠️ 技術細節

* **核心：** 原生 JavaScript, HTML5, CSS3 (無外部依賴)。
* **相容性修正 (Patch for Legacy OS)：**
    * 由於 iOS 11 不支援 `padStart` API，已手動實作補零函式。
    * 移除 `backdrop-filter` 毛玻璃特效以確保舊硬體渲染流暢度。
    * 變數宣告採用 `var` 以確保在舊版 JavaScriptCore 引擎上的穩定性。

### 📝 授權 (License)

本專案採用 MIT License 授權，歡迎自由修改與使用。
