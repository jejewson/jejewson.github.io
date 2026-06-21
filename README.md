# Jack Jewson — Academic Website

A personal academic website built with [Quarto](https://quarto.org/) and hosted on GitHub Pages.

## Local Development

1. [Install Quarto](https://quarto.org/docs/get-started/)
2. Clone this repo and run:

```bash
quarto preview
```

This opens a live preview at `http://localhost:4848` that updates as you edit.

## Editing content

All content lives in `index.qmd`. Edit it like a Markdown file — Quarto renders it to HTML when you preview or publish.

## Deploying to GitHub Pages

### Option A — Automatic (GitHub Actions, recommended)

1. Push this repo to GitHub (e.g. `https://github.com/jackjewson/jackjewson.github.io` or any repo).
2. Go to **Settings → Pages** and set the source to the `gh-pages` branch.
3. Every push to `main` triggers the workflow and redeploys automatically.

### Option B — Manual render

```bash
quarto render          # builds into docs/
```

Then commit and push the `docs/` folder. Set GitHub Pages source to `docs/` on the `main` branch.

## File structure

```
.
├── _quarto.yml          # Site configuration
├── index.qmd            # Main page content
├── styles.css           # Custom styles
├── docs/                # Rendered output (auto-generated)
└── .github/workflows/
    └── publish.yml      # GitHub Actions deployment
```
