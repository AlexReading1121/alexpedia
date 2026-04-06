# Alexpedia Wiki Log

## Format

`YYYY-MM-DD HH:mm | action | source | output | note`

## Entries

- 2026-04-06 18:49 | init | llm-wiki.md | `wiki/index.md`, `wiki/log.md` | 初始化圖書館結構
- 2026-04-06 18:56 | ingest | user article input | `wiki/books/2026-04-06-male-mating-strategies.md` | 完成摘要整理並更新索引
- 2026-04-06 19:49 | taxonomy-setup | user request | `wiki/human/*`, `wiki/society/*`, `raw/*` | 建立 Human/Society 分類與 PDF ingest 流程
- 2026-04-06 20:00 | ingest human 1.0 | `raw/human/1.0-philosophy/1.1_The wisdom of life.pdf` | `wiki/human/1.0-philosophy/2026-04-06-the-wisdom-of-life.md` | 完成首篇哲學 PDF 整理並建立該分類索引
- 2026-04-06 20:14 | ingest human 1.0 batch | `raw/human/1.0-philosophy/1.2~1.13` | `wiki/human/1.0-philosophy/2026-04-06-*.md` | 批次完成 12 份 PDF 整理並更新分類索引
- 2026-04-06 20:40 | ingest human 2.0 batch | `raw/human/2.0-psychological/*.pdf` | `wiki/human/2.0-psychological/2026-04-06-*.md` | 批次完成 6 份心理學 PDF 整理並更新總索引
