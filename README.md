# HEI Event Observatory

Interactive dashboard tracking events from 27 Taiwan higher education institutions (15 public + 12 private).

## Live Demo

**[View Dashboard](https://imbad0202.github.io/hei-event-observatory/)**

## Features

- **211 events** crawled from 27 universities across the 2025-2026 academic year
- **13 data-driven categories** derived from keyword analysis (AI/Digital, Medical, Sustainability, etc.)
- **5 interactive tabs**: Overview, Event Browser, Analysis, School Profile, Admin
- **Quality assured**: 99.5% verified with source URLs, fact-checked against original pages
- Light/Dark theme toggle
- XLSX/JSON export
- Fully responsive

## Tech Stack

Single-file HTML dashboard:
- React 18 + Babel Standalone (client-side JSX)
- Tailwind CSS (CDN)
- Chart.js (doughnut, bar, line, polar area)
- SheetJS (XLSX export)
- Google Fonts: Instrument Serif + DM Sans + JetBrains Mono

## Data

- **Source**: University event pages, crawled via WebSearch + WebFetch
- **Date range**: 2025-08-01 ~ 2026-07-31
- **Schools**: NTU, NTHU, NYCU, NCKU, NCCU, NCU, NSYSU, NCHU, NTNU, NTUT, NTUST, CCU, NUK, NCNU, NTOU, FJU, SCU, THU, TKU, FCU, CYCU, YZU, CGU, SHU, PCCU, MCU, USC
- **Quality**: 210 verified / 1 unverified, 0 duplicates removed

## Lighthouse Scores

| Category | Score |
|----------|-------|
| Performance | 55* |
| Accessibility | 100 |
| Best Practices | 100 |
| SEO | 100 |

*Performance limited by CDN-loaded external scripts (React, Babel, Chart.js, Tailwind, SheetJS) inherent to single-file architecture.

## License

MIT
