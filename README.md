# Personal homepage

A clean, single-page academic-style homepage. Plain HTML + CSS — no build step.

## Files
- `index.html` — content (edit the sections marked `<!-- EDIT: ... -->`)
- `style.css` — styling and light/dark theme tokens
- `profile.jpg` — your photo (add this; a square image works best)
- `cv.pdf` — your CV (add this)

## Preview locally
Just open `index.html` in a browser. Or serve it:

```bash
python3 -m http.server 8000
# then visit http://localhost:8000
```

## Publish on GitHub Pages
Your site will live at `https://<username>.github.io`.

1. Create a repository named **exactly** `<username>.github.io` (using your GitHub username).
2. Push these files to the `main` branch:
   ```bash
   git init
   git add .
   git commit -m "Initial homepage"
   git branch -M main
   git remote add origin https://github.com/<username>/<username>.github.io.git
   git push -u origin main
   ```
3. In the repo: **Settings → Pages → Build and deployment → Source: Deploy from a branch**, branch `main`, folder `/ (root)`.
4. Wait ~1 minute, then visit `https://<username>.github.io`.

## Customize
- Search `index.html` for `EDIT:` to find every spot that needs your info.
- Duplicate a `<li class="pub">` block per publication.
- Colors live in the `:root` (light) and `[data-theme="dark"]` blocks at the top of `style.css`.
