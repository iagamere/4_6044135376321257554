# MARGINS — A quieter way to read.
Local-first EPUB/PDF reader (PWA). No backend; books stay in the browser (IndexedDB).

## Deploy on GitHub Pages
1. Create a repo, upload ALL files in this folder to the repo root.
2. Settings > Pages > Deploy from a branch > `main` / root.
3. Open `https://<user>.github.io/<repo>/` (HTTPS required for install/offline).
4. Open once online, then "Install app" / "Add to Home Screen". Offline works after the first load.

## Run locally
`python3 -m http.server 8000` then open http://localhost:8000

## Notes
- EPUB.js, PDF.js, JSZip and fonts are loaded from CDNs on first visit, then cached by the service worker.
- Browser storage can be cleared by the user or browser; there is no sync or backup.
- Highlights/notes: EPUB only. Not yet tested on real devices.
