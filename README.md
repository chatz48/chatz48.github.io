# Portfolio — Arun Chatha

A single-page portfolio site for GitHub Pages showcasing resume, experience, skills, and projects.

## Contents

- **About** — Short intro and background  
- **Experience** — EFB, Dynium, NVIDIA  
- **Skills** — Languages, ML, data, web, cloud  
- **Projects** — Healthcare app, FPL portfolio optimisation  
- **Education** — Nottingham (MSc CS), Manchester (BA Economics)  
- **Contact** — Email, phone, CV download  

## Run locally

Open `index.html` in a browser, or use a simple server:

```bash
# Python 3
python -m http.server 8000

# Node (npx)
npx serve .
```

Then visit `http://localhost:8000`.

## Deploy to GitHub Pages

1. Create a new repository on GitHub (e.g. `username.github.io` for a user site, or any repo name for a project site). Do **not** add a README or other files when creating it (so the repo is empty).

2. **Open a terminal in this folder** (the one containing `index.html`, not the parent). That way the repo root on GitHub will be your site root (no "Portfolio website" folder on GitHub).

   ```bash
   cd "Portfolio website"
   git init
   git add .
   git commit -m "Initial portfolio"
   git branch -M main
   git remote add origin https://github.com/chatz48/chatz48.github.io
   git push -u origin main
   ```

   Replace `YOUR_USERNAME` and `YOUR_REPO` with your GitHub username and repo name. After this, the GitHub repo will have `index.html`, `styles.css`, `script.js`, `README.md`, and `CV 2026.pdf` at the **root** of the repo.

3. In the repo: **Settings → Pages**:
   - **Source**: Deploy from a branch  
   - **Branch**: `main` (or `master`)  
   - **Folder**: `/ (root)`  
   - Save  

4. After a minute or two, the site will be at:
   - User site: `https://YOUR_USERNAME.github.io`
   - Project site: `https://YOUR_USERNAME.github.io/YOUR_REPO/`

### If using a project site (not username.github.io)

Links and assets are relative, so the site works at any path. The CV link `CV%202026.pdf` will resolve correctly relative to the page URL.

## Customisation

- **Content**: Edit `index.html` (sections, copy, contact).
- **Styling**: Edit `styles.css` (colors in `:root`, layout, typography).
- **CV**: Replace `CV 2026.pdf` with your latest PDF and keep the same filename, or update the `href` in the HTML.

## Licence

Content and design © Arun Chatha. Use the structure for your own portfolio if you like.
