# Hosting on GitHub Pages

This repository contains a single-page site (`index.html`) suitable for hosting with GitHub Pages.

## Quick steps (recommended)

1. Create a GitHub repository (for example `mycollege-site`).
2. From your project folder (PowerShell):

```powershell
git init
git add .
git commit -m "Initial commit"
git branch -M main
# replace <username> and <repo> with your values:
git remote add origin https://github.com/<username>/<repo>.git
git push -u origin main
```

3. Go to your repository on GitHub -> Settings -> Pages.
   - Under "Source" choose the `main` branch and the `/ (root)` folder. Click Save.
   - After a minute or two your site will be available at `https://<username>.github.io/<repo>/` (for a project page) or at `https://<username>.github.io/` if you used a repo named `<username>.github.io`.

## Notes & tips

- Keep `index.html` at the repository root — GitHub Pages serves `index.html` from the selected branch root.
- If you reference images (e.g., `images5.jpg`), ensure they are committed in the repo with the same relative paths. For example, keep images in the repo root or an `images/` folder and update paths accordingly.
 - This repo now includes lightweight placeholder SVG images in an `images/` folder (`img1.svg`..`img4.svg`) and `favicon.svg` so the gallery displays out-of-the-box. Commit and push them along with `index.html`.
- If you want a personal site (no `/repo/` path), name the repository exactly `<username>.github.io` and push to the `main` branch root.
- If you have a custom domain, add a `CNAME` file with the domain name (one line) to the repo root and configure DNS as documented by GitHub.

If you want, I can:
- Add a sample `images/` folder with placeholder images.
- Create a GitHub Actions workflow to automatically deploy (not needed for Pages but possible for advanced flows).
- Walk you through the exact Settings clicks with screenshots.
