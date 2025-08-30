# Kissinger Undergraduate Thesis — Explorer

Explore Henry A. Kissinger’s undergraduate thesis — “The Meaning of History: Reflections on Spengler, Toynbee, and Kant” — alongside a generated mindmap, a structured outline, and a concise summary. A polished landing page ties everything together.

- Live site: https://dicklesworthstone.github.io/kissinger_undergraduate_thesis/

## What’s Included
- `index.html`: Landing page using Tailwind (CDN) with quick links to all artifacts and inline SVG icons (no icon font).
- `kissinger_thesis.md`: Improved, authoritative Markdown version of the thesis.
- `kissinger_thesis.html`: Reader that auto-renders `kissinger_thesis.md` client‑side (Tailwind Typography, dark mode, code highlight, inline SVG icons, “Aa” reader controls for font + width).
- `henry_a_kissinger_the_meaning_of_history_reflections_on_spengler_toynbee_and_kant_0aa02530_pdf_mindmap.html`: Mindmap visualization (HTML).
- `henry_a_kissinger_the_meaning_of_history_reflections_on_spengler_toynbee_and_kant_0aa02530_pdf_mindmap_outline.md`: Mindmap-derived outline (Markdown, rendered on GitHub).
- `henry_a_kissinger_the_meaning_of_history_reflections_on_spengler_toynbee_and_kant_0aa02530_pdf_summary.md`: Concise summary (Markdown, rendered on GitHub).
- `assets/`: Self‑hosted social preview images (`og.jpg`, `og.webp`), PWA icons (`android-chrome-*.png`, `apple-touch-icon.png`).
- `site.webmanifest`, `safari-pinned-tab.svg`, `favicon.svg`: App metadata and icons.

## How to Use
- Visit the live site above and use the cards/buttons.
- Thesis (HTML): `kissinger_thesis.html` automatically fetches and renders `kissinger_thesis.md`. Edit the Markdown and refresh the page.
- Reader controls: Click “Aa” in the reader header to adjust font family (Inter/Literata/Newsreader), font size, and reading width. Theme toggle is next to it.
- Markdown resources open on GitHub’s blob pages so they render nicely.

## How the Mindmap and Summary Were Generated
These artifacts were prepared by Jeffrey Emanuel:

- Mindmap and Summary were generated using https://fixmydocuments.com.
- You can also reproduce a similar mindmap locally using the open‑source tool: https://github.com/Dicklesworthstone/mindmap-generator

Quick options:
- Fastest path: Upload the thesis (or any document) to FixMyDocuments and select the Mindmap and Summary options to generate both artifacts in one go.
- Open‑source path: Clone `mindmap-generator`, follow its README to install dependencies, and run it against your source document to export a mindmap (and outline if supported).

## GitHub Pages
This repo is ready for GitHub Pages in either configuration:
- Root mode: Serve from `main` branch, root folder.
- Docs mode: Serve from `main` branch, `/docs` folder.

Included for convenience:
- `.nojekyll` at root and in `docs/` to bypass Jekyll processing.
- `docs/` contains mirrored copies of the landing page, reader, Markdown, and assets so either Pages mode works.

If you edit the landing page or HTML locally and you are using Docs mode, mirror your changes:

```bash
cp -f index.html docs/index.html
cp -f kissinger_thesis.html kissinger_thesis.md docs/
cp -fr assets docs/
cp -f henry_*_pdf_mindmap.html docs/
```

## Local Preview
Because the reader fetches `kissinger_thesis.md`, preview with a local server (to avoid browser file:// fetch restrictions):

```bash
python3 -m http.server 8000
# then open http://localhost:8000/kissinger_thesis.html
```

## Tech Notes
- Tailwind (CDN) + Typography plugin; inline SVG icons (no icon font).
- Reader uses Marked + DOMPurify (via CDN with SRI) and highlight.js.
- Self‑hosted OG image and PWA icons; `site.webmanifest` configured.
- Everything is static; for the reader, use a local server when previewing.

## Context
This repository presents a readable edition of Kissinger’s undergraduate thesis, with additional generated materials (mindmap, outline, summary) to aid exploration and study.
