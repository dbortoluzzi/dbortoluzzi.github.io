# dbortoluzzi.github.io

Personal site built with **[Hugo](https://gohugo.io/)** and the **[hugo-profile](https://github.com/gurusabarish/hugo-profile)** theme (Go module in `go.mod`), deployed to **GitHub Pages** via Actions.

**Layout:** `hugo.yaml` holds all copy and settings; `layouts/partials/` overrides theme partials; `static/` holds assets (e.g. CV under `static/cv/`).

## Commands

```bash
hugo mod get          # fetch theme module
hugo server -D        # local dev → http://localhost:1313
hugo --minify         # production build → public/
```

## Deploy

Pushing to **`main`** runs `.github/workflows/main.yml`: Hugo build, output pushed to **`gh-pages`**. Work on **`devel`** (or a feature branch), then merge into `main` when you want the site updated.

## License

See `LICENSE`.
