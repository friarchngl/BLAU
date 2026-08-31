# BLAU — Eatery & Coffee

Website for **BLAU Eatery & Coffee**, an all-day eatery and coffee bar in Kelapa Gading,
North Jakarta. This repo holds the site itself plus the research and brand notes behind it.

> **Status: work in progress.** The homepage and a dedicated Menu page are built. There is no
> separate About or Visit page — those nav items were dead links pointing at sections that
> never existed, so they were removed rather than built out.
> Some content is still placeholder — see [What still needs input](#what-still-needs-input).

---

## Preview it

**No build step.** The site is plain HTML, CSS and vanilla JavaScript — no framework, no
bundler, no dependencies.

```bash
python -m http.server 8000 --directory site
```

Then open `http://localhost:8000`. Or just double-click `site/index.html`.

There is also `site/index.build.html`, a single self-contained file with every image and the
video inlined as data URIs. Useful for emailing or dropping into a preview tool where you
can't upload a folder. It is **generated** — always edit `site/index.html`, never the build.

## Deploy for client review

**GitHub Pages.** A workflow is included at `.github/workflows/deploy.yml`. One-time setup:
repo **Settings → Pages → Source → GitHub Actions**. After that every push to `main`
publishes `site/` automatically.

**Netlify or Vercel** are faster if you want a link in two minutes — drag the `site/` folder
onto their dashboard. No config needed, since there is nothing to build.

---

## What's on the homepage

| Section | Notes |
|---|---|
| **Hero** | Full-bleed photo, official logo lockup, location and hours |
| **Coffee Bulk Order** | Pinned scroll stage, bottles wiping in against their own label colour |
| **Open Kitchen** | Take-home products, packaging shot crossfades to the product on hover |
| **Menu** | Photo band drifting right to left, continuously; the whole band links through to the dedicated menu page below |
| **What's On** | Horizontal slider with arrows, carrying the four real promo posters |
| **Loyalty Card** | The stop-motion card on a cream ground, autoplay and looping |
| **Footer** | Visit, Order Now, socials, CTA block, legal bar |

The header's **Menu** and **Shop** are both plain links to their own pages now — there is no
dropdown, and no About or Visit item (see the status note above).

Structure follows [locavorenxt.com](https://locavorenxt.com/); the nav hover sweep follows
[uniongroupjakarta.com](https://uniongroupjakarta.com/). Full reasoning in
[`docs/03-references.md`](docs/03-references.md).

## The Menu page

`site/menu.html` is a dedicated, real-HTML menu — all 78 items across all 9 categories,
searchable and readable on mobile, not a PDF embed. A sticky category tab bar sits under the
header and highlights whichever section is in view as you scroll. It shares the homepage's
header and footer components, but the header has no hero to blend into so it stays solid navy
throughout, and the page ground is cream (matching the print menu's interior pages) rather than
the homepage's dark hero.

## The Shop page

`site/shop.html` is the full take-home catalogue: all 8 Coffee Bulk Order flavours and all 4
Open Kitchen products, in a bordered poster grid (the layout the user referenced — hairline
cell borders, name/price row, one-line description). Bulk bottle cards use the same
ground-baked photography as the homepage's pinned stage; Open Kitchen cards keep the
packaging-shot-crossfades-to-product hover from the homepage section. **No prices are shown**
for either range — real pricing was never supplied, so each card reads "Ask on WhatsApp"
(bulk) or its real pack size (kitchen) instead of an invented number, and links straight to a
pre-filled WhatsApp message for that item. Colours and type stay on BLAU's own tokens; only the
grid layout came from the reference.

## Repo layout

```
site/
  index.html            ← the homepage. Edit this one.
  index.build.html      ← generated single-file copy of index.html. Do not edit.
  menu.html             ← the full menu page. Edit this one.
  menu.build.html       ← generated single-file copy of menu.html. Do not edit.
  shop.html             ← the full shop page. Edit this one.
  shop.build.html       ← generated single-file copy of shop.html. Do not edit.
  assets/
    hero.jpg            hero photograph
    brand/              official logo files, transparent margins trimmed
    strip/              dish photography for the Menu band
    promo/              the four promo posters
    loyalty/            loyalty card video + poster frame
    bottles/             Coffee Bulk Order bottle photography, ground baked in
    kitchen/              Open Kitchen packaged/unpackaged product pairs
docs/
  01-brief.md           the business, positioning, assumptions, open questions
  02-menu.md            all 78 menu items transcribed with prices (2026 revision)
  03-references.md      reference sites, what to take from each
  04-style-directions.md  five visual directions and why we picked this one
  05-brand-assets.md    official colours and logo file inventory
  direction-board.html  the five directions, mocked up side by side
assets/
  brand-original/       untouched logo files as supplied
```

**Not in git** (see `.gitignore`): `assets/BLAU-menu-2025.pdf` (29 MB) and
`assets/menu-pages/` (32 MB, the PDF rendered one PNG per page). Together they are 95% of the
folder and none of it is needed to run or review the site — everything useful is already
transcribed into `docs/02-menu.md`, and the dish photography that *is* used lives in
`site/assets/strip/`. Keep both in Drive alongside the repo. Clone size is about 3 MB.

## Design tokens

Sampled directly from the supplied logo files, not guessed. Defined at the top of
`site/index.html`.

| Token | Hex | Role |
|---|---|---|
| `--blau-navy` | `#133A6B` | Primary. The logo navy |
| `--blau-cream` | `#F7F3EB` | Secondary. Warm off-white, **not** pure white |
| `--blau-navy-deep` | `#0C2445` | Derived. Site ground |
| `--blau-navy-mid` | `#1D4E86` | Derived. Secondary fills |

Typeface is **Poppins**, a stand-in for BLAU's real geometric sans. One variable swap when the
brand font is known. Details in [`docs/05-brand-assets.md`](docs/05-brand-assets.md).

---

## What still needs input

Ordered by how much it blocks a launch.

1. **Interior photography.** Every reference site leans on it and BLAU has none — only food
   shots. The hero is currently a drinks photo standing in for a shot of the room.
2. **Vector logo (SVG/AI).** Everything supplied is raster, so the mark can't scale cleanly for
   print or a favicon.
3. **Privacy Policy and Terms pages.** Both are `#` placeholders in the footer. Either write
   them or remove the links before launch.
4. **GrabFood link.** Also `#`. GoFood is wired to the real listing.
5. **Coffee Bulk Order and Open Kitchen pricing.** Never supplied, so `site/shop.html` shows
   "Ask on WhatsApp" for the 8 bulk flavours instead of an invented number. Kitchen items show
   their real pack size (10 pcs, 80 gr, etc.) since that much was confirmed.
6. **The brand typeface.**
7. **Domain, and platform decision** — static hosting as built, or port to WordPress/Elementor
   if you want to edit prices yourself.

Menu prices are current as of the 2026 revision (`assets/BLAU-menu-2026.pdf`, supplied
2026-08-21) — no longer an open item.

### Two inconsistencies worth resolving

- The promo posters use **two different Instagram handles** — `@blau.id` on the affogato
  poster, `@blau.eatery` on the student poster. The site currently links `@blau.id`.
- The Buy 1 Get 1 poster reads **"Cappucino"**. Correct spelling is *Cappuccino*; the site uses
  the correct one.

## Regenerating the single-file build

`site/index.build.html` is `site/index.html` with every `assets/…` reference replaced by a
data URI. Regenerate it after any edit, or delete it if you don't need it.

---

Built for BLAU Eatery & Coffee. Jl. Pelepah Elok I QA2/7, Kelapa Gading, Jakarta Utara.
Open daily 10.00–22.00 · [@blau.id](https://www.instagram.com/blau.id/) ·
[WhatsApp](https://wa.me/6281999718181)
