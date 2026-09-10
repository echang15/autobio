# Autobiography

A personal autobiography, published as a simple static website via GitHub Pages.

## Structure

- `index.html` — homepage / table of contents, linking to each chapter
- `about.html` — a short note about the project
- `chapters/` — one HTML file per chapter (e.g. `01-early-life.html`)
- `chapters/_template.html` — copy this to start a new chapter
- `assets/css/style.css` — all site styling
- `assets/images/` — photos referenced by chapters

No build step, no framework — just plain HTML/CSS, so it's easy to edit by hand and free
to host on GitHub Pages.

## Adding a chapter

1. Copy `chapters/_template.html` to `chapters/NN-short-title.html`.
2. Fill in the title, year range, and body text.
3. Add a row for it in `index.html`'s table of contents.
4. Fix the "previous/next chapter" links at the bottom of the new chapter and its neighbors.

## Publishing (GitHub Pages)

Once this branch is merged into the repo's default branch:

1. Go to the repo's **Settings → Pages**.
2. Under "Build and deployment", set **Source** to "Deploy from a branch".
3. Choose the default branch and the `/ (root)` folder, then **Save**.
4. The site will be published at `https://<username>.github.io/<repo>/`.

Every push to the default branch after that automatically updates the live site.
