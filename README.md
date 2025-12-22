📌 Grace Baking – Recipe Management Web App

🔍 專案簡介
Grace Baking 是一個使用 Vue 3 製作的前端單頁應用（SPA），目標是提供 家庭烘焙者 一個快速瀏覽、搜尋、收藏與列印食譜的輕量化管理工具。
本專案聚焦於：

清楚的資料結構設計

良好的使用者體驗

前端專案的可擴充性

🎯 使用情境

想快速依分類（蛋糕 / 餅乾 / 麵包）找到食譜

想調整份量後直接列印

不需要登入、不需要後端，單人使用即可

🧩 核心功能與嘗試

食譜分類與即時搜尋：使用 Vue 的 computed 與 watch 實作動態過濾與排序

收藏喜愛食譜（localStorage）：嘗試將使用者偏好儲存在瀏覽器，實現跨頁面資料保存

星等評分功能：利用元件化設計，實作互動性評分系統

依人數動態調整材料份量：嘗試運用資料綁定與計算屬性，提升使用者操作便利性

列印友善版食譜頁面：調整 CSS 以提供乾淨的列印樣式

RWD（桌機 / 手機）：使用 Tailwind CSS 建立響應式介面

🛠 技術選擇與嘗試

技術	說明 / 嘗試
Vue 3 (CDN)	元件化設計與狀態管理，嘗試組件拆分與 props 傳遞
JavaScript (ES6)	核心邏輯實作，包括資料過濾、動態計算與事件監聽
Tailwind CSS	快速 UI 建構、響應式設計與列印樣式調整
localStorage	嘗試實作前端資料持久化，模擬簡單使用者資料儲存
GitHub Pages	靜態網站部署與版本控管實踐

🧠 資料模型設計（目前版本）

Recipe {
  id: Number,
  name: String,
  category: String,
  shortDesc: String,
  ingredients: String[], // 後續可改為 {name, amount, unit} 提升可維護性
  steps: String[],
  favorite: Boolean,
  rating: Number
}


⚠️ 目前限制與取捨

使用 localStorage，未支援跨裝置同步

無登入系統（刻意縮小 scope）

所有資料為前端模擬資料

🚀 未來可擴充方向

串接 RESTful API，實現跨裝置資料同步

拆分更多 Vue 元件，提高可維護性

使用 Pinia 進行全域狀態管理

加入後端與使用者帳號系統

🔗 Demo
👉 Grace Baking Demo
