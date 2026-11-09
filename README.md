# Droša izaugsme bankām — website

A static one-page website (plain HTML, CSS and JavaScript). No build step and no framework are needed.

## Files
- `index.html` — the whole site (markup, styles and scripts)
- `package.json` — optional; provides `npm start` for a local preview
- `vercel.json` — Vercel settings (clean URLs, basic security headers)
- `.gitignore`

## Run locally
Option 1: double-click `index.html` to open it in a browser.

Option 2 (local server, needs Node.js):
```
npm start
```
Then open http://localhost:3000

## Deploy: GitHub + Vercel
1. Create a new empty repository on GitHub.
2. In this folder run:
   ```
   git init
   git add .
   git commit -m "Initial commit"
   git branch -M main
   git remote add origin https://github.com/YOUR-USER/YOUR-REPO.git
   git push -u origin main
   ```
3. Go to https://vercel.com/new, import the repository.
4. Framework Preset: **Other**. Leave Build Command and Output Directory empty. Click **Deploy**.

Every later `git push` redeploys the site automatically.

## Notes
- Google Fonts (Newsreader, Public Sans) load from the internet; fallback fonts are defined.
- The contact form opens the visitor's email app with a prepared message to podzinamarta3@gmail.com. It does not need a server.
