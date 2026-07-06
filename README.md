# Excel Combiner Pro

A single-page browser tool that merges multiple Excel (`.xlsx`/`.xls`) and CSV files into one unified spreadsheet. No server, no install, no dependencies — just open the HTML file and go.

## Features

- **Drag & drop file upload** — drop files anywhere in the app area, or use the file picker
- **CSV + Excel support** — handles `.xlsx`, `.xls`, and `.csv` files
- **File reordering** — drag files to change their order (important for append mode)
- **Two merge modes:**
  - **Row-by-Row** — interleaves rows from each file by longest length
  - **Append** — concatenates all rows sequentially
- **Column conflict resolution** — when multiple files share the same column name, choose which source to keep or keep all with prefixes
- **Auto-resolve** — set a default conflict strategy (first file, last file, keep all) to skip manual prompts
- **Column ordering** — drag columns or use ▲/▼ buttons to rearrange output columns
- **Live preview** — see merged results before downloading (simple table or Excel-like grid view)
- **Light/dark theme** — toggle with persistent preference via `localStorage`
- **Responsive** — works on desktop and mobile screens
- **Processing indicator** — button shows loading state during file generation

## How to Use

1. Open `excel_combiner_pro.html` in any modern browser
2. Upload files via the **+ Tambah Fail** button or drag-and-drop
3. Configure merge mode, preview rows, and output name in settings
4. Resolve any column conflicts (or let auto-resolve handle it)
5. Reorder columns if needed
6. Preview the merged data
7. Click **Muat Turun Excel** to download the combined `.xlsx` file

## Tech

- Vanilla JavaScript (no framework)
- [SheetJS (xlsx)](https://sheetjs.com/) — Excel file parsing and generation
- Plus Jakarta Sans via Google Fonts
- Lucide-style SVG icons

## License

MIT
