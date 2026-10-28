# ef-product-log

Product sourcing log for Ellison & Fitz

**Brand:** Ellison & Fitz  
**Lane:** Backend ops / sourcing  
**Status:** Repo `ellison-fitz/ef-product-log`. Kept separate from `ef-sops` (this log has supplier names and costs).  
**Not for:** VA customer-support pages. CS truth stays on the [live SOP](https://kevinc710.github.io/ef-sops/). Ops how stays in [ops/](https://kevinc710.github.io/ef-sops/ops/).

This file is the current state of every product we are moving between suppliers. Each product page has the current facts at the top and a dated log underneath, newest first. Rewrite the top block in place when a fact changes. Do not stack "Updated" footnotes: put the date in the log.

Site: index.md + products/ render via GitHub Pages (Jekyll). Each product page now has a **Scale read** row (30-day units and trend, margin vs supplier cost, supplier reliability, Meta).

Snapshot taken Wed 2026-10-28, ~10:10 AM CT. Shopify reads (status, price, buyable colors, open orders) are from the Admin API at that time. 30-day sales are Shopify analytics net units for 2026-09-28 to 2026-10-28 (today partial), with the prior 30 days and last 7 (10-22 to 10-28) vs prior 7 days (10-15 to 10-21) for trend. Meta is read-only from ad set and campaign names, last 30 days and 10-25 to 10-27, using Meta-reported purchases and ROAS. The "35 / 1.53" style numbers in ad set names are copied as written; 1.53 is read as the break-even ROAS. Slack and WhatsApp were not re-read for this refresh. Sourcing update 2026-10-28 ~1:20 PM CT: WhatsApp and Slack facts added for Camille, Maris, Enzo; Maren Lantern Pullover and Beck Waffle Polo pages added (Shopify re-read for both). Not tracked here yet at the 10:10 AM snapshot: Maren Lantern Pullover (40 units 30d, 39 in 7d vs 1; 3d ROAS 1.74 on $603 vs 1.5 in the ad set name, 30d 2.01; 20 orders unfulfilled, oldest 12065 from 10-21) and Bram Rib Cardigan (32 units 30d, 17 in 7d vs 9; 3d ROAS 2.10 on $263 vs 1.51, 30d 2.45; 12261 open from today).

## Sourcing gaps

As of 2026-10-28.

| Product | Gap | Who said no | Next |
|---|---|---|---|
| [Maren Lantern Pullover](products/maren-lantern-pullover.md) | Sage Green (match listing, not mint/olive) and Brick/Terracotta (not bright orange). All 20 open orders have one of them. | Lay: not available (10-28) | Ask Hart by name, then Cherry |
| [Beck Waffle Polo](products/beck-waffle-polo.md) | Light Blue, Light Green, Mustard (M, order 11943) | Lay: not available (10-28) | Ask Hart, then Cherry |
| [Camille Knit Sweater](products/camille-knit-sweater.md) | Colors beyond Black/Apricot (11686 Burgundy L, 11756 White S) | Cherry: only Black/Apricot (10-27). Hart: no (10-11) | Lay to confirm her 4 colors |
| [Freya Zip Pullover](products/freya-zip-pullover.md) | Temu colors (Butter, Grey, Olive, Pink) | see page | Abby: switch or refund |
| [Maris Drape Sweater](products/maris-drape-sweater.md) | Full color range from the better-fabric supplier | 50 unit MOQ per color | Decide after the replacement sample |

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
| [Maris Drape Sweater](products/maris-drape-sweater.md) | Cherry. Hart pitched | $17.41 Cherry (PLW) vs $20.30 Hart landed | 8 colors, XS–5XL | Live | none. 12222 shipped | 359 (7d 74 vs 120, down) · On, ROAS 1.55 30d / 1.61 last 3d | Scale product. ~$32.58 margin. Third 3d read over 1.53 (1.74, 1.56, 1.61), but OG 1.52 and Batch 2 1.39 | Finish Cherry vs Hart comparison. Watch OG and Batch 2 | Kevin |
| [Enzo Button Knit](products/enzo-button-knit.md) | Cherry. Hart pitched | $14.76 Cherry (PLW) vs $14.40 Hart landed | Olive, Coffee, Black (2 listings; `enzo-button-knit` now $49.99, `enzo-knit` $39.99) | Live | 9 orders from 10-27 on, normal. 11941 + 11942 on one tracking, both still fully paid | 115 (7d 48 vs 39, up) · On, ROAS 2.07 30d / 3.90 last 3d | Scale candidate. ~$35.23 margin at $49.99 (~$25.23 at $39.99). Fourth 3d read over 1.49 (3.90 at CPA ~$19), spend ~$100/day | Kevin decides whether to add spend. Watch conversion at $49.99. Check whether 11941/11942 needs a refund | Kevin |
| [Maren Lantern Pullover](products/maren-lantern-pullover.md) | unknown (non-gap colors shipping). Lay no on Sage/Terracotta. Hart asked | unknown | 6 colors, XS–5XL, all buyable | Partial | 20 unfulfilled, oldest 12065 (10-21), all have Sage Green or Terracotta | 40 (7d 39 vs 1, up) · On, ROAS 1.74 last 3d on $603 vs 1.5, 2.01 30d | Demand is there, but blocked on Sage Green and Terracotta | Source Sage + Terracotta (Hart, then Cherry) | Kevin |
| [Beck Waffle Polo](products/beck-waffle-polo.md) | unknown. Lay no on Light Blue/Light Green/Mustard | unknown | 10 colors, S–4XL, all buyable | Blocked | 11943 (Light Blue, Light Green, Mustard M, 11 days) | 3 (one order) · unknown | Not a candidate | Ask Hart, then Cherry. Else exchange or store credit | Kevin, Abby |
| [Camille Knit Sweater](products/camille-knit-sweater.md) | Lay (again for 11686, 11756). Cherry Black/Apricot only | unknown | Coffee, Apricot, White, Black (Emerald, Burgundy off) | Partial | none. 5 Lay orders still on old 10-10 tracking | 30 (7d 3 vs 9, down) · Nearly off ($2 last 3d), ROAS 2.01 30d | Strong ROAS, but supply-blocked (Lay only, cost unknown) | Kevin asks Lay her colors, price, lead time. Then Abby sends 11686, 11756 to Lay | Kevin, Abby |
| [Freya Zip Pullover](products/freya-zip-pullover.md) | Cherry (1688 colors). Lay/Hart asked for Temu colors | $18.91 US 1pc (Cherry quote) | Temu listing: Camel, Navy only (Butter, Grey, Olive, Pink off; Olive/Pink off since 10-26 night). 1688 listing `freya-pullover`: 8 colors | Partial | 11798, 11832, 11868, 11874, 11888, 11893, 11934 (12055 shipped) | 16 (7d 0 vs 13, stopped) · Off ($0 last 3d), ROAS 1.18 30d | No: 5 of 7 open orders unmatchable, 11893 has Olive (off), 30d ROAS under 1.46, no sales in 7d | Abby: Butter/Grey buyers switch or refund. Check Olive for 11893. Ship 11832 (Navy S, 14 days) | Abby |
| [Denver Knit Pullover](products/denver-knit-pullover.md) | Cherry (new cream version) | $9.36/unit bulk ex-shipping. Sample price "very high", exact unknown | Cream only (still buyable) | Partial | none | 26 (7d 11 vs 15, down) · On, ROAS 1.17 30d / 1.08 last 3d, CPA ~$69 | No: misses Axel's 5+/day at ≤ $21 CPA. 3d ROAS fell to 1.08, under 1.47 | Hold the 250 bulk. Watch how the $64.99 price converts | Kevin |
| [Milan Leopard Dress](products/milan-leopard-dress.md) | Cherry | $23.40 (PLW) | Navy, Sky | Partial | none | 10 (0 in 7d) · Off in practice, ROAS 1.17 30d | Cooled off. Not a scale call now | Confirm the 11556 customer knows only one dress shipped | Abby |
| [Milo Lattice Polo](products/milo-lattice-polo.md) | Cherry (no Emerald) | $14.14 (PLW) | 6 colors (Emerald off) | Partial | none | under 3 · Test ad set, ~$1 last 3d | No traction | none | Abby |
| [Willa Crop Jacket](products/willa-crop-jacket.md) | Cherry (no Orange). Hart max size L | $18.60 (PLW) | Cream, Red, Orange still buyable | Partial | 11807 (Orange XL + Red XL, 16 days) | 2 (0 in 7d) · Off (ad set paused) | No traction | Ads are off, so draft (Leandro/Kevin). Offer 11807 L or refund | Leandro, Abby |
| [Veylan Pullover](products/veylan-pullover.md) | Hart (alt style). Cherry discontinued | $13.30 Hart alt | Black, White (S–3XL on listing; Hart is M–3XL) | Partial | none | 2 (0 in 7d) · Off | Not a candidate | Watch the new tracking move | Kevin |
| [Kian Rivet Short](products/kian-rivet-short.md) | Hart (US-shipped alt). Cherry discontinued | $25.50–$28.70 each | Grey, Black (listing Unlisted) | Drafted | none | 0 · Off | Not a candidate | Keep Unlisted | Kevin |
| [Elisa Flat Loafers](products/elisa-flat-loafers.md) | unknown | unknown | none (Draft) | Drafted | none | 1 (pre-draft) · none | Parked for GMC | Bring back with clean photos after GMC review clears | Kevin, Leandro |
| [Leif Stripe Trouser](products/leif-stripe-trouser.md) | none. Cherry has no exact match | $19.34 (PLW) | Khaki (listing still Active) | Blocked | none | 0 net · Off | Not a candidate | Decide whether to draft the listing | Kevin, Leandro |
| [Linnea Pearl Top](products/linnea-pearl-top.md) | unknown (Cherry pointed to Lay) | $15.87 (PLW) | Black, Light Cyan, Peach, Cream | Blocked | 11661 (22 days) | under 3 · Off | Not a candidate | Confirm with Lay or refund | Abby |

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
- [products/maren-lantern-pullover.md](products/maren-lantern-pullover.md)
- [products/beck-waffle-polo.md](products/beck-waffle-polo.md)

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
| `Shopify 10-25` | Shopify Admin API + analytics read, 2026-10-25 ~10:20 AM CT |
| `Shopify 10-28` | Shopify Admin API + analytics read, 2026-10-28 ~10:10 AM CT |
| `Shopify 10-27` | Shopify Admin API + analytics read, 2026-10-27 ~10:35 AM CT |
| `Shopify 10-26` | Shopify Admin API + analytics read, 2026-10-26 ~10:30 AM CT |
| `Shopify 10-24` | Shopify Admin API + analytics read, 2026-10-24 ~10:10 AM CT |
| `Shopify 10-23` | Shopify Admin API + analytics read, 2026-10-23 ~10:25 AM CT |
| `Shopify 10-22` | Shopify Admin API + analytics read, 2026-10-22 ~10:25 AM CT |
| `Shopify 10-21` | Shopify Admin API + analytics read, 2026-10-21 ~10:20 AM CT |
| `Meta 10-28` | Meta Ads read-only, account act_731553569252529, last 30 days and 10-25 to 10-27, read 2026-10-28 |
| `Meta 10-27` | Meta Ads read-only, account act_731553569252529, last 30 days and 10-24 to 10-26, read 2026-10-27 |
| `Meta 10-26` | Meta Ads read-only, account act_731553569252529, last 30 days and 10-23 to 10-25, read 2026-10-26 |
| `Meta 10-25` | Meta Ads read-only, account act_731553569252529, last 30 days and 10-22 to 10-24, read 2026-10-25 |
| `Meta 10-24` | Meta Ads read-only, account act_731553569252529, last 30 days and 10-21 to 10-23, read 2026-10-24 |
| `Meta 10-23` | Meta Ads read-only, account act_731553569252529, last 30 days and 10-20 to 10-22, read 2026-10-23 |
| `Meta 10-22` | Meta Ads read-only, account act_731553569252529, last 30 days and 10-19 to 10-21, read 2026-10-22 |
| `Meta 10-21` | Meta Ads read-only, account act_731553569252529, last 30 days and 10-18 to 10-20, read 2026-10-21 |
| `Meta 10-20` | Meta Ads read-only, account act_731553569252529, last 30 days and 10-17 to 10-19, read 2026-10-20 |
| `Kevin 10-18` | Kevin told the ops agent directly in chat on 10-18 |
| `WA Lay MM-DD` / `WA Hart private MM-DD` | Same WhatsApp chats, with the message date |
| `brief` | From the request brief. Not re-found in Slack or Shopify |

WhatsApp tags come from what was read earlier today. The 2026-10-28 sourcing update used WhatsApp and Slack facts read that day.
