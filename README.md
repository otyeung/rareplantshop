# Rare Plant Shop

A simple static website for a rare plant shop, built with [Mobirise](https://mobirise.com/) and published with GitHub Pages.

## Live site

The site is published to two hosts:

| Host | URL |
| --- | --- |
| Vercel | https://rareplantshop.vercel.app |
| GitHub Pages | https://otyeung.github.io/rareplantshop/ |

## Contents

| Path | Description |
| --- | --- |
| `index.html` | Home page of the site |
| `assets/` | Bootstrap, theme, images, fonts and other static assets |

## Running locally

Clone the repository and serve the folder with any static web server:

```bash
git clone https://github.com/otyeung/rareplantshop.git
cd rareplantshop
python3 -m http.server 8000
```

Then open http://localhost:8000 in your browser.

## Deployment

Both hosts deploy automatically from the `main` branch:

- **Vercel** — the repository is connected as a Vercel Git integration. Pushes to `main` publish to production; pushes to other branches create preview deployments. The site is served statically from the repository root (no build step). `.vercelignore` keeps the Mobirise editor project file out of the deployment bundle.
- **GitHub Pages** — served from the `main` branch root folder. `.nojekyll` makes Pages publish the files as-is instead of processing them with Jekyll.

To deploy to Vercel manually:

```bash
vercel deploy --prod
```

## License

Licensed under the [Apache License 2.0](LICENSE).
