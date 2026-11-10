# 這一站，青春 (青春という名の一駅) - Vibe Coding 與 Prompt 說明文件

本專題網頁是透過 AI 協同開發（Vibe Coding）完成的大二影展專題網站。以下為製作過程中所使用的 Prompt 指令與開發筆記記錄，供作業評分與技術交流使用。

---

## 一、 核心 Prompt 設計思維與指令拆解

在本次開發中，我們將企劃書 PDF 的所有核心內容（包含執行摘要、現況分析、SWOT、市場區隔與定位、廣告腳本、組員心得）交給 AI 進行結構化解析，並提出了以下關鍵 Prompt 指令：

### 1. 風格與美學設定 Prompt
> **Prompt 示例：**
> 「請將此網頁風格設計成『文青復古風』。色彩搭配請使用沈穩的米色、宣紙紋理、墨色文字與復古紅/墨綠色點綴。字體請使用 Noto Serif TC 與 Noto Sans TC。加入垂直排版元素與細緻的邊框陰影，營造日式鐵道與青春回憶的氛圍。」

### 2. 架構與響應式功能 Prompt
> **Prompt 示例：**
> 「網頁需要具備完整的頂部導覽列（Navbar）、左側側邊欄（Sidebar），以及點擊可切換的分頁內容（Tab system）。必須完整支援 Grid System 與 RWD 響應式功能，確保在手機、平板與桌機上均能完美顯示所有企劃資訊與表格。」

### 3. SEO 與專案結構 Prompt
> **Prompt 示例：**
> 「請在 HTML 頭部加入完整的 SEO Meta 標籤（包含 description、keywords、author 及 Open Graph 社群分享標籤）。同時在說明中清楚指明 CSS 檔案需要切割並放置於 `css/` 資料夾內（如 main.css, layout.css, components.css, retro.css），圖片資源放置於 `images/` 資料夾內。」

---

## 二、 交付的三個指定連結

1. **(1) Prompt 說明 Markdown 檔案（本檔案）：** [GitHub prompts.md 連結](https://github.com/your-username/railway-youth-film/blob/main/prompts.md)
2. **(2) InfinityFree 自有免費網址首頁：** [http://your-infinityfree-site.epizy.com](https://haa.great-site.net/movie/hoh.html)
3. **(3) Vercel 部署後的線上網址：** [https://railway-youth-film.vercel.app](https://12736.vercel.app/)

---
© 2026 這一站，青春 影展專題企劃團隊
