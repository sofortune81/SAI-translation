# SAI Leisure Group 2025 Annual Report — Chinese Translation

English → Traditional Chinese translation of the **S.A.I. Leisure Group Company Limited
(海天地悅旅集團有限公司, HKEX: 1832)** 2025 Annual Report.

**View it here:** https://sofortune81.github.io/SAI-translation/

## Contents

| File | What it is |
|---|---|
| `index.html` | The page GitHub Pages serves. Holds the wrapper only — charset, Traditional Chinese serif font stack, per-page cards, responsive tables — and no translated text. |
| `chunk1.html`, `chunk2.html`, … | Raw translation fragments as produced by the pipeline — no wrapper, no styling. |

`index.html` stitches the chunks together in the browser: it fetches `chunk1.html`,
`chunk2.html`, … in order and stops at the first one that does not exist. To publish a new
section, add the next `chunkN.html` — numbering must be contiguous, and `index.html` does
not change. The page range in the header is derived from the loaded pages.

Local preview needs a web server (`fetch` is blocked on `file://`):
`python3 -m http.server`, then open http://localhost:8000/.

## Note

Machine-assisted translation, for review purposes only. Where the English and Chinese
versions of the annual report differ, the English version prevails.
