# Exorcise the Plant

A browser arcade game: play as Muse, dodge hazards, collect warding seals,
and exorcise the possessed snake plant. Single self-contained HTML file, no
build step, no dependencies.

## What's in this repo

- `index.html` — the entire game (HTML, CSS, and JS inlined)
- `render.yaml` — Render Blueprint for one-click static site deploy
- `.gitignore` — standard ignores

## Push to GitHub

```bash
cd exorcise-the-plant-site
git init
git add .
git commit -m "Initial commit: Exorcise the Plant"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/exorcise-the-plant.git
git push -u origin main
```

(Create the empty repo at https://github.com/new first.)

## Deploy on Render

**Option A — Blueprint (recommended):** In the Render dashboard, click
**New > Blueprint**, connect the repo, and Render will read `render.yaml`
and create the static site automatically.

**Option B — Manual static site:** Click **New > Static Site**, connect the
repo, and use these settings:

- **Build Command:** *(leave empty)*
- **Publish Directory:** `./`

Then hit **Deploy**. You'll get a public URL like
`https://exorcise-the-plant.onrender.com`.

## Notes

- The game is fully client-side; there is nothing to build and no server
  code, so the free Render static site tier works fine.
- Every `git push` to `main` auto-redeploys on Render.
