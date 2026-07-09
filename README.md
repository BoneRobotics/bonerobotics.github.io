# Bone — Website Pilot

Static site, ready for GitHub Pages (or any static host).

## Files
- `index.html`   — desktop one-pager (auto-redirects to mobile.html on small screens; add `?desktop` to skip)
- `mobile.html`  — mobile version
- `terms.html`   — Terms of Use
- `privacy.html` — Privacy Policy
- `support.js`   — page runtime (required, keep next to the HTML files)
- `assets/`      — images

## Deploy on GitHub Pages
1. Push this folder's CONTENTS to a repo (files at repo root, or in `/docs`).
2. Repo → Settings → Pages → Source: `main` branch (root or `/docs`).
3. Custom domain (e.g. bonerobotics.ai): add it in Pages settings, then at your DNS
   (Cloudflare) create a CNAME record pointing the domain to `<user>.github.io`.
   In Cloudflare, set SSL mode to "Full" once Pages issues its certificate.

## Known gaps before real launch
- The contact form is a visual mockup — it does not send anything yet.
  Wire it to Formspree/Cloudflare Workers or similar.
- Fonts load from Google Fonts (needs internet).

© 2026 Bone AI Inc.
