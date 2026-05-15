# gpaschalidis.github.io

Personal academic website of **Georgios Paschalidis** — ELLIS PhD student at the
University of Amsterdam Computer Vision Lab.

🔗 **Live:** https://gpaschalidis.github.io/

## Stack

Static site, no build step. Hosted on GitHub Pages.

- `index.html` — markup and inline scripts (theme toggle, mobile nav, scroll-spy, abstract/bibtex toggle)
- `styles.css` — design tokens, responsive layout, light/dark themes
- `george.jpg` — profile photo
- `<paper>/` — per-publication teaser assets (`lexis/`, `rhino/`, `sdfit/`, `cwgrasp/`)

## Features

- Mobile-first responsive layout (phone → tablet → desktop)
- Automatic dark mode (`prefers-color-scheme`) with a manual, persisted toggle
- Open Graph / Twitter card metadata and an inline SVG favicon
- Accessible: skip link, focus-visible styles, ARIA labels, `prefers-reduced-motion`

## Local preview

```bash
python3 -m http.server 8000
# open http://localhost:8000
```

## Adding a publication

Copy a `<article class="publication">` block in `index.html`, then update the
teaser image, title, venue, authors, and the badge links. The Abstract/Bibtex
panels use matching `data-index` values within the same `.links` container.
