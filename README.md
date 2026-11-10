# personal-website

Source for [mattmatt777.github.io/personal-website](https://mattmatt777.github.io/personal-website/), built with Jekyll and the [cvless](https://github.com/piazzai/cvless) theme and hosted on GitHub Pages.

## Editing

- `index.md` is the home page (the About text under the particle banner).
- `cv.md` is the full CV page. It also prints cleanly from the browser.
- `_config.yml` holds your name, tagline, email, the lines under "Contact", and the icon links (LinkedIn, email, CV). Leave `url` and `baseurl` out: GitHub Pages fills them in, so the site works at the github.io address or at a custom domain without changes.
- `_includes/` and `_layouts/default.html` override a few theme files so links work under `/personal-website/` as well as on a custom domain.
- `assets/` holds the favicons.

Every push to `main` rebuilds the site. GitHub Pages should be set to "Deploy from a branch", `main`, `/ (root)`. The theme is loaded with `remote_theme`, which Pages supports natively, so no workflow is needed.

## Preview locally

```sh
bundle install
bundle exec jekyll serve --config _config.yml,_config.dev.yml
```

Then open http://localhost:4000.
