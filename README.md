<div align="center">

# 🛰️ 低軌衛星資訊應用 × LINE 推播

### 用低軌衛星觀測資料，打造你的即時推播系統

[![GitHub Pages](https://img.shields.io/badge/GitHub%20Pages-線上簡報-blue?style=for-the-badge&logo=github)](https://chatgpt3a01.github.io/leo-satellite-line-bot/)
[![License](https://img.shields.io/badge/授權-阿亮老師課程專用-red?style=for-the-badge)](LICENSE)

<img src="https://img.shields.io/badge/NASA-POWER%20API-0B3D91?style=flat-square&logo=nasa" />
<img src="https://img.shields.io/badge/LINE-Messaging%20API-00C300?style=flat-square&logo=line&logoColor=white" />
<img src="https://img.shields.io/badge/Google-Apps%20Script-4285F4?style=flat-square&logo=google&logoColor=white" />
<img src="https://img.shields.io/badge/Sentinel--2-ESA-003399?style=flat-square" />
<img src="https://img.shields.io/badge/時長-60～90%20分鐘-FD7E14?style=flat-square" />

</div>

---

## 📋 專案簡介

這是一套 **60～90 分鐘**的完整實作教學，帶你從零開始：

> 🛰️ **認識低軌衛星** → 📡 **呼叫 NASA API** → 📊 **解讀衛星資料** → 📲 **LINE 互動機器人**

學生跟著操作，就能打造一套「**低軌衛星觀測 LINE 互動機器人**」，在 LINE 中輸入地點，即時取得衛星觀測資料與生活建議分析！

---

## 🏗️ 系統架構

```
使用者在 LINE 輸入地點（如「台南」或「23.0, 120.2」）
        ↓
LINE Webhook 將訊息轉發至 Google Apps Script
        ↓
GAS 解析地點，呼叫 NASA POWER API 取得衛星觀測資料
        ↓
資料轉譯成「人看得懂的話」+ 生活建議分析
        ↓
LINE Reply API 即時回覆到使用者手機 📱
```

---

## 📊 課程內容

<table>
<tr>
<td width="50%">

### 🛰️ Part 1：認識低軌衛星
- 📌 什麼是低軌衛星（LEO）
- 📌 Sentinel-2 衛星介紹
- 📌 NDVI 植被指數概念
- 📌 衛星資料的應用場景

### 📡 Part 3：衛星資料 API 實作
- 🔧 什麼是 API（生活化比喻）
- 🔧 NASA POWER API 參數詳解
- 🔧 撰寫 GAS 取得衛星資料
- 🔧 解讀 JSON 回傳格式

### 🎯 Part 5：延伸應用與總結
- 🚀 設定每日自動排程
- 🚀 更換全球觀測地點
- 🚀 NDVI 植被監測進階
- 🚀 完整程式碼總覽

</td>
<td width="50%">

### ⚙️ Part 2：環境準備與設定
- 📌 NASA POWER API 介紹（免費！）
- 📌 LINE Developers 帳號建立
- 📌 取得 Channel Access Token
- 📌 建立 Google Apps Script 專案

### 📲 Part 4：LINE 推播整合
- 🔧 資料轉譯規則（數字→人話）
- 🔧 撰寫資料解讀函式
- 🔧 串接 LINE Messaging API
- 🔧 執行測試 — 成就感爆棚！

</td>
</tr>
</table>

---

## 🧰 使用工具

| 工具 | 說明 | 費用 | 連結 |
|:---:|:---|:---:|:---:|
| 🛰️ **NASA POWER API** | 衛星觀測資料（氣溫、降雨、濕度） | 免費，無需 Key | [前往官網 →](https://power.larc.nasa.gov/) |
| 💻 **Google Apps Script** | 雲端程式環境，瀏覽器就能寫 | 免費 | [前往使用 →](https://script.google.com/) |
| 📲 **LINE Messaging API** | 訊息推播服務 | 免費方案 | [前往設定 →](https://developers.line.biz/) |

---

## ✅ 前置需求

```
你需要什麼？
│
├─► Google 帳號 ──────► 用於 Google Apps Script
│
├─► LINE 帳號 ────────► 用於接收推播訊息
│
└─► 電腦 + 瀏覽器 ───► Chrome 或 Edge 即可
                        不用安裝任何軟體！
```

---

## 🚀 快速開始

1. **開啟課程簡報** → 從 Part 1 開始
2. **跟著步驟操作** → 每一步都有詳細說明
3. **完成實作** → 60～90 分鐘後，你的 LINE 就會收到衛星觀測日報！

---

## 📱 成果展示

完成後，在 LINE 中輸入城市名稱，機器人會即時回覆：

```
🛰️ 衛星觀測日報
━━━━━━━━━━━━
📍 地點：台南
📅 日期：20260210
━━━━━━━━━━━━
🌡️ 氣溫：18.5°C（涼爽 🍂）
📊 最高/最低：22.3°C / 15.1°C
💧 降雨量：0.2 mm（無降雨 ☀️）
💨 相對濕度：72%
━━━━━━━━━━━━
💬 衛星資料分析：
• 氣溫涼爽，建議攜帶薄外套
• 無降雨，適合戶外活動
━━━━━━━━━━━━
📡 資料來源：NASA POWER（低軌衛星觀測）
```

---

## 📂 專案結構

```
📦 低軌衛星資訊應用
├── 📄 index.html                    ← 課程首頁（統整頁）
├── 📄 Part1_認識低軌衛星.html        ← 低軌衛星概念
├── 📄 Part2_環境準備與設定.html      ← API 與 LINE 設定
├── 📄 Part3_衛星資料API實作.html     ← NASA API 串接
├── 📄 Part4_LINE推播整合.html        ← LINE 推播整合
├── 📄 Part5_延伸應用與總結.html      ← 延伸與完整程式碼
├── ⚡ GAS程式碼生成器.html           ← 一鍵生成 GAS 程式碼
├── 📄 README.md                     ← 本文件
└── 📄 LICENSE                       ← 授權聲明
```

---

<div align="center">

## 👨‍🏫 作者資訊

<img src="作者資訊.png" width="600" />

**曾慶良（阿亮老師）**

[![Facebook](https://img.shields.io/badge/Facebook-阿亮老師-1877F2?style=for-the-badge&logo=facebook&logoColor=white)](https://www.facebook.com/?locale=zh_TW)
[![YouTube](https://img.shields.io/badge/YouTube-阿亮老師-FF0000?style=for-the-badge&logo=youtube&logoColor=white)](https://www.youtube.com/@Liang-yt02)
[![3A社團](https://img.shields.io/badge/Facebook-3A科技研究社-1877F2?style=for-the-badge&logo=facebook&logoColor=white)](https://www.facebook.com/groups/2754139931432955?locale=zh_TW)

</div>

---

## 📜 授權聲明

```
© 2026 阿亮老師 版權所有

本專案僅供「阿亮老師課程學員」學習使用。

⚠️ 禁止事項：
  🚫 禁止修改本專案內容
  🚫 禁止轉傳或散布
  🚫 禁止商業使用
  🚫 禁止未經授權之任何形式使用

如有任何授權需求，請聯繫作者。
```

---

<div align="center">

### ⭐ 喜歡這個專案嗎？請給一個 Star！

**最後更新：2026-02-10**

[🔝 回到頂部](#-低軌衛星資訊應用--line-推播)

</div>
