# thegoodcitizen.sg

The Good Citizen wedding photography website — static site for https://www.thegoodcitizen.sg.

## Structure

- `index.html` — the whole site (single-page app: Home, About, Weddings,
  Pre-Wedding, Family Time Capsule, Pricing, Kind Words, Contact, Apps,
  Golden Hour)
- `assets/` — photos and artwork
- `s/` — support PDFs (`TWB-Support.pdf`, `Bible555-Support.pdf`)
- `app-ads.txt` — AdMob verification file (must stay byte-identical)
- `_redirects` — Cloudflare Pages rules: real files first, then the SPA
  fallback (`/* /index.html 200`)

## Deploy

Cloudflare Pages, project connected to this repo (branch `main`). Test
address first, then thegoodcitizen.sg.

## Contact form

The form posts to a Google Apps Script backend ("The Good Citizen -
Website Enquiry Form") which files enquiries into the Wedding / Family
Enquiries sheets and emails hello@thegoodcitizen.sg.

## Source

Built from the Muse draft-website artifact (export 2026-11-11); images
extracted from the single-file export into `assets/`.
