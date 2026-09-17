# 日常食記 · Vic

Firebase 靜態 PWA 版飲食與生活行為紀錄 App。

- GitHub Pages 直接開啟 App
- Google 登入
- Firestore 跨裝置同步
- 手動記錄每餐食物與 9 類份數
- 記錄喝水、睡眠、步數、運動、排便、垃圾食物與保健品

Firebase 資料使用 `users/{uid}/data/nutrition-journal-main`，不會混用打工薪水 App 的資料文件。

## PWA 更新規則

`sw.js` 的 cache 名稱使用 `nutrition-YYYY-MM-DD-N`。

- `YYYY-MM-DD` 使用台北時間的修改日期
- `N` 以此專案累積第幾次推上線為主；多個本機修改還沒推時，仍共用同一個版本號
- 例：`nutrition-2026-09-18-2`
