# template-11 — Tailwind Landing Template

A minimal, responsive landing page built with Tailwind CSS (CDN). This repository contains a single-page HTML template suitable for demos, product landing pages, or small marketing sites — themed here as an MCP Server / mindfulness shop UI.

## Stack
- Language: HTML + CSS (Tailwind)
- Framework / runtime: Tailwind CSS (via CDN)
- Notable patterns: single static HTML entry, inline Tailwind configuration for colors/shadows

## Features
- Hero card with call-to-action buttons
- Responsive navigation and layout (mobile-first)
- Category circle items and feature cards
- Lightweight: no build step required — Tailwind loaded from CDN
- Easy theme customization via inline tailwind.config in index.html

## Files
- index.html — main template and single page for the site
- LICENSE — repository license
- .gitignore — typical ignores
- README.md — this file

## Preview / Run locally
The simplest way is to open index.html in your browser. To serve it from a local HTTP server:

Using Python 3 (recommended):
```bash
git clone https://github.com/boulangeriealexandre/template-11.git
cd template-11
python3 -m http.server 8000
# then open http://localhost:8000 in your browser
```

Or with Node (http-server):
```bash
npx http-server -c-1 .
# open http://localhost:8080
```

You can also publish the `main` branch to GitHub Pages from the repo settings.

## Customization
- Colors & theme: edit the inline tailwind.config script near the top of index.html (colors: `ink`, `brand`, and boxShadow `soft`).
- Content: update headings, paragraphs, badges, and emoji icons directly inside index.html.
- Images: replace emoji placeholders with <img> tags or SVGs as needed.
- If you need a build step (to use a tailored Tailwind build), add a package.json + Tailwind CLI and replace the CDN usage.

## Contributing
Feel free to open issues or pull requests. Suggested small improvements:
- Extract styles and assets into subfolders (assets/, css/)
- Replace emoji with accessible SVG icons
- Add a simple build pipeline to purge unused Tailwind classes for production

## License
This repository includes a LICENSE file. See LICENSE for details.

## Questions you might ask next
- How can I add a custom font and ensure it loads fast?
- Where should I place images and icons if I restructure the project into an assets/ folder?
- Can you add a minimal package.json and Tailwind CLI config so we can build a production CSS file?
