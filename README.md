# Menu PDF to HTML

Converts a restaurant menu PDF (with photos) into one self-contained HTML file that works offline.

## Files
- `index.html` – the converter
- `pdf.min.js`, `pdf.worker.min.js` – PDF reader (pdf.js 3.11.174, Apache-2.0)

## Deploy on GitHub Pages
1. Create a repository and upload these three files to the root.
2. Settings → Pages → Source: "Deploy from a branch" → Branch: `main`, folder `/ (root)` → Save.
3. After a minute the converter is live at `https://<username>.github.io/<repo>/`.

## Hosting a converted menu with a fixed link
Upload the downloaded menu file (e.g. `menu.html`) to the same repo.
Its link is `https://<username>.github.io/<repo>/menu.html`.
To update the menu later, replace the file with one of the **same name** – the link and any QR codes keep working.
