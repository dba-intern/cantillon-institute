# The Cantillon Institute

Live site: [cantillon.institute](https://cantillon.institute)

An independent research institute examining the structural transformation of monetary systems, capital formation, and the political economy of financial power. Est. 2021, Washington D.C.

---

## How the site works

This is a static site. Every file in this repository is served directly to the browser. There is no database, no backend, and no build process. Netlify detects any commit to this repository and redeploys the live site automatically within 60 seconds.

---

## File naming convention

All paper files — both HTML and PDF — follow a consistent `[fellow]-paper-[nn]` convention:

```
[fellow]-paper-[nn].html    HTML working paper page (e.g. thornton-paper-01.html)
[fellow]-paper-[nn].pdf     PDF download (e.g. thornton-paper-01.pdf, in /papers folder)
[fellow].html               Fellow biography and paper index (e.g. thornton.html)
```

The `[fellow]` segment uses the fellow's lowercased family name:
`thornton`, `eccles`, `vargas`, `black`, `rueff`, `myrdal`, `tobin`, `fisher`, `menger`, `nakamura`, `cos`, `martyn`, `khaldun`, `liang`, `galbraith`

---

## File structure

```
/
├── index.html                    Homepage
├── papers.html                   Full papers archive (all 15 series)
├── briefs.html                   Briefs archive (research staff digests)
├── signals.html                  Market data and indicators (live FRED + DefiLlama + static datasets)
├── about.html                    Institute about page
├── glossary.html                 Monetary economics glossary
├── style.css                     All design and layout
├── sitemap.xml                   Search engine sitemap
├── llms.txt                      AI crawler optimisation and content index
├── robots.txt                    Search engine crawler instructions
├── favicon.png                   Browser tab icon
├── og-image.png                  Social sharing preview image (1200×630)
├── README.md                     This file
│
├── Fellow biography pages
│   ├── thornton.html             Thomas H. Thornton — The Dollar Displacement Thesis
│   ├── eccles.html               Preston W. Eccles — The Transmission Problem
│   ├── vargas.html               Elena R. Vargas — The Invisible Economy
│   ├── black.html                Kai R. Black — The Protocol Layer
│   ├── rueff.html                Renée V. Rueff — The Union's Fault Lines
│   ├── myrdal.html               Helena S. Myrdal — The Destination Thesis
│   ├── tobin.html                Gideon W. Tobin — The Architecture of Preservation
│   ├── fisher.html               Diana I. Fisher — The Liability Architecture
│   ├── menger.html               Adrian K. Menger — Insurance and the Digital Asset Gap
│   ├── nakamura.html             Rin Y. Nakamura — The Institutional Deficit
│   ├── cos.html                  Jacob T. Cós — The Sovereign Compact
│   ├── martyn.html               Henry E. Martyn — The Long Record
│   ├── khaldun.html              Tariq N. Khaldun — The Riba Question
│   ├── liang.html                Wei J. Liang — The Internal Circulation
│   └── galbraith.html            Dana M. Galbraith — The Consumption Layer
│
├── Working paper HTML pages
│   ├── thornton-paper-01.html    No. 1: What GENIUS and CLARITY Actually Build
│   ├── thornton-paper-02.html    No. 2: Repercussions of the Dollar Displacement Architecture
│   ├── thornton-paper-03.html    No. 3: The Labor Vector
│   ├── thornton-paper-04.html    No. 4: The Rate Corridor Under Pressure
│   ├── thornton-paper-05.html    No. 5: Two Failures from One Decision
│   ├── thornton-paper-06.html    No. 6: The Hollow Bank
│   ├── thornton-paper-07.html    No. 7: The Permanent Record
│   ├── thornton-paper-08.html    No. 8: The Accelerated Contradiction
│   ├── thornton-paper-09.html    No. 9: The Invisible Tax
│   ├── eccles-paper-01.html      The Reserve Channel
│   ├── vargas-paper-01.html      The Pressure Point Thesis
│   ├── black-paper-01.html       The Finality Illusion
│   ├── rueff-paper-01.html       The Settlement Gap
│   ├── myrdal-paper-01.html      The Architecture of Arrival
│   ├── tobin-paper-01.html       What the GENIUS Act Means for Trust-Held Assets
│   ├── fisher-paper-01.html      The Pension Fund Problem
│   ├── menger-paper-01.html      The Valuation Problem
│   ├── nakamura-paper-01.html    The Shimomura Inversion
│   ├── cos-paper-01.html         The EIB at the Inflection Point
│   ├── martyn-paper-01.html      The Bretton Woods Lesson
│   ├── khaldun-paper-01.html     The Threshold Question
│   ├── liang-paper-01.html       The Complete Stack
│   └── galbraith-paper-01.html   The Other Side of the Ledger
│
└── papers/                       PDF downloads
    ├── thornton-full-report.pdf  Complete Dollar Displacement Thesis (email-gated on homepage)
    ├── thornton-paper-01.pdf
    ├── thornton-paper-02.pdf
    ├── thornton-paper-03.pdf
    ├── thornton-paper-04.pdf
    ├── thornton-paper-05.pdf
    ├── thornton-paper-06.pdf
    ├── thornton-paper-07.pdf
    ├── thornton-paper-08.pdf
    ├── thornton-paper-09.pdf
    ├── eccles-paper-01.pdf
    ├── vargas-paper-01.pdf
    ├── black-paper-01.pdf
    ├── rueff-paper-01.pdf
    ├── myrdal-paper-01.pdf
    ├── tobin-paper-01.pdf
    ├── fisher-paper-01.pdf
    ├── menger-paper-01.pdf
    ├── nakamura-paper-01.pdf
    ├── cos-paper-01.pdf
    ├── martyn-paper-01.pdf
    ├── khaldun-paper-01.pdf
    ├── liang-paper-01.pdf
    └── galbraith-paper-01.pdf
```

---

## Brief file naming convention

Research Briefs follow a date-first naming convention:

```
brief-[YYYY]-[MM]-[DD]-[slug].html
```

Examples:
```
brief-2026-05-19-occ-genius-yield-overreach.html
brief-2026-05-19-ncua-genius-credit-union-split.html
```

Slugs should be 3 to 4 words maximum. Briefs are attributed to Research Associate, Research Analyst, or Research Assistant — never a personal name.

When a new Brief is published, update three files:
1. `briefs.html` — add a new brief-row entry at the top of the list
2. `sitemap.xml` — add the new URL at priority 0.7
3. `llms.txt` — paste the llms.txt block produced at the end of Brief generation

---

## Signals page

`signals.html` contains 12 charts across 5 thematic sections:

| Section | Charts | Source |
|---|---|---|
| Dollar Architecture | Stablecoin market cap, Fed reserve balances, ON RRP, Top 5 issuers, SWIFT share | DefiLlama API (live), FRED API (live, key required), Static |
| European Fractures | TARGET2 balances | Static (ECB, Dec 2024) |
| Tokenization | RWA by asset class | Static (RWA.xyz, Dec 2024) |
| Alternative Stack | mBridge cumulative settlement, e-CNY transaction value | Static (manual update) |
| Capital Movement | Singapore family offices, Islamic finance assets | Static (manual update) |
| Illicit Flows | Illicit VA volume stablecoin vs other | Static (Chainalysis/FATF 2026) |

**FRED API key** is stored in the `FRED_API_KEY` constant at the top of signals.html. Key: configured. Do not expose in public documentation.

**To add a chart:** add a new `.signal-card` div in the appropriate section, add the corresponding Chart.js build function in the script block, call it in the `DOMContentLoaded` init section.

**To update static data:** edit the labels/values arrays directly in the relevant build function in signals.html.

---

## GitHub Desktop workflow (recommended)

Using GitHub's web upload interface only updates the specific files you drag in — all other files in the repo stay at their previous version. This causes nav inconsistencies when some pages are updated and others are not.

**Correct workflow using GitHub Desktop:**

1. Clone the repo once: File > Clone repository > dba-intern/cantillon-institute
2. When Claude produces output files, download them and copy into the cloned repo folder, replacing existing files
3. GitHub Desktop shows all changed files automatically in the left panel
4. Write a commit message at the bottom left
5. Click **Commit to main**
6. Click **Push origin**
7. Netlify deploys automatically within 60 seconds

The cloned repo folder is the single source of truth. Never upload files to GitHub web interface — always use GitHub Desktop to push from the local folder.

---

## Updating the site

**To edit any page:**
1. Open the file on GitHub
2. Click the pencil icon to edit
3. Make changes
4. Click Commit changes
5. Netlify redeploys automatically

**To update a PDF:**
1. Name the new file identically to the one it replaces
2. Go into the `papers/` folder on GitHub
3. Click Add file → Upload files
4. Upload the new file; GitHub will overwrite the existing one
5. Commit changes

---

## Adding a new paper by an existing fellow

1. **PDF:** Name the file `[fellow]-paper-[nn].pdf` (e.g. `thornton-paper-10.pdf`) and upload to `papers/`
2. **HTML:** Create `[fellow]-paper-[nn].html` following the template of any existing paper page for that fellow
3. **Bio page:** Update `[fellow].html` — replace the forthcoming entry in the series section with a published paper row linking to the new HTML page
4. **Papers archive:** Add the new paper row to `papers.html` in the correct series block
5. **Sitemap:** Add `<url>` entry to `sitemap.xml` at priority `0.9`
6. **llms.txt:** Add the paper title and abstract to the content index
7. Commit all changed files together

---

## Adding a new fellow and series

1. **Bio page:** Create `[fellow].html` from the bio page template
2. **Paper HTML:** Create `[fellow]-paper-01.html` from the working paper template
3. **PDF:** Upload `[fellow]-paper-01.pdf` to `papers/`
4. **Homepage fellows grid:** Add a fellow card to `index.html` in the `#fellows` section
5. **Papers archive:** Add a new series block to `papers.html`
6. **Sitemap:** Add entries for the bio page (priority `0.8`) and paper page (priority `0.9`)
7. **llms.txt:** Add the fellow and their series to the content index
8. Commit all files together

---

## Fellows and series

| Fellow | Series | Location |
|--------|--------|----------|
| T.H. Thornton | The Dollar Displacement Thesis (9 papers) | New York |
| P.W. Eccles | The Transmission Problem | Washington D.C. |
| E.R. Vargas | The Invisible Economy | Montevideo |
| K.R. Black | The Protocol Layer | Lisbon |
| R.V. Rueff | The Union's Fault Lines | Frankfurt |
| H.S. Myrdal | The Destination Thesis | Singapore |
| G.W. Tobin | The Architecture of Preservation | Bermuda |
| D.I. Fisher | The Liability Architecture | London |
| A.K. Menger | Insurance and the Digital Asset Gap | Zurich |
| R.Y. Nakamura | The Institutional Deficit | Tokyo |
| J.T. Cós | The Sovereign Compact | Monaco |
| H.E. Martyn | The Long Record | Washington D.C. |
| T.N. Khaldun | The Riba Question | Doha |
| W.J. Liang | The Internal Circulation | Shanghai |
| D.M. Galbraith | The Consumption Layer | Chicago |

---

## Domain setup

- Primary domain: `cantillon.institute` (canonical)
- Redirect domain: `cantillon.xyz` (redirects to primary)
- Both managed via Namecheap nameservers pointing to Netlify DNS
- SSL certificates managed automatically by Netlify

---

## Design system

- Background: `#0b0c0d`
- Primary text: `#e8e4da`
- Accent: `#378ADD` (cold steel blue)
- Headline font: Barlow Condensed 700
- Body font: DM Sans 400/600/700

---

*This repository is private infrastructure for cantillon.institute. Do not expose API keys, personal information, or unpublished draft content.*
