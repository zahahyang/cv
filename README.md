# Zahah Yang — Senior Brand Designer Portfolio

A bilingual (EN / 中文) personal portfolio site for Zahah Yang.

---

## 📁 檔案結構

```
zahah-yang-portfolio/
├── index.html                              # 主頁面（HTML + CSS + JS 全部包在裡面）
├── README.md                               # 這份文件
├── favicon.svg                             # 主 favicon（向量,現代瀏覽器優先用）
├── favicon-16.png                          # favicon fallback 16×16
├── favicon-32.png                          # favicon fallback 32×32
├── favicon-180.png                         # iOS / iPad 加入主畫面圖示
├── favicon-512.png                         # PWA / 高解析度備份
├── og-image.png                            # 社群分享預覽圖 1200×630 (LinkedIn/FB/Twitter)
├── og-image.svg                            # OG 圖原始向量檔（之後修改用）
└── images/
    ├── skechers-uno-keyvisual.jpg          # Case 01 SKECHERS UNO 主視覺
    ├── geocan-01-about.jpg                 # Case 02 久廣 — About 頁
    ├── geocan-02-logo-construction.jpg     # Case 02 久廣 — Logo 構成輔助線
    ├── geocan-03-color-system.jpg          # Case 02 久廣 — Brand Color 系統
    ├── geocan-04-typography.jpg            # Case 02 久廣 — Typography 規範
    ├── geocan-05-business-cards.jpg        # Case 02 久廣 — 名片系統
    └── geocan-06-website.jpg               # Case 02 久廣 — 網站應用
```

---

## 🚀 快速預覽（本機測試）

### 方法一：直接打開
雙擊 `index.html`，瀏覽器會直接開啟。
⚠️ 注意：某些瀏覽器（如 Chrome）對 `file://` 協議有限制，建議用方法二。

### 方法二：本機伺服器（推薦）

開啟 Terminal，cd 到此資料夾，然後執行其中一行：

**Python 3：**
```bash
python3 -m http.server 8000
```

**Node.js：**
```bash
npx serve .
```

然後在瀏覽器打開 `http://localhost:8000`。

---

## 🌐 部署選項

### 選項 A：GitHub Pages（免費，推薦）

1. 在 GitHub 建立新 repo（建議命名 `zahahyang.github.io` 直接成主站，或 `cv` 之類的子站）
2. 把整個資料夾推上去：
   ```bash
   cd zahah-yang-portfolio
   git init
   git add .
   git commit -m "Initial portfolio site"
   git remote add origin <你的 repo url>
   git push -u origin main
   ```
3. 到 repo Settings → Pages → 啟用 GitHub Pages（source: main branch）
4. 等幾分鐘後可在 `https://<your-username>.github.io/<repo-name>/` 訪問

### 選項 B：Netlify / Vercel（免費，更快）

1. 註冊 [Netlify](https://netlify.com) 或 [Vercel](https://vercel.com)
2. 把資料夾拖到 Netlify Drop 區，或用 GitHub 連動部署
3. 自動取得一個 URL，可以接自訂網域

### 選項 C：自己有的網域空間
直接 FTP 上傳整個資料夾即可。

---

## ✏️ 之後如何修改內容

### 修改文字（中英文）
打開 `index.html`，搜尋你要改的中文或英文，直接改即可。
中英文成對使用 `data-lang-en` 與 `data-lang-zh` 標籤，**兩個都要改**才對應一致。

### 修改圖片
直接替換 `images/` 資料夾下的檔案（保留原檔名最快），或在 HTML 中改 `<img src="...">` 路徑。

### 修改顏色 / 字體
打開 `index.html`，在 `<style>` 區塊頂部找 `:root { ... }`，所有顏色與字體變數都集中在這裡。

---

## 📝 內容架構

### 第一螢幕（Hero）
- 名字、職稱、定位
- 跨產業 B2B 翻譯者敘事

### Cases 三個案例（依證據強度排序）
1. **Case 01 — SKECHERS UNO**
   - 主視覺：UNO 城市漫遊 KV
   - **Live Site 連結**：https://zahahyang.github.io/visual_portfolios/portfolio/onepage/uno/index.html
2. **Case 02 — 久廣 Geocan**
   - 6 張 Brand Guideline lightbox gallery
3. **Case 03 — 騰雲 Skycloud**
   - 區塊鏈金融平台 Design System

### Awards
- ShowDaily 醫療展年度專刊 NT$1M+ 廣告業績
- 2021 經濟日報傑出員工獎

### Experience timeline + Skills + Education + Contact

---

## ⚠️ 重要提醒（CV 同步事項）

你之前已經同意但還沒動手執行 CV 修改：

### 🇬🇧 English CV — Skycloud（騰雲）section
**Find this line:**
> Concurrently led VIS rebuilding for two subsidiary companies under the parent group

**Change to:**
> Led VIS rebuilding for two subsidiary companies under the parent group — Skycloud first, with **GoEasy Tech subsequently brought into the visual system**

### 🇹🇼 中文 CV — 騰雲段
**找這一行：**
> 同步操盤騰雲運算與高易科技兩家集團子公司的企業識別系統重塑

**改成：**
> 先後操盤騰雲運算與高易科技兩家集團子公司的企業識別系統重塑 — 騰雲為起點，**高易科技後續納入既有視覺系統**

---

## 🎯 還沒做的待辦事項（之後可補）

- [ ] Case 03 騰雲補圖（如果未來有想法）
- [ ] 個人專業照（Hero 區）
- [x] ~~CV 修改: Concurrently → Sequentially~~ ✅ 已完成
- [x] ~~favicon~~ ✅ 已完成 (Z 字母標)
- [x] ~~og:image meta tag~~ ✅ 已完成 (數字優先設計 1200×630)

---

## 🔧 部署後需要更新 OG 圖的情況

OG 圖上目前寫的是 `zahahyang.github.io`。如果你之後改用其他網域(例如買了 zahahyang.com),需要更新:

1. 編輯 `og-image.svg`,把 `zahahyang.github.io` 改成新網域
2. 重新轉成 PNG（指令：`cairosvg og-image.svg -o og-image.png --output-width 1200 --output-height 630`）
3. 同時改 `index.html` `<head>` 中 `og:image` 標籤的 URL（要寫絕對路徑,例如 `https://zahahyang.com/og-image.png`）

---

## 🛠 技術細節

- 純 HTML / CSS / Vanilla JavaScript（無框架，無建構步驟）
- 中英文切換用 `localStorage` 記憶使用者偏好
- 響應式設計：桌機 / 手機通吃
- 鍵盤無障礙：Lightbox 支援 ESC / 左右鍵
- 字體：Inter + Fraunces（英文）, Noto Sans TC + Noto Serif TC（中文）— 由 Google Fonts CDN 載入

---

## 📞 Contact

- Email: sarah20120829@gmail.com
- LinkedIn: linkedin.com/in/zahahyang
- Cake: cake.me/zahahyang_zht

---

Last updated: 2026-05-05
