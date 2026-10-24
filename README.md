# Diarium Local Converter (Obsidian & Text Export)

A privacy-first web utility that converts Diarium SQLite backup files (`.diary` or `.diarium`) into structured, ready-to-use **Obsidian Markdown vaults**, clean text files, or DOCX documents entirely within your browser.

---

## FEATURES

- **Obsidian-Ready ZIP Export:** Automatically packages your journal entries into chronologically sorted `.md` files complete with custom YAML frontmatter.
- **Smart Multi-Entry Grouping:** Intelligently groups multiple entries written on the same calendar day into a single daily note, appending subsequent entries neatly underneath with timestamps.
- **Timezone-Safe Parsing:** Uses robust UTC date components to prevent timezone drift bugs, ensuring late-night or early-morning entries land on the correct calendar date.
- **Dynamic Schema Inspection:** Automatically detects and maps database columns (`Entries`, `Text`, `Heading`, etc.) across different Diarium versions.

---

## HOW TO USE

1. Save or extract the **`index.html`** file to a folder on your Windows PC.
2. Open `index.html` in a modern web browser (such as Google Chrome, Microsoft Edge, or Mozilla Firefox).
3. Keep an internet connection active on the first load so the page can fetch the required SQLite (`SQL.js`), JSZip, and DOCX JavaScript libraries from public CDNs.
4. Select a **COPY** of your `.diary` or `.diarium` backup file using drag-and-drop or the file picker.
5. The application will automatically verify the database schema, process timestamps securely, and display a clean preview of your entries.
6. Click **Export Obsidian Vault (.zip)** to instantly download a ready-to-extract folder for Obsidian, or choose **Export Single TXT** / **Export DOCX** as needed.

---

## PRIVACY

- The selected backup is processed entirely inside your browser's local memory.
- The page **never** uploads your diary file or sends its contents to any external server, analytics service, or API.
- Network requests are strictly limited to fetching the required open-source libraries from public CDNs on initial load; those requests never transmit any diary data.

---

## IMPORTANT LIMITATIONS

- Optimized and validated for standard Diarium manual backup schemas (`Entries` table).
- It extracts and formats text, paragraphs, and bullet points; media files, images, and audio attachments are not included in this text-based export.
- Always keep your original backup file untouched and work exclusively on a backup copy.