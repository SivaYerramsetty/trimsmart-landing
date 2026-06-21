# TrimSmart — landing page

Static waitlist landing page for **TrimSmart**, a tax-aware "what should I trim, and when"
portfolio analyzer for self-directed investors. This repo exists only to host the marketing /
demand-validation page; the analyzer itself lives in a separate private repo.

## Live site
https://sivayerramsetty.github.io/trimsmart-landing/

## How it works
- `index.html` — self-contained page (inline CSS + JS, no build step). The email waitlist form
  posts to [Formspree](https://formspree.io) endpoint `https://formspree.io/f/xojoarnn` via a
  dependency-free AJAX handler, so the visitor stays on the page and sees a confirmation.
- `.nojekyll` — tells GitHub Pages to serve files as-is (no Jekyll processing).

## Deploy
GitHub Pages is configured to serve from the `main` branch root. Any push to `main` republishes
the site automatically — just commit and push `index.html`.

## Editing
- The product name "TrimSmart" is a placeholder; find-and-replace to rename.
- To change the form destination, update the `<form action=...>` URL in `index.html`.
