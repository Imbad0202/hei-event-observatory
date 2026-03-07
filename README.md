# HEI Event Observatory

Interactive dashboard tracking academic events from 27 Taiwan higher education institutions (15 public + 12 private) across **3 academic years** (112–114).

## Live Demo

**[View Dashboard](https://imbad0202.github.io/hei-event-observatory/)**

## Features

- **572 events** crawled from 27 universities across 3 academic years (2023–2026)
- **Multi-year filtering**: Select 112 / 113 / 114 academic year or view all
- **13 data-driven categories** derived from keyword analysis (AI/Digital, Medical, Sustainability, etc.)
- **5 interactive tabs**: Overview, Event Browser, Analysis, School Profile, Admin
- **Quality assured**: 95%+ verified, 0 duplicates, all 12 valid categories
- Light/Dark theme toggle
- XLSX/JSON export (per academic year or full dataset)
- Fully responsive

## Academic Year Coverage

| 學年度 | 期間 | Events |
|--------|------|--------|
| 114 | 2025-08 ~ 2026-07 | 208 |
| 113 | 2024-08 ~ 2025-07 | 205 |
| 112 | 2023-08 ~ 2024-07 | 159 |

## Tech Stack

Single-file HTML dashboard:
- React 18 + Babel Standalone (client-side JSX)
- Tailwind CSS (CDN)
- Chart.js (doughnut, bar, line, polar area)
- SheetJS (XLSX export)
- Google Fonts: Instrument Serif + DM Sans + JetBrains Mono

## Data

- **Source**: University event pages, crawled via WebSearch + WebFetch
- **Date range**: 2023-08-01 ~ 2026-07-31 (3 academic years)
- **Schools**: NTU, NTHU, NYCU, NCKU, NCCU, NCU, NSYSU, NCHU, NTNU, NTUT, NTUST, CCU, NUK, NCNU, NTOU, FJU, SCU, THU, TKU, FCU, CYCU, YZU, CGU, SHU, PCCU, MCU, USC
- **Quality**: ~99% verified / 0 duplicates

## Data Schema

Each event record:
```json
{
  "id": "NTU-114001",
  "school_id": "NTU",
  "school_name": "國立臺灣大學",
  "academic_year": "114",
  "category": "TALK",
  "category_name": "專題演講",
  "title": "...",
  "date": "2025-10-15",
  "unit": "電機工程學系",
  "url": "https://...",
  "source": "webfetch",
  "confidence": "high"
}
```

## License

MIT
