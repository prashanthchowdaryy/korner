# Crafty Korner India – plain Node + HTML/CSS/JS (no dependencies)
Run: `npm start` → http://localhost:3000 · Admin: /admin (password from env `ADMIN_PASSWORD`, default `admin123` – change it!)
Pictures go in `/images`. Content lives in `/data/*.json`. Set your real domain in `data/site.json` ("url") for SEO/sitemap.
Deploy: push to GitHub → connect to Render/Railway (Node, start command `npm start`), add env var ADMIN_PASSWORD, attach a persistent disk for `data` and `images` so admin changes survive redeploys.

**Photo uploads (Cloudinary):** create a free Cloudinary account, copy the API environment variable from the dashboard (looks like `cloudinary://API_KEY:API_SECRET@CLOUD_NAME`) and add it as env var `CLOUDINARY_URL` on Render. Admin uploads then go to Cloudinary and the site uses the returned link, so photos survive redeploys. Without it, uploads are saved to `/images` on the server.
