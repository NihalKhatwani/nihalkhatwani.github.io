# Personal Website

A lightweight, fast-loading personal site styled after the
[Minimal](https://orderedlist.com/minimal/) theme. Pure HTML + CSS — no build
step, no JavaScript, no external fonts. The whole page is well under 10 KB.

## Edit your info

Everything is in two files:

- **`index.html`** — your content (name, tagline, about, projects, links). Look
  for the `EDIT THESE` comment at the top and the placeholder text throughout.
- **`style.css`** — colors, spacing, layout. You probably don't need to touch
  this.

Optional: add an `avatar.jpg` next to `index.html` and uncomment the `<img class="avatar">`
line in `index.html`.

## Preview locally

Just open `index.html` in your browser. Or serve it:

```bash
python3 -m http.server 8000
# then visit http://localhost:8000
```

## Host on GitHub Pages (free)

1. Create a new repository on GitHub.
   - For a site at `https://<username>.github.io`, name the repo
     **`<username>.github.io`**.
   - For a project site at `https://<username>.github.io/<repo>`, name it
     anything.
2. Push this folder:

   ```bash
   git init
   git add .
   git commit -m "Initial site"
   git branch -M main
   git remote add origin https://github.com/<username>/<repo>.git
   git push -u origin main
   ```

3. On GitHub: **Settings → Pages → Build and deployment → Source: Deploy from a
   branch**, pick **`main`** and **`/ (root)`**, then **Save**.
4. Wait ~1 minute. Your site is live.

The included `.nojekyll` file tells GitHub Pages to serve the files as-is
(faster, no Jekyll processing).
