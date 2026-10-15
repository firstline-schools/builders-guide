# FirstLine Builders Guide

A single public page, served by GitHub Pages from `main` at
https://firstline-schools.github.io/builders-guide/. It is what anyone at FirstLine reads before
building a tool. It is NOT the starter kit (`firstline-schools/fls-starter-kit`), which is one of the
paths this page describes.

## How the page is laid out
- Top (AI Task Force feedback, 2026-10-14: "too busy", pathways first, more graphic, prompts): the four
  stops as one graphic trail, simplest first (1 a Claude artifact or Gemini Canvas page; 2 a Google Site;
  3 Forms/Sheets/Apps Script; 4 the starter kit, the only stop that needs GitHub; keep it last). Each stop
  has "Start with a prompt" (opens the prompt box: Copy, Open in Claude = claude.ai/new?q=, Open in ChatGPT =
  chatgpt.com/?q=, Gemini = copy then paste) and direct links (sites.new, forms.new). Then one "not sure?"
  line and four tiles (#source, #describe, #check, #ip). Keep the top to exactly that.
- The folds that used to sit on top (#words, #source, #describe, #compare) live under "Good to know".
- #ip (who owns what you build) sits after the rules; vendor terms checked 2026-10-14; two FirstLine policy
  lines are marked "To confirm" until FirstLine decides.
- Facts about what each platform can do (who can open a shared link, plan limits) change often:
  check the vendor's own documentation before changing them, and keep the "last checked" date on
  `#compare` current.
- Below: folded `<details>` sections, each with an `id` that links open it (`#words`, `#compare`, `#google`, `#claude`,
  `#github`, `#backend`, `#path`, `#check`, `#data`, `#lessons`, and each recipe's own id).
  Any `href="#x"` must point at an id that exists on the page.
- `#path` is a six-question chooser; its rules are in the inline script (`decide()`), and every
  recipe id it names must exist.

## Rules
- `glossary.html` is a second page: the technical words (118 terms, seven groups, a search box), linked from the end of `#words` ("Dive deeper"). Plain words; "At FirstLine" lines only for facts you have checked. Add terms in the right group, alphabetically.
- `index.html` is the source. Styles and script are inline; `fls-logo.png` is the only other file.
- **Public repository:** no student or staff names, IDs or records, no passwords, keys or tokens.
- People build in **claude.ai**; never tell a reader to use a terminal.
- Staff-facing words: name mechanisms and roles (the request form, your supervisor), never a person
  to "ask".
- FirstLine look: navy `#002F60`, orange `#E47727`, Open Sans. "FirstLine", never "Firstline".
- Apps Script samples on the page were tested against a mock Sheet; change one only with the same care.
