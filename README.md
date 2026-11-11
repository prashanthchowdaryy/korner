# Crafty Korner India – plain Node + HTML/CSS/JS (no dependencies)
Run: `npm start` → http://localhost:3000 · Admin: /admin (password from env `ADMIN_PASSWORD`, default `admin123` – change it!)
Pictures go in `/images`. Content lives in `/data/*.json`. Set your real domain in `data/site.json` ("url") for SEO/sitemap.
Deploy: push to GitHub → connect to Render/Railway (Node, start command `npm start`), add env var ADMIN_PASSWORD, attach a persistent disk for `data` and `images` so admin changes survive redeploys.
