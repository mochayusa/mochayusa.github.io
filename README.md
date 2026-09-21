# mochayusa.github.io

Personal website of [@mochayusa](https://github.com/mochayusa), hosted with [GitHub Pages](https://pages.github.com/).

**Live site:** https://mochayusa.github.io

## About this repo

This is a GitHub Pages *user site*. Because the repository is named `<username>.github.io`, GitHub serves whatever is on the default branch (`main`) at `https://<username>.github.io` with no extra configuration.

The site is plain HTML and CSS with no build step:

| File         | Purpose                                             |
| ------------ | --------------------------------------------------- |
| `index.html` | Single-page site: hero, about, projects, contact    |
| `style.css`  | Styles, including automatic light/dark mode         |

Placeholder content is marked with `TODO` comments in `index.html`; search for them to find what to fill in.

## Getting started

1. Clone the repo:

   ```sh
   git clone https://github.com/mochayusa/mochayusa.github.io.git
   cd mochayusa.github.io
   ```

2. Preview locally by serving the folder with any static server, for example:

   ```sh
   python3 -m http.server 8000
   ```

   Then open http://localhost:8000.

3. Edit `index.html` and `style.css`, then commit and push to `main`:

   ```sh
   git add .
   git commit -m "Update site"
   git push origin main
   ```

## Deployment

Pushes to `main` are published automatically by GitHub Pages, usually within a minute or two. If the site doesn't appear, check **Settings → Pages** in the GitHub repo and confirm the source is set to deploy from the `main` branch (root folder).

## Options for building the site

- **Plain HTML/CSS/JS:** no build step; files are served as they are.
- **Jekyll:** GitHub Pages builds Jekyll sites natively, so you can add a `_config.yml`, layouts, and Markdown pages.
- **Other static site generators** (Hugo, Astro, Eleventy, etc.): build the site and deploy the output using a GitHub Actions workflow, then set the Pages source to **GitHub Actions**.

## Custom domain

To use your own domain, add a `CNAME` file at the repo root containing the domain name, and configure DNS as described in the [GitHub Pages docs](https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site).
