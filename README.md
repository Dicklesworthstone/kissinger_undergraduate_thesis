# Kissinger Undergraduate Thesis — Explorer

Explore Henry A. Kissinger’s undergraduate thesis — “The Meaning of History: Reflections on Spengler, Toynbee, and Kant” — alongside a generated mindmap, a structured outline, and a concise summary. A polished landing page ties everything together.

- Live site: https://dicklesworthstone.github.io/kissinger_undergraduate_thesis/

## What’s Included
- `index.html`: Landing page using Tailwind (CDN) with quick links to all artifacts.
- `henry_a_kissinger_the_meaning_of_history_reflections_on_spengler_toynbee_and_kant_0aa02530_pdf_optimized.html`: Readable HTML version of the thesis.
- `henry_a_kissinger_the_meaning_of_history_reflections_on_spengler_toynbee_and_kant_0aa02530_pdf_mindmap.html`: Mindmap visualization (HTML).
- `henry_a_kissinger_the_meaning_of_history_reflections_on_spengler_toynbee_and_kant_0aa02530_pdf_mindmap_outline.md`: Mindmap-derived outline (Markdown, rendered on GitHub).
- `henry_a_kissinger_the_meaning_of_history_reflections_on_spengler_toynbee_and_kant_0aa02530_pdf_optimized.md`: Thesis text as Markdown (rendered on GitHub).
- `henry_a_kissinger_the_meaning_of_history_reflections_on_spengler_toynbee_and_kant_0aa02530_pdf_summary.md`: Concise summary (Markdown, rendered on GitHub).

## How to Use
- Visit the live site above and use the cards/buttons to open each resource.
- HTML resources open directly in your browser.
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
- `docs/` contains a mirrored copy of the landing page and HTML artifacts so either Pages mode works.

If you edit the landing page or HTML locally and you are using Docs mode, mirror your changes:

```bash
cp -f index.html docs/index.html
cp -f henry_*_pdf_optimized.html docs/
cp -f henry_*_pdf_mindmap.html docs/
```

## Tech Notes
- Tailwind and Font Awesome are loaded from CDNs; no build step is required.
- Everything is static — open `index.html` locally or host via Pages.

## Context
This repository presents a readable edition of Kissinger’s undergraduate thesis, with additional generated materials (mindmap, outline, summary) to aid exploration and study.
