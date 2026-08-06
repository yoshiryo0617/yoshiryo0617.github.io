# Personal website — Ryo Yoshida

Static single-page site. Edit `index.html` directly.

## Structure

- `index.html` — all content, plus SEO metadata (canonical, OGP/Twitter Card, schema.org `Person` JSON-LD)
- `style.css` — site styles
- `assets/` — images (avatar, etc.)
- `vendor/` — vendored Pico CSS (self-hosted so the page renders without a CDN round-trip)
- `robots.txt`, `sitemap.xml` — crawler hints; bump `<lastmod>` in `sitemap.xml` after substantial updates
- `googleb3aa656ba23a183d.html` — Google Search Console verification

## Local preview

```
open index.html
```

No build step.

## Deploy

GitHub Pages serves the repo root of `main` at <https://yoshiryo0617.github.io/>.

## Updating Pico

```
curl -sSL -o vendor/pico.classless.min.css \
  https://unpkg.com/@picocss/pico@2/css/pico.classless.min.css
```
