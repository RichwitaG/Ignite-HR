# Ignite HR — Static Site Package

This ZIP contains the latest **Ignite HR** landing page and a README with deployment steps.

## What’s included
- `index.html` — your production-ready landing page
- `README-Ignite-HR.md` — this guide

## What changed (this build)
- Removed **floating stats** in hero ("500+" and "24/7" badges)
- Kept **Compliance Fortress** and **HR Tech Stack** **removed**
- Restored the other four solutions: **Talent Architecture, Performance Engineering, Culture Strategy, Leadership Acceleration**
- Footer replaced with: `228 Park Ave S #676725, NY, NY 10003 · 1-800-IGNITE-HR`

---

## Quick deploy to GitHub Pages

### Option A — Publish from repo **root** (recommended)
1. Create a public repo (e.g., `Ignite-HR`).
2. Upload `index.html` to the **top level** of the default branch (usually `main`).
3. In **Settings → Pages**:
   - **Source**: *Deploy from a branch*
   - **Branch**: `main`
   - **Folder**: `/ (root)`
   - Save.
4. Visit: `https://<your-username>.github.io/<Repo-Name>/` (case-sensitive).

### Option B — Publish from `/docs` folder
1. Put `index.html` inside a folder named `docs/` at the root of your repo.
2. In **Settings → Pages**:
   - **Branch**: `main`
   - **Folder**: `/docs`
   - Save.

> If you ever add folders starting with `_`, drop a blank file named `.nojekyll` in the publishing root so Pages doesn’t run Jekyll.

---

## Command-line quick start
```bash
# one-time repo setup
git init
git add index.html README-Ignite-HR.md
git commit -m "Ignite HR landing page"
git branch -M main
git remote add origin https://github.com/<your-username>/Ignite-HR.git
git push -u origin main
# then enable Pages in Settings → Pages as described above
```

---

## (Optional) Custom domain
- Add a **CNAME** record for `www` to `<your-username>.github.io` at your DNS provider.
- For the apex (root) domain, add the 4 A records to GitHub Pages IPs.
- In **Settings → Pages**, set your **Custom domain** and enable **Enforce HTTPS**.

---

## Troubleshooting
- **404**: Ensure `index.html` is located at the selected **root** or **/docs** of the publishing branch.
- **Old content**: Hard refresh or append a querystring (e.g., `?v=2`).
- **Fonts/Assets**: Use absolute HTTPS URLs or repo-relative paths for any external assets.

_Last packaged: 2025-09-30T23:36:11_