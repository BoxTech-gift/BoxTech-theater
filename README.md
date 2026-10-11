# BoxTech theater — static GitHub Pages site (project, sub-path)

مرآة ثابتة لموقع **بوكس تيك** (كراسي ومسارح وملاعب وقاعات).

Static mirror of https://playground-grandstand.grok.me built for hosting as a GitHub Pages **project site** under the sub-path `/BoxTech-theater/`.

**Live:** https://boxtech-gift.github.io/BoxTech-theater/ (`/BoxTech-theater/` → `/BoxTech-theater/ar/`)

Repo: https://github.com/BoxTech-gift/BoxTech-theater

## Contents

- Arabic (`/ar/…`) and English (`/en/…`) HTML routes from the source sitemap (~1226 pages), each as `…/index.html`
- `assets/*` (JS/CSS), `media/*` (product & project images), favicon, OG images, `.nojekyll`, `404.html` SPA fallback
- TanStack Router `basepath` = `/BoxTech-theater`; Vite asset helper `Mv` returns `/BoxTech-theater/`+e
- Every HTML/CSS/JS/manifest URL is prefixed with `/BoxTech-theater`
- `sitemap.xml` / `robots.txt` use absolute `https://boxtech-gift.github.io/BoxTech-theater/…` URLs

## Gaps / known limits

- This is a **static** export: live server APIs, quote/form backends, or WebSocket features from the original host do not run here.
- Google Fonts load from `fonts.googleapis.com` (requires network).

## History

- Built from theaterstage/BoxTech-seating@fe2c0fc (route chunks restored, asset helper fixed, `media/plates/*.svg` added), with `/BoxTech-seating` → `/BoxTech-theater`.
