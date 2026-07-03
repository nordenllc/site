# Norden — website

A small, static, dependency-free website for Norden. Three pages:

- `index.html` — home
- `masora.html` — the Masora white paper
- `atlas.html` — the Arlington Commercial Vitality Atlas project
- `style.css` — one shared stylesheet

No build step, no frameworks, no external fonts or scripts. It loads instantly and works offline. Open any `.html` file directly in a browser to preview.

## Deploy on GitHub Pages

1. Create a repository (e.g. `norden-site`) and add these files at the repository **root**.
2. Push to the `main` branch.
3. In the repo, go to **Settings → Pages**.
4. Under **Build and deployment**, set **Source** to *Deploy from a branch*, pick `main` and the `/ (root)` folder, and save.
5. Your site publishes at `https://<user-or-org>.github.io/<repo>/` within a minute or two.

For a custom domain (e.g. `norden.llc`), add it under Settings → Pages → Custom domain and create the matching DNS record with your registrar. GitHub will provision HTTPS automatically.

## Editing

Everything is hand-editable HTML. To change a color or spacing globally, edit the variables at the top of `style.css` (`:root { --paper … --accent … }`). The "record" blocks on the Masora and Atlas pages are plain monospaced text inside `<div class="record">` — edit them like text; alignment is by spaces.

Update the `This page last modified` line in each footer when you change a page.
