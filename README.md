# Diarium Local Converter

## HOW TO USE

1. Save or extract the **`index.html`** file to a folder on your Windows PC.
2. Open `index.html` in a modern web browser (such as Google Chrome, Microsoft Edge, or Mozilla Firefox).
3. Keep an internet connection active on the first load so the page can fetch the required SQLite (SQL.js) and DOCX JavaScript libraries from public CDNs.
4. Select a **COPY** of your `.diary` or `.diarium` backup file using drag-and-drop or the file picker.
5. The application will automatically detect the verified database schema, process the .NET timestamps, and display a clean human-readable preview of your entries.
6. Click **Export Clean TXT** or **Export DOCX** to download your converted journal documents.

---

## PRIVACY

* The selected backup is processed entirely inside your browser's local memory.
* The page **never** uploads your diary file or sends its contents to any external server, analytics service, or API.
* Network requests are strictly limited to fetching the required open-source libraries from public CDNs on initial load; those requests never transmit any diary data.

---

## IMPORTANT LIMITATIONS

* This version is specifically optimized and validated for standard Android Diarium manual backup schemas (`Entries` table utilizing `.NET Ticks` for timestamps, `Heading` for titles, and `Text` for body content).
* It extracts and formats text, paragraphs, and bullet points; media files, images, and audio attachments are not included in this text-based export.
* Always keep your original backup file untouched and work exclusively on a backup copy.