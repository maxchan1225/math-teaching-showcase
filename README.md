# 數學教學軟件及電子教材展示網站

這是一個 Firebase Hosting + Firestore 的展示網站示例，支援教師即時貼上文字、上傳小型文檔或圖片。提交成功後，內容會寫入 Firestore，展示牆會即時更新並標示作者姓名。

## 功能

- 填寫作者姓名
- 直接貼上文字內容後上傳
- 可選擇附加圖片、PDF、文字檔、Word、PowerPoint
- 圖片與 PDF 可直接在頁面預覽
- 文字內容會直接出現在展示牆
- Firestore 即時監聽，新增內容後展示牆立即更新
- 只有管理員 Google 帳號 `qwer124@aol.com` 登入後可以移除展示內容

## 注意

本示例已跳過 Firebase Storage，檔案會以資料形式直接存到 Firestore，因此單檔上限為 650KB，適合教學展示和小型教材示例。

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
npx firebase-tools deploy --only hosting,firestore:rules --project teacherstudy-ac70b
```
