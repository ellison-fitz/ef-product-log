# ef-product-log

Product sourcing log for Ellison & Fitz

**Brand:** Ellison & Fitz  
**Lane:** Backend ops / sourcing  
**Status:** Repo `ellison-fitz/ef-product-log`. Kept separate from `ef-sops` (this log has supplier names and costs).  
**Not for:** VA customer-support pages. CS truth stays on the [live SOP](https://kevinc710.github.io/ef-sops/). Ops how stays in [ops/](https://kevinc710.github.io/ef-sops/ops/).

This file is the current state of every product we are moving between suppliers. Each product page has the current facts at the top and a dated log underneath, newest first. Rewrite the top block in place when a fact changes. Do not stack "Updated" footnotes: put the date in the log.

Site: index.md + products/ render via GitHub Pages (Jekyll). Each product page now has a **Scale read** row (30-day units and trend, margin vs supplier cost, supplier reliability, Meta).

Snapshot taken Tue 2026-10-20, ~10:15 AM CT. Shopify reads (status, price, buyable colors, open orders) are from the Admin API at that time. 30-day sales are Shopify analytics net units for 2026-09-20 to 2026-10-20, with the prior 30 days and last 7 vs prior 7 days for trend. Meta is read-only from ad set names (product name is in the ad set or campaign name), last 30 days and 10-17 to 10-19, using Meta-reported purchases and ROAS. The "35 / 1.53" style numbers in ad set names are copied as written; 1.53 is read as the break-even ROAS. Slack and WhatsApp were not re-read for this refresh.

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
| [Maris Drape Sweater](products/maris-drape-sweater.md) | Cherry. Hart pitched | $17.41 Cherry (PLW) vs $20.30 Hart landed | 8 colors, XS–5XL | Live | 12 (19 units), normal Cherry flow | 331 (7d 116 vs 83, up) · On, ROAS 1.60 30d / 1.50 last 3d | Scale product. ~$32.58 margin. Watch ROAS vs 1.53 | Finish Cherry vs Hart comparison | Kevin |
| [Enzo Button Knit](products/enzo-button-knit.md) | Cherry. Hart pitched | $14.76 Cherry (PLW) vs $14.40 Hart landed | Olive, Coffee, Black (2 listings) | Live | 11941, 11942 (CL, possible duplicate), 12007, 12013 | 61 (7d 44 vs 17, up) · On, ROAS 1.74 V2 | **Scale candidate.** ~$25.23 margin | Finish Cherry vs Hart comparison. Check 11941/11942 duplicate | Kevin |
| [Camille Knit Sweater](products/camille-knit-sweater.md) | Lay (only source) | unknown | Coffee, Apricot, White, Black (Emerald, Burgundy off) | Partial | 11831 (Emerald S), 11996 (Coffee L). 5 Lay orders still on old 10-10 tracking | 23 (7d 9 vs 14) · On, ROAS 1.70 30d / 0.56 last 3d | Traction, but supply-blocked (Lay only, cost unknown) | Lay ships the 5 + tells us her 4 colors. 11831 color swap or refund | Abby (Lay) |
| [Freya Zip Pullover](products/freya-zip-pullover.md) | Cherry (1688 colors). Lay/Hart asked for Temu colors | $18.91 US 1pc (Cherry quote) | Camel, Navy, Olive, Pink (Butter, Grey off) | Partial | 11798, 11832, 11868, 11874, 11888, 11893, 11903, 11934 | 15 (7d 13 vs 2, up) · On, ROAS 1.23 30d / 0.72 last 3d | Demand yes, but 6 of 8 open orders unmatchable and ROAS under 1.46 | Abby: Butter/Grey buyers switch or refund. Check 11896 (Grey L) that shipped 10-19 | Abby |
| [Denver Knit Pullover](products/denver-knit-pullover.md) | Cherry (new cream version) | $9.36/unit bulk ex-shipping. Sample price "very high", exact unknown | Cream only (still buyable) | Partial | 12003, 12005, 12010, 12015. Sample-run orders now tracked | 13 (all in last 7d) · On again, ROAS 1.43, CPA ~$38 | Not yet: ~1.9/day vs Axel's 5+/day at ≤ $21 CPA | Hold the 250 bulk. Decide whether Cream should still be buyable while ads run | Kevin |
| [Milan Leopard Dress](products/milan-leopard-dress.md) | Cherry | $23.40 (PLW) | Navy, Sky | Partial | 11556 (1 Navy S, 19 days) | 33 (7d 1 vs 2, down) · Nearly off, ROAS 1.55 30d | Cooled off. Not a scale call now | Find out why Cherry is holding 11556 | Abby |
| [Milo Lattice Polo](products/milo-lattice-polo.md) | Cherry (no Emerald) | $14.14 (PLW) | 6 colors (Emerald off) | Partial | 11873 (item removed, $49.08 paid, $0 refunded) | 0 · Test ad set, ~$3 | No traction | Confirm 11873 refund | Abby |
| [Willa Crop Jacket](products/willa-crop-jacket.md) | Cherry (no Orange). Hart max size L | $18.60 (PLW) | Cream, Red, Orange still buyable | Partial | 11807 (Orange XL + Red XL, 8 days) | 3 (0 in 7d) · Off (ad set paused) | No traction | Ads are off, so draft (Leandro/Kevin). Offer 11807 L or refund | Leandro, Abby |
| [Veylan Pullover](products/veylan-pullover.md) | Hart (alt style). Cherry discontinued | $13.30 Hart alt | Black, White (S–3XL on listing; Hart is M–3XL) | Partial | none. All 10 orders show updated tracking 10-19/10-20. 10791 Veylan refunded | 5 (0 in 7d) · Off | Not a candidate | Watch the new tracking move | Kevin |
| [Kian Rivet Short](products/kian-rivet-short.md) | Hart (US-shipped alt). Cherry discontinued | $25.50–$28.70 each | Grey, Black (listing Unlisted) | Drafted | none | −1 net (0 orders) · Off | Not a candidate | Keep Unlisted | Kevin |
| [Elisa Flat Loafers](products/elisa-flat-loafers.md) | unknown | unknown | none (Draft) | Drafted | none | 4 (pre-draft) · none | Parked for GMC | Bring back with clean photos after GMC review clears | Kevin, Leandro |
| [Leif Stripe Trouser](products/leif-stripe-trouser.md) | none. Cherry has no exact match | $19.34 (PLW) | Khaki (listing still Active) | Blocked | none | 0 net · Off | Not a candidate | Decide whether to draft the listing | Kevin, Leandro |
| [Linnea Pearl Top](products/linnea-pearl-top.md) | unknown (Cherry pointed to Lay) | $15.87 (PLW) | Black, Light Cyan, Peach, Cream | Blocked | 11661 (14 days) | 1 net · Off | Not a candidate | Confirm with Lay or refund | Abby |

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
| `Meta 10-20` | Meta Ads read-only, account act_731553569252529, last 30 days and 10-17 to 10-19, read 2026-10-20 |
| `Kevin 10-18` | Kevin told the ops agent directly in chat on 10-18 |
| `brief` | From the request brief. Not re-found in Slack or Shopify |

WhatsApp tags come from what was read earlier today. I did not re-open WhatsApp for this draft.
