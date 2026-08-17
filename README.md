# mdrinsights.com

Static site, no build step. Four pages sharing one stylesheet:

- `index.html` — home
- `what-we-do.html`
- `how-it-works.html`
- `contact.html`
- `styles.css` — shared by all four pages

## Deploying

This repo is connected to Cloudflare Pages. Every push to `main` triggers an
automatic rebuild and deploy — no manual upload step needed.

**Build settings in Cloudflare Pages:** none required. Framework preset:
`None`. Build command: (leave blank). Output directory: `/`.

## Making changes

1. Edit the relevant `.html` file or `styles.css`.
2. Commit and push to `main`.
3. Cloudflare Pages picks it up automatically — check the Cloudflare
   dashboard's "Deployments" tab for build status, usually live within a
   minute or two.

Since all four pages pull from the same `styles.css`, a single color or
type change updates every page at once — no need to edit each file.
