# Contact Sheet

A single-page camera tool: take pictures one at a time, keep or retake each one,
then save them as one combined PDF — for attaching to a file-upload form (e.g. a
Canvas assignment) that only accepts a single PDF.

Runs entirely client-side (camera capture + PDF assembly via [jsPDF](https://github.com/parallax/jsPDF),
vendored in `libs/`). Nothing is uploaded anywhere; the finished PDF is saved to
your device's normal downloads location, and you attach it yourself wherever it's needed.

## Enabling GitHub Pages for this repo

1. Push this repo to GitHub (`git remote add origin <your-repo-url>`, then `git push -u origin main`).
2. On GitHub: **Settings → Pages**.
3. Under **Build and deployment → Source**, choose **Deploy from a branch**.
4. Branch: `main`, folder: `/ (root)`. Save.
5. After a minute or two, the page is live at:
   `https://<your-username>.github.io/<repo-name>/`

## Local testing

Camera access requires a secure context. Opening `index.html` directly as a
`file://` URL works in Chrome/Edge for local testing; on the published GitHub
Pages URL it works normally since that's served over HTTPS.
