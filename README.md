# tamra.dev

The landing page for **[Tamra](https://github.com/tamra-dev/tamra-agent-ledger)** — a
tamper-evident evidence ledger for AI agents. It seals every LLM call, tool call, and human
approval into a cryptographic hash chain you can hand to an auditor, who can verify it offline
without trusting you.

**Live:** https://tamra.dev

## What's here

A single self-contained static page. No build step, no dependencies, no external requests —
all CSS and JS are inline, and the OG image is a plain PNG.

| File | Purpose |
|------|---------|
| `index.html`  | The whole site — light/dark themed, responsive |
| `og.png`      | 1200×630 social preview image |
| `CNAME`       | Custom domain for GitHub Pages (`tamra.dev`) |
| `robots.txt`  | Crawler directives + sitemap pointer |
| `sitemap.xml` | Single-URL sitemap |

## Local preview

No tooling required — open the file directly:

```bash
open index.html
```

Or serve it, if you want a real origin (for testing the theme toggle's `localStorage`):

```bash
python3 -m http.server 8000   # then visit http://localhost:8000
```

## Deploy

Hosted on GitHub Pages from the `main` branch of this repo, served at the custom domain
`tamra.dev` (see `CNAME`). To publish an update, commit and push:

```bash
git add -A && git commit -m "Update site" && git push
```

Pages rebuilds automatically within a minute or two.

## License

Content and code for this page are released under the [Apache License 2.0](https://www.apache.org/licenses/LICENSE-2.0),
matching the Tamra project.
