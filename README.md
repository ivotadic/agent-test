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
- The H1 heading in `index.md` includes today's date via Jekyll's Liquid `date` filter
  (`{{ "today" | date: "%B %-d, %Y" }}`). This date is computed at each Jekyll build, so it reflects the
  time of the last deploy rather than the visitor's local "today".
- Change the `theme:` value in [`_config.yml`](_config.yml) to another GitHub Pages supported theme, such as
  `jekyll-theme-minimal` or `jekyll-theme-slate`, to change the look of the site.
- Add more `.md` files with front matter (e.g. `about.md`) to create additional pages.

After pushing changes to `main`, check the repository's **Actions** tab for the automatic
"pages build and deployment" workflow run, then visit the published GitHub Pages URL to see the result.
