# 口罩資訊地圖網
使用 Vue3 + Vue Cli 4.5.15、
Mapbox GL JS 地圖框架，
並以 Axios 串接口罩API之資訊應用網站。

UI 設計自行以 Figma 繪製，
並使用 Tailwind 搭配 SCSS 切版。

## 線上展示
[Demo](https://daylilystudio.github.io/maskmap/)

## 功能
1. 左側欄
- 收合按鈕可將左側欄收起
- 初始狀態：
  - 顯示所在地附近 5 公里內的藥局（依近到遠排列）
  - 若無法取得 User 所在地，就顯示API的前50筆資料
- 搜尋與篩選：
  - 輸入關鍵字可搜尋目前左側卡片清單中的藥局名
  - 點選縣市左側卡片顯示該縣市藥局清單
  - 點選開關顯示所有標記過★號的藥局
- 藥局資訊卡：
  - 點擊藥局名地圖會移置該藥局圖標
  - 顯示與 User 所在地距離 (如果有開定位)
  - 可標記號★用於篩選（記錄在localStorage）
  - 口罩數量，並依數量多寡顯示不同顏色（充足、少量、無庫存）
  - 點擊「開啟地圖」，會打開Google地圖，並顯示該藥局位置
  - 點擊「撥打電話」可撥打藥局電話

2. 地圖
- 初始狀態：
  - 顯示所在地附近 5 公里內的藥局地圖圖標
  - 若無法取得 User 所在地，地圖視角顯示預設地點
- 圖標：
  - 圖標依大人口罩數量多寡顯示不同顏色（充足、少量、無庫存）
  - 點擊圖標後左側卡片會滾動至該圖標之藥局卡片
- 功能按鈕：
  - 點i可查看口罩數量顏色提示等資訊解說
  - 點＋–可放大、縮小地圖

## 介面展示
- Desktop UI
  ![Desktop UI](https://i.imgur.com/iy4udjP.jpeg)

- Mobile UI

  ![Mobile UI](https://i.imgur.com/ehUBI4e.jpeg)

- Color Guildline

  ![Color Guildline](https://i.imgur.com/4l0pWV8.png)
