# ef-product-log

Product sourcing log for Ellison & Fitz

**Brand:** Ellison & Fitz  
**Lane:** Backend ops / sourcing  
**Status:** Repo `ellison-fitz/ef-product-log`. Kept separate from `ef-sops` (this log has supplier names and costs).  
**Not for:** VA customer-support pages. CS truth stays on the [live SOP](https://kevinc710.github.io/ef-sops/). Ops how stays in [ops/](https://kevinc710.github.io/ef-sops/ops/).

This file is the current state of every product we are moving between suppliers. Each product page has the current facts at the top and a dated log underneath, newest first. Rewrite the top block in place when a fact changes. Do not stack "Updated" footnotes: put the date in the log.

Site: index.md + products/ render via GitHub Pages (Jekyll). Each product page now has a **Scale read** row (30-day units and trend, margin vs supplier cost, supplier reliability, Meta).

Snapshot taken Fri 2026-10-23, ~10:25 AM CT. Shopify reads (status, price, buyable colors, open orders) are from the Admin API at that time. 30-day sales are Shopify analytics net units for 2026-09-23 to 2026-10-23 (today partial), with the prior 30 days and last 7 (10-17 to 10-23) vs prior 7 days (10-10 to 10-16) for trend. Meta is read-only from ad set and campaign names, last 30 days and 10-20 to 10-22, using Meta-reported purchases and ROAS. The "35 / 1.53" style numbers in ad set names are copied as written; 1.53 is read as the break-even ROAS. Slack and WhatsApp were not re-read for this refresh.

## Rules

| Rule | Current how |
|---|---|
| Main supplier | **Cherry / Beehive** (Beehiveship) |
| Approved backups | **Lay** (Dropsure) and **Hart** (Wio). Use them only for products Cherry can't cover. |
| Traction | 3+ sales in 30 days |
| Substitutes | Never ship a different item, color, size or style without telling the customer first and getting their OK (or offering a refund). |
| Dead tracking | If Shopify shows a Cherry tracking number that never moved, the customer gets an update from Abby before we re-source. |
| Shopify writes | Agents need Kevin's explicit OK. Listing color blocks are done by Leandro or Kevin. |
| WhatsApp | Nobody sends to Lay or Hart unless Kevin says to send that message. |

## Index

| Product | Current supplier | Cost | Live colors | Status | Open orders | 30d units (trend) · Meta | Scale read | Next action | Owner |
|---|---|---|---|---|---|---|---|---|---|
| [Maris Drape Sweater](products/maris-drape-sweater.md) | Cherry. Hart pitched | $17.41 Cherry (PLW) vs $20.30 Hart landed | 8 colors, XS–5XL | Live | none | 348 (7d 98 vs 88, up) · On, ROAS 1.54 30d / 1.22 last 3d | Scale product. ~$32.58 margin. Last 3d ROAS under 1.53 for the third read running | Finish Cherry vs Hart comparison. Watch ROAS | Kevin |
| [Enzo Button Knit](products/enzo-button-knit.md) | Cherry. Hart pitched | $14.76 Cherry (PLW) vs $14.40 Hart landed | Olive, Coffee, Black (2 listings) | Live | none. 11941 + 11942 on one tracking, both still fully paid | 68 (7d 26 vs 35, down) · On, ROAS 1.61 30d / 1.03 last 3d | **Scale candidate, on watch.** ~$25.23 margin. Last 3d under 1.49 | Finish Cherry vs Hart comparison. Check whether 11941/11942 needs a refund | Kevin |
| [Camille Knit Sweater](products/camille-knit-sweater.md) | Lay (only source) | unknown | Coffee, Apricot, White, Black (Emerald, Burgundy off) | Partial | 11831 (Emerald S, 10 days). 5 Lay orders still on old 10-10 tracking | 30 (7d 8 vs 12) · On, ROAS 2.02 30d / 3.85 last 3d | Strong ROAS, but supply-blocked (Lay only, cost unknown) | Lay ships the 5 + tells us her 4 colors. 11831 color swap or refund | Abby (Lay) |
| [Freya Zip Pullover](products/freya-zip-pullover.md) | Cherry (1688 colors). Lay/Hart asked for Temu colors | $18.91 US 1pc (Cherry quote) | Temu listing: Camel, Navy, Olive, Pink (Butter, Grey off). 1688 listing `freya-pullover`: 8 colors | Partial | 11798, 11832, 11868, 11874, 11888, 11893, 11903, 11934, 12055 | 17 (7d 4 vs 13, down) · On (V1 + V2), ROAS 1.18 30d / 0.93 last 3d | No: 6 of 9 open orders unmatchable, ROAS under 1.46, sales slowing | Abby: Butter/Grey buyers switch or refund | Abby |
| [Denver Knit Pullover](products/denver-knit-pullover.md) | Cherry (new cream version) | $9.36/unit bulk ex-shipping. Sample price "very high", exact unknown | Cream only (still buyable) | Partial | 12104 (Cream M, 10-23) | 20 (7d 18 vs 2) · On, ROAS 1.18 30d / 0.84 last 3d, CPA ~$74 | No: misses Axel's 5+/day at ≤ $21 CPA. Price now $64.99 (was $39.99) | Hold the 250 bulk. Watch how the $64.99 price converts | Kevin |
| [Milan Leopard Dress](products/milan-leopard-dress.md) | Cherry | $23.40 (PLW) | Navy, Sky | Partial | 11556 (1 Navy S, 22 days) | 24 (7d 1 vs 0) · Nearly off, ROAS 1.36 30d | Cooled off. Not a scale call now | Find out why Cherry is holding 11556 | Abby |
| [Milo Lattice Polo](products/milo-lattice-polo.md) | Cherry (no Emerald) | $14.14 (PLW) | 6 colors (Emerald off) | Partial | none | under 3 · Test ad set, ~$1 last 3d | No traction | none | Abby |
| [Willa Crop Jacket](products/willa-crop-jacket.md) | Cherry (no Orange). Hart max size L | $18.60 (PLW) | Cream, Red, Orange still buyable | Partial | 11807 (Orange XL + Red XL, 11 days) | 2 (0 in 7d) · Off (ad set paused) | No traction | Ads are off, so draft (Leandro/Kevin). Offer 11807 L or refund | Leandro, Abby |
| [Veylan Pullover](products/veylan-pullover.md) | Hart (alt style). Cherry discontinued | $13.30 Hart alt | Black, White (S–3XL on listing; Hart is M–3XL) | Partial | none | 5 (0 in 7d) · Off | Not a candidate | Watch the new tracking move | Kevin |
| [Kian Rivet Short](products/kian-rivet-short.md) | Hart (US-shipped alt). Cherry discontinued | $25.50–$28.70 each | Grey, Black (listing Unlisted) | Drafted | none | 0 · Off | Not a candidate | Keep Unlisted | Kevin |
| [Elisa Flat Loafers](products/elisa-flat-loafers.md) | unknown | unknown | none (Draft) | Drafted | none | 3 (pre-draft) · none | Parked for GMC | Bring back with clean photos after GMC review clears | Kevin, Leandro |
| [Leif Stripe Trouser](products/leif-stripe-trouser.md) | none. Cherry has no exact match | $19.34 (PLW) | Khaki (listing still Active) | Blocked | none | 0 net · Off | Not a candidate | Decide whether to draft the listing | Kevin, Leandro |
| [Linnea Pearl Top](products/linnea-pearl-top.md) | unknown (Cherry pointed to Lay) | $15.87 (PLW) | Black, Light Cyan, Peach, Cream | Blocked | 11661 (17 days) | under 3 · Off | Not a candidate | Confirm with Lay or refund | Abby |

Status key: **Live** = sourced and shipping normally. **Partial** = live, but some colors, sizes or orders can't be sourced. **Blocked** = no supplier for the open orders. **Drafted** = off the store.

## Products

- [products/veylan-pullover.md](products/veylan-pullover.md)
- [products/kian-rivet-short.md](products/kian-rivet-short.md)
- [products/freya-zip-pullover.md](products/freya-zip-pullover.md)
- [products/camille-knit-sweater.md](products/camille-knit-sweater.md)
- [products/denver-knit-pullover.md](products/denver-knit-pullover.md)
- [products/milo-lattice-polo.md](products/milo-lattice-polo.md)
- [products/willa-crop-jacket.md](products/willa-crop-jacket.md)
- [products/maris-drape-sweater.md](products/maris-drape-sweater.md)
- [products/enzo-button-knit.md](products/enzo-button-knit.md)
- [products/elisa-flat-loafers.md](products/elisa-flat-loafers.md)
- [products/leif-stripe-trouser.md](products/leif-stripe-trouser.md)
- [products/linnea-pearl-top.md](products/linnea-pearl-top.md)
- [products/milan-leopard-dress.md](products/milan-leopard-dress.md)

## Source tags

| Tag | Where |
|---|---|
| `#08 MM-DD` | Slack `#08-cherry-beehive` |
| `#00 MM-DD` | Slack `#00-kevin-leandro-ops` |
| `#04 MM-DD` | Slack `#04-ops-alerts` (daily digests, Flow alerts, delay monitor) |
| `DM K/L MM-DD` | Slack DM Kevin ↔ Leandro |
| `Abby report 10-16` | Abby's Supplier Availability and Fulfillment Report in `#00` (posted 10-15 10:12 PM CT) |
| `WA Hart–Wio 1` | WhatsApp "Hart – Wio supplier 1" |
| `WA Hart private` | WhatsApp "Hart – Private communication" |
| `WA Lay` | WhatsApp Lay chat |
| `PLW r###` | Sheet "E&F - PLW & Quotation", tab `PLW`, row ### |
| `Quote Sep r##` | Same sheet, tab `September` (Cherry quotes), row ## |
| `Shopify 10-18` | Shopify Admin API read, 2026-10-18 ~4:20 PM CT |
| `Shopify 10-20` | Shopify Admin API + analytics read, 2026-10-20 ~10:15 AM CT |
| `Shopify 10-23` | Shopify Admin API + analytics read, 2026-10-23 ~10:25 AM CT |
| `Shopify 10-22` | Shopify Admin API + analytics read, 2026-10-22 ~10:25 AM CT |
| `Shopify 10-21` | Shopify Admin API + analytics read, 2026-10-21 ~10:20 AM CT |
| `Meta 10-23` | Meta Ads read-only, account act_731553569252529, last 30 days and 10-20 to 10-22, read 2026-10-23 |
| `Meta 10-22` | Meta Ads read-only, account act_731553569252529, last 30 days and 10-19 to 10-21, read 2026-10-22 |
| `Meta 10-21` | Meta Ads read-only, account act_731553569252529, last 30 days and 10-18 to 10-20, read 2026-10-21 |
| `Meta 10-20` | Meta Ads read-only, account act_731553569252529, last 30 days and 10-17 to 10-19, read 2026-10-20 |
| `Kevin 10-18` | Kevin told the ops agent directly in chat on 10-18 |
| `brief` | From the request brief. Not re-found in Slack or Shopify |

WhatsApp tags come from what was read earlier today. I did not re-open WhatsApp for this draft.
