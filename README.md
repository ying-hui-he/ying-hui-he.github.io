# ying-hui-he.github.io

Personal academic website for Yinghui He.

Static single-page site — no build step.

## Structure

```
index.html         Single-page site
asset/
  css/             bootstrap.css, all.css (FontAwesome)
  webfonts/        FontAwesome font files
  image/           Profile photo, publication thumbnails
  pdfs/            CV and other PDFs
```

All styling lives inline in `index.html` under `<style>`. Edit content directly in `index.html`.

## Preview locally

```
python3 -m http.server 8000
```

Then open http://localhost:8000.

## Deploy

Push to `main`. GitHub Pages serves `index.html` from the repo root.
