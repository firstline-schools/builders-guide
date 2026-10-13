# FirstLine Builders Guide

A single public page, served by GitHub Pages from `main` at
https://firstline-schools.github.io/builders-guide/. It is what anyone at FirstLine reads before
building a tool. It is NOT the starter kit (`firstline-schools/fls-starter-kit`), which is one of the
paths this page describes.

## How the page is laid out
- Top: three steps. (1) "What are you building?": five rows from simplest to most involved (a Claude
  page → a one-time look at data through the BQ Project → a Google Site → Forms/Sheets/Apps Script →
  the starter kit). Only the last row needs GitHub; keep it last. (2) Describe it to Claude and name
  the row picked, so the assistant doesn't choose a different path. (3) Check it. Keep this short; it
  is the front door, and it must not send people to GitHub first.
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
