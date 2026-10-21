# Flower Lab Shop legal website

The public pages of Flower Lab Shop's Instagram assistant (home, privacy policy, data deletion, terms, support), served by GitHub Pages from `main` at https://reyfen-org.github.io/Flower-Lab-Shop-Legal/. Each page has a Ukrainian and an English version; change both together. The service itself lives in the private repo `Reyfen/flower-lab-shop`.

## Ground rules

- **Update the "last updated" date with every change.** Whenever a page's content changes, set its date to the day of the change, in both languages, in the same `DD-Mon-YYYY` format (e.g. `21-Oct-2026`). The dates are in the `<p class="updated">` under the page heading of `privacy.html`, `data-deletion.html` and `terms.html` (`Останнє оновлення: …` and `Last updated: …`). `index.html` and `support.html` have no date.
- **The pages must match what the service really does.** The privacy policy lists what the bot stores, who processes it (Meta, Google Cloud, Anthropic, Telegram), and how long it is kept (messages 90 days, summaries at most 3 years). If the service adds a channel, a processor, online ordering or payment, or changes retention, update the policy and the data deletion page before that change goes live. The source of truth for behaviour is `docs/06-security.md` and `docs/09-open-questions.md` in the service repo.
- **Meta uses two URLs from this site:** `privacy.html` (Privacy policy URL) and `data-deletion.html` (User data deletion URL). Don't rename or move them.
- **No cookies, analytics, external fonts or scripts.** The policy says so; `style.css` uses system fonts only.
- **Commit only when asked.** Work happens directly on `main`; a push to it updates the live site.
