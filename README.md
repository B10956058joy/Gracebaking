📌 Grace Baking – Recipe Management Web App

🔍 專案簡介

Grace Baking 是一個使用 Vue 3 製作的前端單頁應用（SPA），
目標是提供 家庭烘焙者 一個可以快速瀏覽、搜尋、收藏與列印食譜的輕量化管理工具。


本專案聚焦於：

清楚的資料結構設計
良好的使用者體驗
前端專案的可擴充性


🎯 使用情境

想快速依分類（蛋糕 / 餅乾 / 麵包）找到食譜
想調整份量後直接列印
不需要登入、不需要後端，單人使用即可


🧩 核心功能

📂 食譜分類與即時搜尋
❤️ 收藏喜愛食譜（localStorage）
⭐ 星等評分
👨‍🍳 依人數動態調整材料份量
🖨 列印友善版食譜頁面
📱 RWD（桌機 / 手機）

🛠 技術選擇
技術	            說明
Vue 3 (CDN)	      元件化與狀態管理
JavaScript (ES6)	核心邏輯實作
Tailwind CSS	    快速 UI 建構與一致性
localStorage	    儲存使用者偏好（收藏 / 評分）
GitHub Pages	    靜態網站部署

🧠 資料模型設計（目前版本）
Recipe {
  id: Number,
  name: String,
  category: String,
  shortDesc: String,
  ingredients: String[],
  steps: String[],
  favorite: Boolean,
  rating: Number
}

備註：
目前 ingredients 使用字串格式以加快開發速度，
後續可重構為 { name, amount, unit } 結構以提升可維護性。


⚠️ 目前限制與取捨

使用 localStorage，未支援跨裝置同步
無登入系統（刻意縮小 scope）
所有資料為前端模擬資料


🚀 未來可擴充方向
串接 RESTful API
拆分為多個 Vue 元件
使用 Pinia 進行狀態管理
加入後端與使用者帳號系統


🔗 Demo
👉 https://b10956058joy.github.io/Grace-baking/
