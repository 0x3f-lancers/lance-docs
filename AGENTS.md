# Lance docs: notes for writers and coding agents

Public Mintlify docs for Lance, at docs.lancetrade.xyz. Pages are MDX with YAML frontmatter; settings live in `docs.json`. Preview with `pnpm dlx mint dev` and check links with `pnpm dlx mint broken-links` before pushing.

## Audience

- **Members**: traders using a community's bot in Telegram and Lance Trade.
- **Community owners**: people who run a branded Lance bot.

These docs are public. Don't document internals: hosting, environment variables, API routes, database details, the admin bot, partner accounting or anything from the private `lance-bot` repo's `docs/` folder.

## Source of truth

Every claim must match the product today. Facts come from the private `0x3f-lancers/lance-bot` repo: `apps/bot/README.md`, `apps/trade/README.md`, `apps/app/README.md` and the landing page config in `apps/web/lib/`. If a feature isn't live, leave it out; don't write "coming soon".

## Compliance rules

From the landing-page brief, §8. They apply to every page.

**Never:**

- Promise or imply profits for traders ("make money trading", "win rate", "passive income").
- Use these words about Lance: guaranteed, risk-free, safe returns, profit, signals, alpha, financial advice, broker, fund, investment, "100% secure", unhackable. ("Take profit", the order type, is fine.)
- Show fake partner logos, testimonials, user counts or volume figures.
- Mention US stocks, gold, oil or other HIP-3 markets. Lance docs cover crypto perps only.
- Say fees or payouts are "paid automatically". Payouts are a job we run.
- Use Hyperliquid's logo or imply a partnership or endorsement. "On Hyperliquid" as plain text is fine.
- Copy text from other products' sites or terms.
- Use "no KYC" as a selling point, or target US or UK readers.

**Always:**

- End every page with `<RiskWarning />` (from `/snippets/risk-warning.mdx`), except the risk disclosure page itself.
- Give the fee figure wherever fees come up: 0.05% per trade, marked illustrative until final fees are confirmed.
- Label example screens as examples. Northstar is an example brand.
- Keep the official links in `safety/official-links.mdx` in step with the landing page.

## Style

- Second person ("you"), active voice, short sentences.
- Sentence case for headings.
- Bold for buttons and screen names, with the bot's emoji: **🔐 Wallet and access**.
- Code formatting for commands, typed trades and addresses: `/start`, `long eth 50 3x`, `connect.lancetrade.xyz`.
- "Community owner" for partners, "member" for traders, "bot fee" for Lance's builder fee.
