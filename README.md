# Ignite HR — GitHub Pages

This repo contains a single static page for **Ignite HR**.

## Deploy steps (Project Pages)

1. Create a new repository on GitHub (e.g., `Ignite-HR`) and make it **Public**.
2. Upload the two files from this ZIP to the **repo root**:
   - `index.html` (entry file)
   - `README.md` (this file)
3. Go to **Settings → Pages**:
   - **Source**: *Deploy from a branch*
   - **Branch**: `main` and **Folder**: `/ (root)`
   - Save.
4. Open: `https://<your-username>.github.io/<exact-repo-name>/`

**Important notes**

- The published URL path is **case-sensitive**. If your repo is `Ignite-HR`, use `/Ignite-HR/` in the URL.
- Your entry file **must** be named `index.html` and live at the top-level of the selected publishing source.
- If your repo previously had GitHub Pages configured from a different branch/folder, update the Pages settings or move `index.html` accordingly.
- You don’t need Jekyll for this site. If you ever add directories starting with `_`, add a blank `.nojekyll` file to the root to bypass Jekyll.

## Local preview

Just open `index.html` in any browser (no build required).