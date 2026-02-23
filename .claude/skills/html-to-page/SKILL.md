---
name: html-to-page
description: 將 docs/Landing.html 轉換為 Next.js 的 app/page.tsx
argument-hint: （不需要額外參數，直接執行即可）
---

請執行以下步驟，將 Landing Page 的 HTML 轉換為 Next.js 元件：

1. 讀取 `docs/Landing.html` 檔案
2. 將內容轉換為合法的 Next.js React 元件，遵守以下規則：
   - 將所有 `class=` 改為 `className=`
   - 將 inline `style="..."` 字串改為 React style 物件格式（屬性名稱改為 camelCase，例如 `background-color` → `backgroundColor`）
   - 移除 `<html>`、`<head>`、`<body>` 標籤，只保留 body 內的內容
   - 移除所有 `<script>` 標籤
   - 圖片的 `src` 屬性保持原樣不做修改
   - 保留所有原始的 class 名稱與文字內容
3. 將轉換結果寫入 `app/page.tsx`，格式如下：

```tsx
export default function Home() {
  return (
    // 轉換後的 JSX
  )
}
```

完成後告知我已寫入 `app/page.tsx`，不需要在對話中顯示完整程式碼。
