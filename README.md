# DWCI Storefront — Landing Page

Static landing/funnel page for **David Woldt Consulting** asset packs. Sells the
Wave-1 product set (built in the private `dwci-asset-packs` repo) and captures
free-template leads via MailerLite. Deployed as a Render static site.

## What it contains
- `index.html` — single-page storefront (hero, 3 tiers, free-template capture, footer)
- `assets/` — 1280×720 listing preview images (Evergreen & Brass)

## Two things to wire before go-live
1. **Lemon Squeezy checkout URLs** — edit the `CHECKOUT` object near the bottom of
   `index.html` (`flagship` = $297 Starter Kit, `propack` = $79 RACI Pro Pack).
   Buttons stay disabled until a URL is filled in.
2. **MailerLite form** — paste your embedded-form snippet into the
   `<div id="mailerlite-form">` block in `index.html`, replacing the placeholder
   fallback form.

Commit either change and Render auto-deploys.

## Deploy
Render static site (DWCI workspace) · publish path `.` · no build step.
