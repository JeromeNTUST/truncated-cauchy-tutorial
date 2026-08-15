# Truncated Cauchy Jump-Diffusion Tutorial

截斷柯西跳躍擴散模型（Truncated Cauchy Jump-Diffusion, TCJD）互動教學：從對稱截斷 Cauchy 分布出發，一路推導到非對稱模型、市場參數還原，最後落地成可實作的演算法。全篇以中文撰寫，搭配白話說明與逐步微積分推導，適合想搞懂「厚尾又能算動差」這類金融建模技巧的人閱讀。

🔗 線上瀏覽：**[jeromentust.github.io/truncated-cauchy-tutorial](https://jeromentust.github.io/truncated-cauchy-tutorial/)**

## 內容涵蓋

教學分成四個章節（頁面上方分頁可切換）：

1. **打造基礎：對稱截斷 Cauchy 分布** — 定義 TC 分布、推導原始動差、變異數與峰度公式，並證明「形狀（截斷比率 b）與尺度（θ）分離」的關鍵性質。
2. **升級裝備：非對稱截斷 Cauchy 分布** — 從單邊的半截斷 Cauchy（HTC）出發，組合出可以描述市場漲跌不對稱的 ATC 模型，推導其動差公式。
3. **參數還原：從市場數據解碼模型** — 在「等形狀條件」下，把市場的均值、變異數、偏度、峰度反推回模型的 5 個未知參數（p, θ⁺, θ⁻, B⁺, B⁻）。
4. **實戰演算法** — 把前三章的數學推導整理成可執行的虛擬碼（Algorithm 1），說明如何用一維尋根取代原本的高維搜索。

## 技術說明

純靜態單頁網站，只有一個 `index.html`：

- 數學式排版使用 KaTeX/MathJax。
- 四個章節的切換由內建的 `switchTab()` 這段 vanilla JS 控制，沒有其他外部相依或建置流程。
- 直接透過 GitHub Pages 部署（`main` 分支）。

## 參考論文

> 待補：本教學所依據的原始論文（作者、篇名、年份、連結）尚未列出，之後補上。

## License

尚未設定授權條款。
