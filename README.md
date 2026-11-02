# Paperlight PDF Editor

Paperlight is a free, browser-based tool for organizing PDF pages. Open a document, arrange the pages, remove the ones you do not need, and download the edited PDF. Files are processed in your browser and are not uploaded to a Paperlight server.

## Why I made this

I saw someone being asked to pay $50 or more just to make a simple edit to a PDF. That felt like too much for a basic document task. I built Paperlight to make common PDF page tools free and available to everyone, and I am sharing the code so people can use it, learn from it, and help improve it.

## Features

- Open one PDF or several PDFs from your device.
- View page thumbnails and hold a page to open a larger preview. The preview button on each page is another way to open it.
- Select pages individually, or use **Shift-click** to select a range.
- Drag pages to rearrange them. When multiple pages are selected, drag to move them together.
- Rotate selected pages, or rotate every page when nothing is selected.
- Duplicate or delete pages. Undo and redo page changes with the toolbar or keyboard shortcuts.
- Turn off repeated delete confirmations with **Don’t ask again**. Deletions can still be undone; choose **Ask before deleting** to restore the confirmation.
- Add selected pages from another PDF, or merge PDFs together. Choose where the added pages go and reorder source PDFs before adding them.
- Extract selected pages into a separate PDF.
- Split the document into one PDF per page, after selected pages, or by page ranges. Split files download together as a ZIP.
- Choose a filename for the edited PDF and switch between light and dark themes.

## Privacy

Paperlight reads and processes the selected PDF in the browser. The PDF contents are kept in browser memory while the editor is open; the app does not send them to a Paperlight server. The app does not require an account. Your browser stores the theme and delete-confirmation preferences, but the app does not save the PDF itself.

Download your edited document before closing or refreshing the tab. Changes are held in memory and are not an automatic backup of the original file.

## Run it locally

You need Node.js and npm installed.

```bash
git clone https://github.com/YOUR-USERNAME/YOUR-REPOSITORY.git
cd YOUR-REPOSITORY
npm install
npm run dev
```

Open the local address printed by Vite in your terminal (usually `http://localhost:5173`). Replace the GitHub username and repository placeholders with your repository details.

## Available commands

```bash
npm run dev      # Start the local development server
npm run build    # Type-check and create a production build in dist/
npm run preview  # Serve the production build locally
```

## How to use it

1. Choose **PDF** on the home screen and select one or more PDF files.
2. Click a page to select it. Use Shift-click to select a range, or drag pages to change their order.
3. Hold a page briefly to see it larger. You can also use the preview icon on its page card.
4. Use the toolbar to rotate, duplicate, delete, extract, add, merge, or split pages.
5. Choose **Download PDF** to create and save the edited document.

Use **Undo** or **Redo** to move through page changes. After enabling **Don’t ask again**, use **Ask before deleting** in the editor to bring back the delete confirmation.

## What this editor changes

Paperlight provides page-level editing: it changes which pages are in a document, their order, and their rotation. It does not currently edit text or images inside a page, add annotations, or provide OCR tools.

Password-protected, damaged, or unusually structured PDFs may not open or export correctly. Very large PDFs can also need substantial browser memory, depending on your device.

## Built with

- React and TypeScript
- Vite
- PDF.js for reading and rendering pages
- pdf-lib for creating edited PDFs
- JSZip for packaging split PDFs
- lucide-react for icons

## Contributing

Suggestions, bug reports, and pull requests are welcome. Please describe the steps to reproduce a bug. Do not include private or confidential PDF documents in an issue; a small sample PDF with non-sensitive content is safer when an example is needed.

## License

There is no `LICENSE` file in this repository yet. Add the license you choose before publishing if you want to give others clear permission to reuse, modify, and share the project.
