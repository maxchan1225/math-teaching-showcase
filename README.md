# 數學教學軟件及電子教材展示網站

這是一個 Firebase Hosting 展示網站示例，支援教師即時上傳數學教學文件與圖片。上傳成功後，內容會寫入 Firebase Storage，教材資料會寫入 Firestore，展示牆會即時更新並標示作者姓名。

## 功能

- 上傳圖片、PDF、文字檔、Word、PowerPoint 等教材檔案
- 必填作者姓名、教材標題與數學主題
- 圖片與 PDF 可直接在頁面預覽
- 文字檔會顯示內容摘要
- Firestore 即時監聽，新增教材後展示牆立即更新
- Firebase Storage 儲存檔案，Firestore 儲存作者與教材資訊

## Firebase

目前配置使用 Firebase 專案：

```text
teacherstudy-ac70b
```

Hosting target：

```text
math-teaching-showcase
```

部署：

```bash
firebase deploy
```
