# AI米克斯_大屏講義解答html製作（專案藍圖）

> 本檔為跨 Agent 通用的專案藍圖（AGENTS.md 開放標準）。任何 Agent 的每個 session 都應先讀本檔＋`handoff.md`。

## 專案簡介
本專案專門將教師備課教材與講義（包含單字、文法、時態題型等），轉換為兼具「學生端純淨 A4 列印」與「教師端大屏/投影逐題點擊秀答案＋板書多色螢光筆」的雙模式自製電子書（e指書）單一獨立 HTML 檔案。

## 關鍵時程
- 配合日常教學與段考複習進度產出

## 目標與路線圖
- [x] 階段一：完成前 10 頁與時態 P14-18 教師大屏互動版 HTML
- [ ] 階段二：將 `input_example/` 內教材（英文三）轉換為標準大屏互動 HTML 輸出至 `output/`
- [ ] 階段三：依據 `self-made-ebook` 規範持續擴充文法講義其餘章節

## 資料夾結構
```text
AI米克斯_大屏講義解答html製作/
├── AGENTS.md                             # 專案藍圖
├── handoff.md                            # 跨 Agent / 跨電腦交接檔
├── .gitignore                            # Git 忽略設定（GDrive 專用）
├── 2025文法講義_教師大屏版_前10頁.html       # 既有成品：前 10 頁完整全覽
├── 2025文法講義_教師大屏版_時態_P14-18.html  # 既有成品：時態章節 P14-18
├── input_example/                        # 原始教材與參考材料
│   ├── 1150430英文三.pdf
│   ├── 115.04.30 英文三(revised).docx
│   └── 英文三_教師大屏互動解答.html
└── output/                               # 新生成的標準 HTML 講義放置區
```

## 同步層級（本專案初始化至第 3 層級）

| 層級 | 平台 | 位置 | 讀取時機 |
|------|------|------|---------|
| L1 | 本地（GDrive） | `AGENTS.md`＋`handoff.md` | 每個 session |
| L2 | GitHub | `t508-ksvs/aimix-screen-handout-html`（公開，Pages: `https://t508-ksvs.github.io/aimix-screen-handout-html/`） | 指定時 |
| L3 | Obsidian | `Projects/AI米克斯_大屏講義解答html製作/專案工作流程.md` | 有需要時 |

## 工作約定
- 任何 Agent、任何電腦：**開工先讀 `handoff.md`，收工必更新 `handoff.md`**
- 修改共用檔案前先讀最新內容，避免覆蓋其他 Agent 的變更
- 所有回應與文件使用繁體中文
- 產出嚴格遵守 `self-made-ebook` 規範：字體 14pt、Times New Roman + 標楷體、零操作提示干擾文字、單一 HTML 自包含。
- GDrive 上執行 Git 操作須保持 `windows.appendAtomically false` 設定。
