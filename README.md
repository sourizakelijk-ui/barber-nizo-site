# Barber Nizo

Single-file website for Barber Nizo (Phoenixstraat 81, 9000 Gent).

Everything — markup, styles, all images (embedded as base64), and the React app —
lives in one self-contained [`index.html`](index.html). There is no build step:
open the file in any browser, or deploy the folder to any static host.

## Deploy (Netlify)

No build command and no publish subdirectory are needed — `index.html` sits at the
repo root. See [`netlify.toml`](netlify.toml). Connect this repo in the Netlify
dashboard (Add new site → Import an existing project → GitHub → this repo) and it
deploys as-is; every push to `main` redeploys automatically.

## Notes

- Images are embedded directly in the HTML (no external image links).
- React 18.3 + Babel run in the browser via CDN.
- The booking calendar (Cal.com) and Google Fonts are the only external services.
