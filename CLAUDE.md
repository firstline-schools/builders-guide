# FirstLine Builders Guide

A single public page, served by GitHub Pages from `main` at
https://firstline-schools.github.io/builders-guide/. It is what anyone at FirstLine reads before
building a tool. It is NOT the starter kit (`firstline-schools/fls-starter-kit`), which is one of the
paths this page describes.

## How the page is laid out
- Top: four steps (describe it to Claude → build it where it belongs → GitHub only if it needs a
  server → check it before others rely on it), then four rules. Keep this short; it is the front door.
- Below: folded `<details>` sections, each with an `id` that links open it (`#google`, `#claude`,
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
