# romainboces.com

Corporate landing page for **Romain Boces Solution Inc.** — deployed at [romainboces.com](https://romainboces.com).

Static HTML/CSS/JS. No build step. Served via GitHub Pages.

## Structure

```
├── index.html        # Landing page (inline CSS + i18n JS)
├── 404.html          # Not-found page
├── CNAME             # GitHub Pages custom domain
├── .nojekyll         # Prevents Jekyll processing
├── robots.txt        # Search engine crawl rules
├── sitemap.xml       # SEO sitemap (en, fr)
├── llms.txt          # AI-readable company description
├── favicon.svg       # Primary SVG favicon (RB monogram)
├── lang/
│   ├── en.json       # English translations
│   └── fr.json       # French translations
├── README.md         # This file
└── DEPLOY.md         # Deployment and DNS notes
```

## Local preview

```bash
python3 -m http.server 8000
# then open http://localhost:8000/
```

## Languages

English (default) and French. Switch at runtime via the nav dropdown; persisted in `localStorage` and the `?lang=` URL param.

## Follow-ups

- Generate `favicon.ico`, `favicon-16x16.png`, `favicon-32x32.png`, and `apple-touch-icon.png` from `favicon.svg` (e.g. via [favicon.io](https://favicon.io)) and drop them in the repo root — the `<link>` tags are already wired.
