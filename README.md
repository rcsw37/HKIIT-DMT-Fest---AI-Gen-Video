# 第一屆香港資訊科技學院AI數碼媒體節：未來影格

純 HTML、CSS、JavaScript 版本 - 簡單易用，無需建置工具

---

## 📁 檔案結構

```
hkiit-festival-html/
├── index.html          # 主網頁檔案
├── css/
│   └── style.css       # 樣式檔案
├── js/
│   └── script.js       # JavaScript 功能
├── images/             # 圖片資源
│   ├── hkiit-logo.jpg
│   ├── index-academy-logo.png
│   └── SampleV4.pdf
└── README.md           # 本說明文件
```

---

## 🚀 快速開始

### 方法 1：直接開啟（最簡單）

1. 雙擊 `index.html` 檔案
2. 網頁會在預設瀏覽器中開啟

### 方法 2：使用 VS Code（推薦）

1. 用 VS Code 開啟整個 `hkiit-festival-html` 資料夾
2. 安裝 **Live Server** 擴充功能（如果還沒安裝）
3. 右鍵點擊 `index.html` → 選擇 **Open with Live Server**
4. 網頁會在瀏覽器中開啟，並且修改後會自動重新載入

### 方法 3：使用 Python 本地伺服器

```bash
# 在專案資料夾中執行
python -m http.server 8000

# 然後在瀏覽器開啟
# http://localhost:8000
```

---

## ✏️ 修改指引

### 1. 修改文字內容

**位置**：`index.html`

所有文字內容都在 HTML 檔案中，直接搜尋並修改即可。

**範例**：修改活動日期

```html
<!-- 搜尋 "2025年1月" -->
<div class="timeline-date">2025年1月</div>

<!-- 改為 -->
<div class="timeline-date">2025年2月</div>
```

### 2. 修改顏色

**位置**：`css/style.css` 的開頭

```css
:root {
    /* 修改這些顏色變數 */
    --primary-color: #3b82f6;      /* 主要藍色 */
    --secondary-color: #ec4899;    /* 次要粉紅色 */
    --accent-color: #8b5cf6;       /* 強調紫色 */
}
```

### 3. 更換圖片

**步驟**：

1. 將新圖片放入 `images/` 資料夾
2. 在 `index.html` 中搜尋舊圖片檔名
3. 替換為新圖片檔名

**範例**：

```html
<!-- 舊的 -->
<img src="images/hkiit-logo.jpg" alt="HKIIT">

<!-- 新的 -->
<img src="images/new-logo.png" alt="HKIIT">
```

### 4. 更新 Google Form

**位置**：`index.html` 搜尋 "iframe"

```html
<!-- 找到這段 -->
<iframe 
    src="https://docs.google.com/forms/d/e/YOUR_FORM_ID/viewform?embedded=true" 
    width="100%" 
    height="1636">
</iframe>

<!-- 替換 src 為您的新表單連結 -->
```

### 5. 修改字體

**位置**：`index.html` 的 `<head>` 區塊

```html
<!-- 修改 Google Fonts 連結 -->
<link href="https://fonts.googleapis.com/css2?family=您想要的字體&display=swap" rel="stylesheet">
```

然後在 `css/style.css` 中修改：

```css
:root {
    --font-chinese: '您的中文字體', sans-serif;
    --font-english: '您的英文字體', sans-serif;
}
```

---

## 🎨 設計特色

### 顏色方案
- **主色**：藍色 (#3b82f6) - 科技感
- **輔色**：粉紅色 (#ec4899) - 創意感
- **強調色**：紫色 (#8b5cf6) - 未來感

### 字體
- **中文**：Noto Sans TC（思源黑體）
- **英文**：Montserrat

### 響應式設計
- 自動適應桌面、平板、手機螢幕
- 手機版有專用選單

---

## 📤 部署到網路

### 方法 1：Netlify Drop（最簡單）

1. 前往 https://app.netlify.com/drop
2. 將整個 `hkiit-festival-html` 資料夾拖曳到網頁上
3. 等待上傳完成，會獲得一個網址
4. 完成！

### 方法 2：GitHub Pages

1. 在 GitHub 建立新儲存庫
2. 上傳所有檔案
3. 進入 Settings → Pages
4. 選擇 main branch → Save
5. 幾分鐘後網站就會上線

### 方法 3：Vercel

1. 前往 https://vercel.com
2. 註冊並連接 GitHub
3. 匯入您的儲存庫
4. Vercel 會自動部署

---

## 🔧 常見問題

### Q: 圖片無法顯示？
**A**: 檢查圖片檔案是否在 `images/` 資料夾中，檔名是否正確（區分大小寫）。

### Q: Google Form 無法載入？
**A**: 確認表單連結正確，並且表單設定為「允許嵌入」。

### Q: 手機版選單無法開啟？
**A**: 確認 `js/script.js` 檔案已正確載入。

### Q: 修改後沒有變化？
**A**: 
1. 清除瀏覽器快取（Ctrl+F5 或 Cmd+Shift+R）
2. 確認檔案已儲存
3. 如果使用 Live Server，檢查是否正在執行

### Q: 想要移除某個區塊？
**A**: 在 `index.html` 中找到對應的 `<section>` 標籤，刪除整個區塊即可。

---

## 📝 修改檢查清單

部署前請確認：

- [ ] 所有文字內容已更新
- [ ] 日期和時間正確
- [ ] Google Form 連結正確
- [ ] 圖片都能正常顯示
- [ ] 聯絡資訊正確
- [ ] 在不同瀏覽器測試（Chrome、Safari、Firefox）
- [ ] 在手機上測試響應式設計
- [ ] 所有連結都能正常運作

---

## 💡 進階技巧

### 添加新區塊

在 `index.html` 中複製現有的 `<section>` 區塊：

```html
<section class="section" id="new-section">
    <div class="container">
        <h2 class="section-title">新區塊標題</h2>
        <p class="section-subtitle">副標題</p>
        <!-- 您的內容 -->
    </div>
</section>
```

### 修改動畫速度

在 `css/style.css` 中搜尋 `transition`：

```css
/* 修改動畫時間（秒） */
transition: all 0.3s ease;  /* 改為 0.5s 會更慢 */
```

### 停用滾動動畫

在 `js/script.js` 中註解掉這段：

```javascript
// 將這些行註解掉
// observer.observe(el);
```

---

## 📞 技術支援

如有任何問題，請參考：

- **HTML 基礎**：https://www.w3schools.com/html/
- **CSS 教學**：https://www.w3schools.com/css/
- **JavaScript 入門**：https://www.w3schools.com/js/

---

## 📄 授權

本專案為第一屆香港資訊科技學院AI數碼媒體節專用。

---

**版本**：1.0  
**最後更新**：2025年1月  
**製作**：純 HTML/CSS/JS 版本，無需建置工具

