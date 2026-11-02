# ef-product-log

Product sourcing log for Ellison & Fitz

**Brand:** Ellison & Fitz  
**Lane:** Backend ops / sourcing  
**Status:** Repo `ellison-fitz/ef-product-log`. Kept separate from `ef-sops` (this log has supplier names and costs).  
**Not for:** VA customer-support pages. CS truth stays on the [live SOP](https://kevinc710.github.io/ef-sops/). Ops how stays in [ops/](https://kevinc710.github.io/ef-sops/ops/).

This file is the current state of every product we are moving between suppliers. Each product page has the current facts at the top and a dated log underneath, newest first. Rewrite the top block in place when a fact changes. Do not stack "Updated" footnotes: put the date in the log.

Site: index.md + products/ render via GitHub Pages (Jekyll). Each product page now has a **Scale read** row (30-day units and trend, margin vs supplier cost, supplier reliability, Meta).

Snapshot taken Mon 2026-11-02, ~10:20 AM CT. Shopify reads (status, price, buyable colors, open orders) are from the Admin API at that time. 30-day sales are counted from Shopify orders (current quantities, cancelled orders excluded) for 2026-10-04 to 2026-11-02 (today partial), with last 7 days (10-27 to 11-02) vs prior 7 days (10-20 to 10-26) for trend. Meta is read-only from ad set names and spend, last 30 days (10-03 to 11-01), 10-26 to 11-01 (7d) and 10-30 to 11-01 (3d), using Meta-reported purchases and ROAS, plus daily spend for 11-01 and 11-02. The "35 / 1.53" style numbers in ad set names are copied as written; 1.53 is read as the break-even ROAS. Slack and WhatsApp were not re-read for this refresh. **Meta: the main Maris and Denver ad sets are still at $0 (11-01 and today). Maren's ad set also spent $0 on 11-01 and today, so its losing spend has stopped.** The CBO Creative Testing campaign keeps budget on Orso ($348 on 11-01), so Enzo got $33 (0 purchases; 3d 0 purchases on $82). Not tracked here yet: **Faye Brushed Pullover is taking off** (21 units 30d, 20 of them in the last 7 days vs 1; Stack Testing ad set 3d ROAS 5.65 on $92 vs its 1.4, $70 on 11-01 at 5.90; 20 open line items across 12 orders, all 10-31 or later; supplier and cost not in this log). Bram Rib Cardigan (42 units 30d, 16 in 7d vs 14; 3d ROAS 4.86 on $78, 7d 2.90, 30d 2.68; 4 open), Orso Animal Bag (107 units 30d, 45 in 7d vs 8; 3d ROAS 1.55 on $894, 11-01 1.24 on $348, still the biggest spender; 14 open, 2 on hold), Brielle Bow Pullover (3d $17, 0 purchases; 4 open incl. 12078/12079 from 10-22).

## Sourcing gaps

As of 2026-10-28, Maren row updated 2026-10-31. Rechecked 2026-11-02: no change.

| Product | Gap | Who said no | Next |
|---|---|---|---|
| [Maren Lantern Pullover](products/maren-lantern-pullover.md) | Sage Green and Brick/Terracotta. All 22 backlog orders with them marked shipped 10-30 (YT tracking), supplier not recorded (10-31). | Lay: not available (10-28) | Confirm who shipped, cost, and that the colors match |
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
| [Maris Drape Sweater](products/maris-drape-sweater.md) | Cherry. Hart pitched | $17.41 Cherry (PLW) vs $20.30 Hart landed | 8 colors, XS–5XL | Live | 12366, 12368 (11-01), 12380 (today) | 346 (7d 44 vs 89, down) · **Main campaign still off**; Stack Testing ad set $122 on 11-01 at 1.46. ROAS 1.57 30d / 1.43 7d / 1.00 last 3d | Scale product. ~$32.58 margin. Fourth 3d read under 1.53. Main campaign off since 10-30, weekly units halved | Kevin: confirm the pause was intended. Finish Cherry vs Hart comparison | Kevin |
| [Enzo Button Knit](products/enzo-button-knit.md) | Cherry. Hart pitched | $14.76 Cherry (PLW) vs $14.40 Hart landed | Olive, Coffee, Black (2 listings; `enzo-button-knit` $49.99, `enzo-knit` $39.99) | Live | 12340, 12375, 12376. 11941 + 11942 on one tracking, both still fully paid | 125 across both (7d 30 vs 34, flat) · On, but $33 on 11-01 (0 purchases). ROAS 1.97 30d / 2.73 7d / 0 purchases last 3d ($82) | Scale candidate, on watch, weakening. ~$35.23 margin at $49.99. Second 3d read under 1.49, both on tiny spend. CBO budget stays on Orso | Kevin decides whether to give Enzo its own budget. Check whether 11941/11942 needs a refund | Kevin |
| [Maren Lantern Pullover](products/maren-lantern-pullover.md) | unknown. Sage/Terracotta backlog shipped 10-30 (supplier not recorded) | unknown | 6 colors, XS–5XL, all buyable | Partial | 12338 | 49 (7d 16 vs 33, down) · **Stopped spending** ($0 on 11-01 and today). ROAS 0.64 last 3d on $346, 1.08 7d, 1.40 30d | Not a scale call: fourth 3d read under 1.5, 7d and 30d under too. Cost unknown | Confirm who shipped Sage/Terracotta, cost and color match | Kevin |
| [Beck Waffle Polo](products/beck-waffle-polo.md) | unknown. Lay no on Light Blue/Light Green/Mustard | unknown | 10 colors, S–4XL, all buyable | Blocked | 11943 (Light Blue, Light Green, Mustard M, 16 days) | 3 (one order) · small test, $2 last 3d | Not a candidate | Ask Hart, then Cherry. Else exchange or store credit | Kevin, Abby |
| [Camille Knit Sweater](products/camille-knit-sweater.md) | Lay (again for 11686, 11756). Cherry Black/Apricot only | unknown | Coffee, Apricot, White, Black (Emerald, Burgundy off) | Partial | none. 5 Lay orders on old 10-10 tracking (last checked 10-31) | 30 (7d 0 vs 8, stopped) · Nearly off ($2 last 3d), ROAS 2.00 30d | Strong ROAS, but supply-blocked (Lay only, cost unknown) | Kevin asks Lay her colors, price, lead time. Then Abby sends 11686, 11756 to Lay | Kevin, Abby |
| [Freya Zip Pullover](products/freya-zip-pullover.md) | Cherry (1688 colors). Lay/Hart asked for Temu colors | $18.91 US 1pc (Cherry quote) | Temu listing: Camel, Navy only (Butter, Grey, Olive, Pink off). 1688 listing `freya-pullover`: 8 colors | Partial | 11798, 11832, 11868, 11874, 11888, 11893, 11934 (oldest 21 days) | 15 (7d 0 vs 1, stopped) · Off ($0 last 7d), ROAS 1.18 30d | No: 5 of 7 open orders unmatchable, 11893 has Olive (off), 30d ROAS under 1.46, no sales in 7d | Abby: Butter/Grey buyers switch or refund. Check Olive for 11893. Ship 11832 (Navy S, 20 days) | Abby |
| [Denver Knit Pullover](products/denver-knit-pullover.md) | Cherry (new cream version) | $9.36/unit bulk ex-shipping. Sample price "very high", exact unknown | Cream only (still buyable) | Partial | none | 29 (7d 3 vs 13, down) · **Main campaign still off**; 40 / 1.75 test ad set ($20 total). ROAS 1.15 30d / 1.21 7d | No: 7d and 30d under 1.47, far off Axel's 5+/day at ≤ $21 CPA | Hold the 250 bulk | Kevin |
| [Milan Leopard Dress](products/milan-leopard-dress.md) | Cherry | $23.40 (PLW) | Navy, Sky | Partial | none | 3 (0 in 7d) · Off, ROAS 0.80 30d | Cooled off. Not a scale call now | Confirm the 11556 customer knows only one dress shipped | Abby |
| [Milo Lattice Polo](products/milo-lattice-polo.md) | Cherry (no Emerald) | $14.14 (PLW) | 6 colors (Emerald off) | Partial | none | 0 · Test ad set, $0 last 3d | No traction | none | Abby |
| [Willa Crop Jacket](products/willa-crop-jacket.md) | Cherry (no Orange). Hart max size L | $18.60 (PLW) | Cream, Red, Orange still buyable | Partial | none. 11807 refunded $96.13 (now settled) | 0 · Off (ad set paused) | No traction | Ads are off, so draft (Leandro/Kevin) | Leandro |
| [Veylan Pullover](products/veylan-pullover.md) | Hart (alt style). Cherry discontinued | $13.30 Hart alt | Black, White (S–3XL on listing; Hart is M–3XL) | Partial | none | 0 · Off | Not a candidate | Watch the new tracking move | Kevin |
| [Kian Rivet Short](products/kian-rivet-short.md) | Hart (US-shipped alt). Cherry discontinued | $25.50–$28.70 each | Grey, Black (listing Unlisted) | Drafted | none | 0 · Off | Not a candidate | Keep Unlisted | Kevin |
| [Elisa Flat Loafers](products/elisa-flat-loafers.md) | unknown | unknown | none (Draft) | Drafted | none | 1 (pre-draft) · none | Parked for GMC | Bring back with clean photos after GMC review clears | Kevin, Leandro |
| [Leif Stripe Trouser](products/leif-stripe-trouser.md) | none. Cherry has no exact match | $19.34 (PLW) | Khaki (listing still Active) | Blocked | none | 0 · Off | Not a candidate | Decide whether to draft the listing | Kevin, Leandro |
| [Linnea Pearl Top](products/linnea-pearl-top.md) | unknown (Cherry pointed to Lay) | $15.87 (PLW) | Black, Light Cyan, Peach, Cream | Blocked | 11661 (27 days) | 1 · Off | Not a candidate | Confirm with Lay or refund | Abby |

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
| `Shopify 11-02` | Shopify Admin API read (products + orders 10-04 to 11-02), 2026-11-02 ~10:10 AM CT |
| `Shopify 11-01` | Shopify Admin API read (products + orders 10-03 to 11-01), 2026-11-01 ~10:15 AM CT |
| `Shopify 10-31` | Shopify Admin API + analytics read, 2026-10-31 ~10:20 AM CT |
| `Shopify 10-29` | Shopify Admin API + analytics read, 2026-10-29 ~10:25 AM CT |
| `Shopify 10-28` | Shopify Admin API + analytics read, 2026-10-28 ~10:10 AM CT |
| `Shopify 10-27` | Shopify Admin API + analytics read, 2026-10-27 ~10:35 AM CT |
| `Shopify 10-26` | Shopify Admin API + analytics read, 2026-10-26 ~10:30 AM CT |
| `Shopify 10-24` | Shopify Admin API + analytics read, 2026-10-24 ~10:10 AM CT |
| `Shopify 10-23` | Shopify Admin API + analytics read, 2026-10-23 ~10:25 AM CT |
| `Shopify 10-22` | Shopify Admin API + analytics read, 2026-10-22 ~10:25 AM CT |
| `Shopify 10-21` | Shopify Admin API + analytics read, 2026-10-21 ~10:20 AM CT |
| `Meta 11-02` | Meta Ads read-only, account act_731553569252529, 10-03 to 11-01, 10-26 to 11-01 and 10-30 to 11-01, plus daily spend 11-01 and 11-02, read 2026-11-02 |
| `Meta 11-01` | Meta Ads read-only, account act_731553569252529, last 30 days, 10-25 to 10-31 and 10-29 to 10-31, plus daily spend 10-31 and 11-01, read 2026-11-01 |
| `Meta 10-31` | Meta Ads read-only, account act_731553569252529, last 30 days, 10-24 to 10-30 and 10-28 to 10-30, plus campaign/ad set status, read 2026-10-31 |
| `Meta 10-29` | Meta Ads read-only, account act_731553569252529, last 30 days and 10-26 to 10-28, read 2026-10-29 |
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
