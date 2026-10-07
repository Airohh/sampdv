# sampdv.com

Source of [sampdv.com](https://sampdv.com), the portfolio of Sam Pondevie, Data & AI Engineer in Paris
([French version](https://sampdv.com/fr/)).

The whole site is one static page per language, with no framework at runtime:

| File | What it holds |
| --- | --- |
| `public/index.html` | English site: styles, markup and scripts (hybrid search, architecture diagrams, project pages) |
| `public/fr/index.html` | French site, kept in step with the English one |
| `public/img/` | Photo and real figures taken from the project repositories |
| `src/pages/404.astro` | The 404 page; Astro only copies `public/` to `dist/` |
| `wrangler.jsonc` | Cloudflare Workers static assets; a push to `main` deploys |

## Run it

```sh
npm install
npm run dev        # http://localhost:4321
npm run build      # writes dist/
```

Any static server pointed at `public/` works too, for example `python -m http.server 4321 --directory public`.

## Reuse

The **code** is free to reuse under the MIT licence (see `LICENSE`): take the layout, the search, the diagrams.

The **content** is not: the texts, the photo, the name, the project write-ups and the figures describe
Sam Pondevie's own work and stay all rights reserved. Swap them for your own.

Want a site like this built for you? Write to sam.pondevie@gmail.com.

## Credits

Built with [Claude Code](https://claude.com/claude-code). Early design explorations drew on the free prompts
published by [Meez](https://meez.design/free-prompts). Fonts: IBM Plex and Caveat (SIL Open Font License).
