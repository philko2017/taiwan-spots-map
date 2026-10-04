# 🗺️ 台灣景點分類地圖應用 / Taiwan Scenic Spots & Route Planner

👉 **公開線上體驗網址**：[https://philko2017.github.io/taiwan-spots-map/](https://philko2017.github.io/taiwan-spots-map/)  
*(免下載 App、無廣告、免登入，電腦與手機瀏覽器皆可直接使用)*

---

## 💡 起心動念 / Motivation

### 中文說明
在規劃旅遊或日常私房景點時，市面上的地圖應用常充斥著商業廣告、繁複的選單，以及在「儲存地點」與「規劃路線」之間割裂的操作體驗。

這套小工具誕生的初衷非常純粹：

**「我希望能有一張乾淨、純粹屬於自己的地圖，可以自由建立彩色分類書籤；更重要的是，能透過最直覺的拖曳排序，自動把同一分類的地點依序連成一條動線（1 ➔ 2 ➔ 3），讓行程規劃一眼看清、輕鬆順暢。」**

無需複雜的登入、沒有追蹤廣告、不需依賴龐大的伺服器後端，打開瀏覽器就能直接規劃與出發。

### English
When planning trips or collecting favorite spots, modern map services are often cluttered with commercial ads, complex menus, and a disconnected workflow between "saving bookmarks" and "drawing itineraries".

This tool was created with a clear and focused vision:

**"A clean, ad-free personal map where I can easily organize custom categorized bookmarks with distinct colors, and instantly connect stops in sequential order (1 ➔ 2 ➔ 3) using intuitive drag-and-drop reordering, making travel itinerary planning completely effortless."**

Zero tracking, zero backend dependencies, and zero setup. Just open in any browser across desktop and mobile devices.

---

## 📖 如何使用 / How to Use

1. **直接開啟使用**：點擊公開網址 [https://philko2017.github.io/taiwan-spots-map/](https://philko2017.github.io/taiwan-spots-map/)。
2. **新增與自訂分類**：在左側面板點選調色盤自訂專屬色彩，建立新分類（例如：「Day 1 海線」、「咖啡甜點」、「必吃美食」）。
3. **搜尋或點選地點**：輸入地名（如「台北101」）搜尋，或直接點擊地圖任意處，自動帶入經緯度並加入景點。
4. **自動順序連線**：同一分類有 2 個以上地點時，地圖會自動以淺色虛線與數字序號（1 ➔ 2 ➔ 3）依序串聯。
5. **上下拖曳調整順序**：展開分類清單，按住地點左側的 `⠿` 圖示上下拖曳，連線與序號瞬間自動更新。
6. **手機加到主畫面**：手機瀏覽器（iOS Safari / Android Chrome）點選「分享」➔「加入主畫面」，即可像原生 App 一樣全螢幕隨開隨用。

---

## ✨ 核心特色 / Key Features

- **🏷️ 自訂分類與即時調色盤**：自由建立彩色分類，即時連動地圖圖釘與右下角圖例。
- **🛣️ 順序連線與拖曳排序**：清單支援滑鼠與手機觸控拖曳排序（`⠿` 圖示），動態連線與數字序號隨拖曳即時重繪。
- **🔍 雙引擎地名搜尋**：整合 OSM Nominatim 與 Photon 雙搜尋引擎，輸入地名自動定位。
- **🗺️ 多元圖資一鍵切換**：右上角提供顯眼的懸浮切換按鈕，支援 Google 繁中街道圖、Google 衛星混合圖、OSM 人道救援圖與 Esri 地形圖。
- **🔒 100% 本地隱私與離線儲存**：所有資料皆儲存在使用者當前裝置的 `localStorage`，不回傳任何伺服器。

---

## 🛠️ 技術架構 / Tech Stack

- **Map Engine**: Leaflet 1.9.4
- **Map Tiles**: Google Maps, OpenStreetMap Humanitarian (HOT), Esri World Street / Topo
- **Geocoding API**: OpenStreetMap Nominatim & Komoot Photon
- **Architecture**: Single-file static web application (`index.html`), Vanilla JavaScript, CSS3
- **Persistence**: Browser `localStorage` (No server / database required)

---

## 📄 授權條款 / License

本專案採 MIT 開源授權，歡迎自由修改與分享。
