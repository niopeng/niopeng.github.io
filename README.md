# niopeng.github.io

Personal website for Shichong (Nio) Peng — a single static page, no build step.

Served by GitHub Pages from the `master` branch root. `.nojekyll` tells Pages to
serve the files as-is (no Jekyll build).

## How to update

Everything lives in [`index.html`](index.html). Near the bottom of the file, in the
`<script>` block, are two lists:

- **`NEWS`** — newest first. Add one line: `["Mon YYYY", \`your update\`],`
- **`PUBS`** — newest first. Add one object with `title`, `authors`, `venue`,
  optional `badge` (e.g. `"Spotlight"`), optional `thumb` (image path), and
  `links` (`[["Paper","https://…"], …]`). Your name auto-bolds; a paper with no
  `thumb` shows a clean placeholder.

Paper thumbnails go in `assets/img/papers/`. Any aspect ratio is fine — they
display at a fixed width and their natural height (no cropping).

Then commit and push:

```
git add -A && git commit -m "update" && git push
```

The change is live in a minute or two.
