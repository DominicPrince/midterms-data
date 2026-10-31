# midterms-data

Live data files for the Midterms tab on [domprince.com](https://domprince.com/midterms): a Polymarket-powered dashboard for the 2026 US midterms. A scheduled GitHub Action in a separate private repo rebuilds them every hour and publishes them here, so a data refresh doesn't cost a site deployment.

| File | What it is | Refreshed |
| --- | --- | --- |
| `news.json` | Recent Google News headlines for each race, grouped by time window | hourly |
| `summary.json` | The short AI-written "what has changed today" note for the Senate, Governor and House views, plus the projected seat counts it quotes | hourly, when the underlying odds move |
| `house.json` | A slim snapshot of every House race, shown while the live odds load | about every 3 hours |

The page reads these through `raw.githubusercontent.com` and falls back to the copies shipped with the site if GitHub can't be reached. Everything here is public information (headlines and market odds).

This repo is temporary and will be deleted after the 2026 midterms.
