# Alexpedia Ingest Guide

這份文件定義 PDF 上傳、整理、發布的標準流程。

## Topic Mapping

- `human/1.0-philosophy`
- `human/2.0-psychological`
- `human/3.0-male-female`
- `society/4.0-finance`
- `society/5.0-business`
- `society/6.0-technology`

## Step 1: 放置 PDF（raw）

把原始 PDF 放到對應的 `raw/` 子資料夾：

- `raw/human/1.0-philosophy/`
- `raw/human/2.0-psychological/`
- `raw/human/3.0-male-female/`
- `raw/society/4.0-finance/`
- `raw/society/5.0-business/`
- `raw/society/6.0-technology/`

建議檔名格式：

`YYYY-MM-DD-source-topic-keyword.pdf`

## Step 2: ingest 指令格式

你可以用這些口令啟動流程：

- `ingest human 1.0`
- `ingest human 2.0`
- `ingest human 3.0`
- `ingest society 4.0`
- `ingest society 5.0`
- `ingest society 6.0`

## Step 3: 產出 wiki 文章

每份 PDF 產生一篇 Markdown，放在對應的 `wiki/` 子資料夾，例如：

- `wiki/human/1.0-philosophy/2026-04-06-stoicism-notes.md`
- `wiki/society/4.0-finance/2026-04-06-etf-basics.md`

文章中要包含：

1. Metadata（日期、來源 PDF、主題、tags）
2. 摘要
3. 重點整理（分段）
4. 可行動結論
5. 原始 PDF 連結

## Step 4: 讓 PDF 可點擊閱讀/下載

在文章中加入相對連結（Quartz 會生成可點擊連結）：

- 同層範例：
  - `[下載原始 PDF](../../../raw/human/1.0-philosophy/2026-04-06-source.pdf)`
- 或使用絕對網站路徑（部署後）：
  - `/alexpedia/raw/human/1.0-philosophy/2026-04-06-source.pdf`

建議優先使用相對路徑，移動網站根路徑時較不易壞連結。
