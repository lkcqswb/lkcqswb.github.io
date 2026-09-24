# lkcqswb.github.io

Personal academic homepage of Kaicheng Luo, served by GitHub Pages from `index.html`.
It is a single static file: no build step, no framework, and only a few lines of JavaScript
(the BibTeX show/copy buttons).

## Layout

- **Title block**: name, affiliation, research focus, links.
- **About / Research / Publications / Education / Contact**: each section is a two-column row,
  with the section name on the left and the content on the right. The layout collapses to one
  column below 760px.
- **Figure 1** (in Research) is plain HTML/CSS, not an image. Its labels (a)–(c) are
  cross-referenced by the list of research directions below it.
- Light and dark themes follow the visitor's system setting (`prefers-color-scheme`).
  Colours are tokens at the top of the `<style>` block.
- Fonts: Source Serif 4 (text), Source Sans 3 (labels, UI), Source Code Pro (BibTeX), loaded
  from Google Fonts with system fallbacks.

## Editing

- **Add a paper**: copy one `<li class="pub">` block inside `<ol class="pubs">`, newest first.
  Give it a unique `id="pub-…"`. The BibTeX button's `aria-controls` must match the `id` of its
  `<div class="bib">`.
- **Add a portrait**: save the photo as `portrait.jpg` in the repo root and uncomment the
  `<img class="portrait">` line in the title block.
- **Update "Last updated"** in the footer when the content changes.

## Where the publication data came from (checked 2026-09-24)

- Titles, arXiv IDs and project pages: arXiv and conference listings, found through web search.
  OpenReview, arXiv, dblp and PMLR themselves were not reachable from the editing environment.
- Author order is the order on the previous version of this page, which was taken from OpenReview.
  The ICML 2025 proceedings order for OmniAudio matches it. The arXiv BibTeX in the ThinkSound and
  OmniAudio repositories uses an older order, so the arXiv versions differ from the published ones.
- The BibTeX entries were written from those fields. Only OmniAudio carries proceedings volume and
  page numbers (PMLR 267, pp. 39060–39084).
- GitHub star counts (ThinkSound 1.4k, OmniAudio 378) are a static snapshot from the same date.
