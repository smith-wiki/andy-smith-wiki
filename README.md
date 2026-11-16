# Andy Smith Wiki

The open wiki at [andy.smith.wiki](https://andy.smith.wiki). Being rebuilt; the
previous Card wiki lives at [old.smith.wiki](https://old.smith.wiki).

- `redirects` — one redirect per line, `<from path> <to URL>`. The build writes
  `<from>/index.html` for each (canonical, meta refresh, `location.replace`
  keeping query and fragment). It keeps every old `andy.smith.wiki/<card id>/`
  URL working.
- `static/` — copied to the site as is, including `404.html`.
- `.github/workflows/pages.yml` — builds and deploys to GitHub Pages on every
  push to `main` (custom domain `andy.smith.wiki`, DNS
  `CNAME andy -> smith-wiki.github.io`).
