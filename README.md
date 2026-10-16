# Anass Bouchnita — PI academic website (v11, October 2026)

This is a static, multipage academic website. It retains the original navy/ivory academic style and includes the site owner's existing portrait and scholarly figures.

## Deploy on GitHub Pages

1. Create a GitHub repository (or use the existing academic website repository).
2. Upload **all files inside `bouchnita-academic-site/`** to the repository root. In particular, `index.html`, `site.js`, `styles.css`, and `assets/` must be at the same level.
3. In GitHub select **Settings → Pages → Build and deployment → Deploy from a branch**, then select `main` and `/ (root)`.
4. The site will be at `https://<username>.github.io/<repository>/`, unless configured as a user site or custom domain.

No build step, dependencies, API keys, or server-side runtime are needed.

## Pages

- `index.html`: PI overview, affiliation, latest Frontiers Research Topic, earlier news.
- `research.html`: integrated multiscale modeling and mechanistically informed AI research program, with a nonredundant set of methods and domain applications.
- `cancer-cell-dynamics.html`: a two-column synthesis of the ERK/p38 tumor–immune study and the 2019 EGFR model, with figures, findings and citations; related works follow.
- `cardiovascular.html`: consolidated studies on platelet calcium signaling and coagulation thresholds, with paired scientific panels and citations.
- `infection-immunity.html`: a consolidated ISG/viral regulation study with paired scientific plots, plus published influenza and population-immunity results, epiENGAGE, and citations.
- `mechanistic-ai.html`: a consolidated EGFR/ERK surrogate-learning study illustrated by author working-result plots, followed by related AI applications.
- `publications.html`: searchable/filterable collection of **55 peer-reviewed journal articles and 7 conference proceedings** derived from the supplied CV, with DOI links or Google Scholar title searches.
- `people.html`, `software.html`, `about.html`: existing team and software sections; expanded academic biography and responsibilities.

## Editing and updating

- News is maintained in the `index.html` section `#news`; keep items reverse chronological and date them explicitly.
- Publication data are in `site.js` and `PUBLICATIONS_DATA.json`; update both for future additions. If a direct publisher link is not verified, the page offers a Scholar title search.
- The verified Google Scholar **author profile ID** could not be identified. All “Academic profile” links therefore use the Google Scholar author-search page. To link to the exact profile, replace `https://scholar.google.com/citations?view_op=search_authors&mauthors=Anass+Bouchnita&hl=en` in the HTML pages with a known `https://scholar.google.com/citations?user=...` URL.
- Shared headers and footers are static across pages. Update all HTML files if changing them.
- `FIGURE_CREDITS.md` documents genuine publication figures, author numerical snapshots, and the user-provided infographic, with explicit distinctions between published and working result panels.
- `UPDATES_2026.md` lists the factual sources used for this update.

## Technical checks

- Confirmed all local HTML/image/script references resolve.
- V9 was rendered using inline-asset desktop and mobile browser previews; all displayed images loaded and no horizontal overflow was detected. Normal browser navigation was restricted in this runtime.
- Validated JavaScript syntax and tested live publication search and area filter (56 initial records; one record on a `dormancy` search).
- Figures, portrait, styles and publication data are stored within the static bundle.

The website has no embedded tracking or external API credentials. Google Fonts, DOI/article and institutional hyperlinks load over the public web.


## v10 publication refresh and editorial polishing (October 2026)

- `publications.html` now reads its 55 journal and 7 proceedings records from `site.js`, aligned to `My_cv (5).pdf` supplied by the researcher. Journal and conference records are separated using the publication type filter.
- Bibliographic display preserves CV year, author sequence, title, journal and available volume/issue/page or article number. For papers without a verified direct link, the link goes to an exact-title Scholar search.
- The About page retains the publication figure (55) but omits the research-theme and doctoral-degree counters, by request; substantive background is preserved.
- Site-wide styling revisions target consistent typography, spacing, accessible links, mobile column wrapping and readability.
- `PUBLICATIONS_DATA.json` is the independent structured bibliography and can be updated alongside `site.js` as new papers appear.

## v11 principal-investigator language and website credit

- The visible content uses a consistent first-person PI perspective ("I", "my research program", and "my collaborators") while preserving explicit credit for coauthored research.
- The About biography and leadership sections are in the PI's first-person voice; the 55-paper metric remains unchanged.
- Each content page has a subtle footer note: **Website design assisted by ChatGPT (OpenAI) · Hosting: GitHub Pages**. Hosting is a deployment designation, not proof that the files have already been published online.
- The site is static and ready for deployment on GitHub Pages following the instructions above.
