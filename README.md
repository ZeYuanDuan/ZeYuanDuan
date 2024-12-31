## 嗨，我是段則元
我是一位具有哲學背景的後端工程師，擁有一年開發經驗。從探索抽象理論到開發網站系統，我對「解決問題」的熱忱始終如一。透過 ALPHA Camp 的培訓與自主學習，我習得後端開發的能力，完成多個專案，建立了紮實的技術基礎。

# 我的專案

## LivePoll

**類似 Slido 的即時投票平台，支援多裝置同步更新投票結果，讓使用者能快速參與互動。專案針對高併發、低延遲以及消息可靠性進行設計與優化。**

**【專案特色】**

-   **高併發與即時更新**：使用 Redis 搭配 WebSocket 處理高併發需求及即時更新，確保前端設備之間的數據同步快速且可靠。
-   **資料快取與持久性**：使用 Redis 儲存投票過程中的臨時狀態，並使用 MySQL 實現投票數據的長期持久化管理。
-   **消息可靠性 (message durability)**：整合 RabbitMQ 作為消息隊列，在高負載情況下提供可靠的消息傳遞機制。
-   **容器化與雲端部署**：採用 Docker 將服務容器化，並部署於 AWS EC2，結合 AWS RDS 進行資料庫管理，以提升系統擴展性與穩定性。

![【LivePoll】System Architecture.png](https://github.com/ZeYuanDuan/ZeYuanDuan/blob/main/%E3%80%90LivePoll%E3%80%91System%20Architecture.png "【LivePoll】System Architecture.png")


## Vocabulary Flashcards


**單字管理應用，利用第三方 API 每日自動推送新單字和例句，讓使用者儲存不熟悉的單字並自訂標籤進行分類。專案技術重點在於 API 開發、資料庫管理及身份驗證。**

  

**【專案特色】**

-   **API 設計與測試**：開發具完整 CRUD 功能的 RESTful API，用於管理用戶數據和單字清單，並使用 Postman 測試 API 邏輯。
-   **身分驗證**：使用 JWT 實現無狀態的身份驗證，並整合 Google OAuth 2.0 提供第三方登入服務。
-   **資料庫和快取**：採用 MySQL 作為主要資料庫，搭配 Redis 快取，提升數據讀取速度，減少伺服器負擔。
-   **每日任務自動化**：使用 CronJobs 排程每日從第三方 API 獲取單字，確保內容更新。

![Vocabulary Flashcards demo.png](https://github.com/ZeYuanDuan/ZeYuanDuan/blob/main/Vocabulary%20Flashcards%20demo.png "Vocabulary Flashcards demo.png")
