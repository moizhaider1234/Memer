# $MEMER website

Single-file static site: `index.html` (HTML/CSS/JS all inline, no build step, no frameworks).

## Adding your images

The site expects two files in an `images/` folder next to `index.html`:

```
images/
  logo.png    ← the smiley-face logo (square, transparent or green background, 256x256+ recommended)
  cover.jpg   ← the "MEMER" crowd illustration (wide, used as a faint hero background)
```

Just drop your two uploaded images into that folder with those exact filenames (or edit the `src`/`url(...)` paths in `index.html` — search for `images/logo.png` and `images/cover.jpg`, there are a few references of each) and everything lights up automatically. No base64, no external hosting needed — GitHub Pages / Vercel / Netlify will all serve them as static assets.

## Editing content

Everything lives in `index.html`:
- Contract address: appears in 3 places (hero badge, buy/dexscreener/solscan links, footer) — search for `Ct4UqNTR5zfMGbMH68NeNeAB4cuFznX6ikHd88PXpump` and replace all if it ever migrates.
- Social links: `https://twitter.com` and `https://t.me` placeholders in the Community section and footer — swap in your real handles.
- Copy: all section text is plain HTML, easy to find and edit near the matching `<section id="...">`.

## Deploying (GitHub Pages)

1. Push `index.html`, `README.md`, and your `images/` folder to the repo.
2. Repo Settings → Pages → Source: deploy from branch → `main` / root.
3. Site goes live at `https://<username>.github.io/<repo>/`.

No build step required — it's a static file.
