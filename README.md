# agent-test

This repository is published as a GitHub Pages site.

## GitHub Pages setup

- **Source:** `Settings -> Pages -> Source -> Deploy from a branch`, set to `main` / `(root)`.
- **Theme:** [`jekyll-theme-cayman`](https://github.com/pages-themes/cayman), one of the themes GitHub Pages
  supports natively, configured in [`_config.yml`](_config.yml).
- **Content:** the home page is [`index.md`](index.md), a Markdown file with Jekyll front matter that Jekyll
  renders using the theme's layout.

## Customizing

- Edit [`index.md`](index.md) to change the page content.
- Change the `theme:` value in [`_config.yml`](_config.yml) to another GitHub Pages supported theme, such as
  `jekyll-theme-minimal` or `jekyll-theme-slate`, to change the look of the site.
- Add more `.md` files with front matter (e.g. `about.md`) to create additional pages.
- The "Showcase" images in `index.md` link directly to specific photos on `images.unsplash.com`. Do **not** use
  Unsplash's old topic-based `source.unsplash.com` redirect endpoint for new images: that service has been
  deprecated and shut down, and now returns `503 Service Unavailable` for every request. Always link to a
  specific photo's `images.unsplash.com/photo-<id>?...` URL (found on the photo's Unsplash page) instead. For
  permanent or licensed images, add files under a new `assets/images` folder and reference them with relative
  paths (e.g. `![Alt text](assets/images/example.jpg)`) instead of any external URL.

After pushing changes to `main`, check the repository's **Actions** tab for the automatic
"pages build and deployment" workflow run, then visit the published GitHub Pages URL to see the result.
