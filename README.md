# The Cantillon Institute

Live site: [cantillon.institute](https://cantillon.institute)

An independent research institute examining the structural transformation of monetary systems, capital formation, and the political economy of financial power. Est. 2021, Washington D.C.

---

## How the site works

This is a static site. Every file in this repository is served directly to the browser. There is no database, no backend, and no build process. Netlify detects any commit to this repository and redeploys the live site automatically within 60 seconds.

---

## File structure

```
/
├── index.html        Main homepage
├── style.css         All design and layout
├── llms.txt          AI crawler optimisation and content index
├── robots.txt        Search engine crawler instructions
├── favicon.png       Browser tab icon
├── og-image.png      Social sharing preview image (1200x630)
├── README.md         This file
└── papers/
    ├── full-report.pdf           Complete working paper series
    ├── paper-01.pdf              No. 1: What GENIUS and CLARITY Actually Build
    ├── paper-02.pdf              No. 2: Repercussions of the Dollar Displacement Architecture
    ├── paper-03.pdf              No. 3: The Labor Vector
    ├── paper-04.pdf              No. 4: The Rate Corridor Under Pressure
    ├── paper-05.pdf              No. 5: Two Failures from One Decision
    ├── paper-06.pdf              No. 6: The Hollow Bank
    ├── paper-07.pdf              No. 7: The Permanent Record
    ├── paper-08.pdf              No. 8: The Accelerated Contradiction
    └── paper-09.pdf              No. 9: The Invisible Tax
```

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
2. Go into the papers/ folder on GitHub
3. Click Add file, then Upload files
4. Upload the new file; GitHub will overwrite the existing one
5. Commit changes

---

## Adding new papers

1. Name the file following the established convention: `paper-10.pdf`, `paper-11.pdf` etc.
2. Upload to the `papers/` folder
3. Add the paper row to `index.html` following the existing pattern
4. Update `llms.txt` with the new paper title and abstract
5. Commit all changed files together

---

## Adding new pages

Each new page is a new `.html` file in the root directory. Copy the structure of `index.html`, keep the same nav and footer, link to the existing `style.css`. Upload and commit. The page is live immediately at `cantillon.institute/filename.html`.

Examples of planned pages:
- `thornton.html` — Thomas H. Thornton fellow biography and papers
- `fisher.html` — Diana I. Fisher fellow biography and papers
- `martyn.html` — Henry E. Martyn fellow biography and papers

---

## Domain setup

- Primary domain: `cantillon.institute` (canonical)
- Redirect domain: `cantillon.xyz` (redirects to primary)
- Both managed via Namecheap nameservers pointing to Netlify DNS
- SSL certificates managed automatically by Netlify

---

## Design system

- Background: `#0b0c0d`
- Primary text: `#dedad0`
- Accent: `#378ADD` (cold steel blue)
- Headline font: Barlow Condensed 700
- Body font: DM Sans 400/600/700
- Paper font: IBM Plex Serif

---

*This repository is private infrastructure for cantillon.institute. Do not expose API keys, personal information, or unpublished draft content.*
