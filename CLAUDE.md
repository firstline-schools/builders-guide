# FirstLine Builders Guide

A single public page, served by GitHub Pages from `main` at
https://firstline-schools.github.io/builders-guide/. It is what anyone at FirstLine reads before
building a tool. It is NOT the starter kit (`firstline-schools/fls-starter-kit`), which is one of the
paths this page describes.

## How the page is laid out
- Top: four steps. (1) Start with your data: where it comes from (you write it / FirstLine's
  official data in BigQuery through the BQ Project / your own Sheet or Form in Drive), then how often
  it changes (once / weekly / by itself). (2) What you're making and who sees it: four rows, simplest
  first (a Claude artifact → a Google Site or GitHub Pages → Forms/Sheets/Apps Script → the starter
  kit); only the last needs GitHub; keep it last. (3) Describe it to Claude naming all three.
  (4) Check it. Keep this short; it is the front door; never send people to GitHub first.
- Facts about what each platform can do (who can open a shared link, plan limits) change often:
  check the vendor's own documentation before changing them, and keep the "last checked" date on
  `#compare` current.
- Below: folded `<details>` sections, each with an `id` that links open it (`#words`, `#compare`, `#google`, `#claude`,
  `#github`, `#backend`, `#path`, `#check`, `#data`, `#lessons`, and each recipe's own id).
  Any `href="#x"` must point at an id that exists on the page.
- `#path` is a six-question chooser; its rules are in the inline script (`decide()`), and every
  recipe id it names must exist.

## Rules
- `index.html` is the source. Styles and script are inline; `fls-logo.png` is the only other file.
- **Public repository:** no student or staff names, IDs or records, no passwords, keys or tokens.
- People build in **claude.ai**; never tell a reader to use a terminal.
- Staff-facing words: name mechanisms and roles (the request form, your supervisor), never a person
  to "ask".
- FirstLine look: navy `#002F60`, orange `#E47727`, Open Sans. "FirstLine", never "Firstline".
- Apps Script samples on the page were tested against a mock Sheet; change one only with the same care.
