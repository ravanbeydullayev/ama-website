# AMA Website — Deployment V3

This package fixes the static-site routing and language-switching structure for Cloudflare Pages.

## Entry pages
- Azerbaijani: `index.html`
- English: `en/home.html`

## Board navigation
The “İdarə Heyəti” / “Board of Directors” navigation item opens the dedicated page: `board.html` (AZ) or `en/board.html` (EN). The page contains the founding team and the separate Board of Directors group. It does **not** redirect to a homepage anchor.

## Language switching
Language controls use absolute site-root paths, so selecting English from an English page cannot create repeated `/en/en/` segments. Each paired page switches to its counterpart.

## Deploy to Cloudflare Pages
1. Open the GitHub repository `ravanbeydullayev/ama-website`.
2. Upload **the contents of this folder** to the repository root (not the outer folder itself).
3. Commit the changes to `main`.
4. In Cloudflare Pages, keep Framework preset `None`, Build command blank, Build output directory `.` and Root directory `/`.
5. Wait for the automatic deployment, then test `index.html`, the EN switch, each menu link, and the Board page.

## Important
This is a static HTML site. Authentication, payments, forms, uploads, and member dashboard data still need backend integration. The Cookie Policy is a draft pending legal review.
