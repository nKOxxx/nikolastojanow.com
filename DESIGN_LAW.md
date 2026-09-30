# PORTFOLIO DESIGN LAW — BINDING

**Rule 1 — Each project page carries its product's own design.** No shared template.
`assets/site.css` is deprecated for project pages.

**Rule 2 — Existing user-approved designs are the source of truth.** Never invent a
replacement for a design the user has already seen and approved. If the design isn't in
this repo's history, it was built in another tool/session — ASK the user for the original
file before redesigning anything.

**Rule 3 — Content law:** no fund/protocol/location claims anywhere; builder-only
positioning. Press history (factual) is allowed.

## Per-page identities (current)

| Page | Identity | Status |
|---|---|---|
| `projects/nybls/` | User's Nybls.html verbatim: violet/acid/magenta, "Feed your brain. Keep the good stuff.", interactive product demo, Find Vault, marquee | RESTORED `f759184` — original was built outside repo history and flattened twice; never again |
| `projects/sovereign-grid/` | Product `design/tokens.css` law: near-black ladder, azure `#3e8bff`, Linear-school data-dense | rebuilt `d95ded2` |
| `projects/alleadz/` | Product `client/src/styles.css`: light paper `#f6f7fb`, indigo `#4338ca`, working-surface shell | rebuilt `d95ded2` |
| `projects/kontor/` | `~/mach/site/` identity: near-black `#0c0e12`, chartreuse `#e8ff47`, Geist Mono | rebuilt `d95ded2` |
| `projects/sovereign-twin/` | User's Sovereign_Twin_Overview.html verbatim: ink/black + signal red `#ff334e`, Georgia serif, orbital hero, decision loop, control room, Reversal & Invalidation Engine | SHIPPED `80595a0` — replaced my invented copper concept page (which never existed as an approved design) |
| `projects/gulfwatch/`, `projects/demoz/` | Still shared-template — need their own identities (ask user for originals if any) | TODO |
| home `index.html`, `projects/index.html` | Personal brand: warm ink `#14120e`, cream `#f2efe8`, gold `#f2d32a` (user logo DNA) | current |

## Ops facts
- GH Pages ~75s post-push; verify live via StealthyFetcher (`~/.scrapling-venv/bin/python`) — sandbox curl returns 000.
- QA recipe: serve repo on localhost (background server), Goliath REST `127.0.0.1:9377` (body needs `userId` + `sessionKey`), fullPage screenshot → PIL crop → tesseract psm 3/4 (write output to file in $HOME, not /tmp — leptonica sandbox quirk), pixel census for accent colors.
- nybls slime art lives at `projects/nybls/slime.png` (extracted from user's 3MB base64 data-URI).
