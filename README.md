# Lance docs

The public docs for Lance at [docs.lancetrade.xyz](https://docs.lancetrade.xyz): how members trade with a community's bot and in Lance Trade, and how community owners launch their own bot. Built with [Mintlify](https://mintlify.com).

## Layout

| Path | What |
| --- | --- |
| `docs.json` | Site settings: name, colours, navigation, navbar and footer |
| `*.mdx` | Pages. A page shows in the sidebar only once it's listed in `docs.json` |
| `snippets/risk-warning.mdx` | The risk warning that closes every page |
| `style.css` | Extra styles (the risk warning) |
| `images/screens/` | Example screens, from the landing page |
| `logo/`, `favicon.png` | Lance wordmark and icon |

## Preview locally

Needs Node 20 or later.

```bash
pnpm dlx mint dev
```

The site opens at http://localhost:3000. Check links before you push:

```bash
pnpm dlx mint broken-links
```

## Publishing

The Mintlify GitHub app deploys every push to `main` to docs.lancetrade.xyz. Open a pull request for changes and merge it when the preview looks right.

## Writing rules

Read [AGENTS.md](AGENTS.md) before you change copy. Every claim must be true today, and the compliance rules there apply to every page.
