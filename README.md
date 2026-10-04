# JEEDS journal website

Static site, no build step. Open `index.html` in a browser or upload the folder to any static host (Netlify, GitHub Pages, Cloudflare Pages).

```
index.html        page shell
css/style.css     all styles (light, dark, print)
js/data.js        journal settings (J), articles (A), figures (FG)
js/app.js         router and pages: home, articles, article, issues, explore, about, authors, resources
js/legal.js       contact page, cookie policy page, cookie notice
js/features.js    live features: World Bank data, OpenAlex literature, Crossref DOI lookup, reading list, citation styles, submission form, RSS
img/              SVG graphics, subject icons, logo, favicon
```

## Edit content
- Add or change articles in `js/data.js`. Each article needs `s` (slug), `t`, `ty`, `d`, `sub`, `kw`, `abs`, plus `body` (full text) or `k` (key points).
- Attach figures by adding them to `FG` in `js/data.js`.
- Publisher, contact, e-ISSN and license details live in `PUB` at the bottom of `js/data.js`.
- Still placeholders: DOIs (10.0000/…), "Editorial Staff", the other board members, publication fees and the sample policies.

## Live data sources (free, no key)
World Bank Open Data, OpenAlex, Crossref. They need an internet connection.
