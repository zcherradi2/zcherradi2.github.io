# zcherradi2.github.io

The source of my portfolio and services site, published by GitHub Pages:
**https://zcherradi2.github.io**

Plain static HTML with CSS inlined into each page. No build step, no framework, no JavaScript
dependency for the content to be readable. That is deliberate: a page that needs a toolchain to
render is a page that can break between a recruiter opening it and the work needing to be seen.

## Pages

| Page | What it is for |
|---|---|
| [`index.html`](https://zcherradi2.github.io/) | Who I am, selected work, tools, and the link to the services page |
| [`projects.html`](https://zcherradi2.github.io/projects.html) | Six projects with stack, what was hard, and a measured result for each |
| [`services.html`](https://zcherradi2.github.io/services.html) | Three fixed-scope offers with the price written down |
| [`case-study.html`](https://zcherradi2.github.io/case-study.html) | One document-AI project measured end to end, in English and French |

## The case study

`case-study.html` is the page I would point a client at first. It shows two invoices from different
sectors going through the same extractor, the twelve and eleven fields returned, the three
arithmetic checks passing on both, and - more useful - what the tool refuses to do: an invoice whose
page 1 prints a total for half its lines is flagged rather than booked.

Every invoice image on that page is **rendered from the actual PDFs**, not a mock-up. Both are
synthetic documents with fictional suppliers and clients, marked
"Document de démonstration - données fictives" on their face.

The reference implementations and the measurement logs behind those figures live in the private
working repository, so the numbers can be re-run rather than taken on trust.

## Editing

```powershell
# pages are hand-written; no build step
# open any page directly in a browser, or serve the folder:
python -m http.server 8123
```

Assets used by the pages (CV, case-study PDF, invoice images) are in `assets/`. Anything larger than
a few hundred KB is referenced by path rather than inlined.

## Licence

Content and design: all rights reserved. The text and images describe my own work; please do not
republish them as your own.
