# ef-product-log

Product sourcing log for Ellison & Fitz

**Brand:** Ellison & Fitz  
**Lane:** Backend ops / sourcing  
**Status:** Repo `ellison-fitz/ef-product-log`. Kept separate from `ef-sops` (this log has supplier names and costs).  
**Not for:** VA customer-support pages. CS truth stays on the [live SOP](https://kevinc710.github.io/ef-sops/). Ops how stays in [ops/](https://kevinc710.github.io/ef-sops/ops/).

This file is the current state of every product we are moving between suppliers. Each product page has the current facts at the top and a dated log underneath, newest first. Rewrite the top block in place when a fact changes. Do not stack "Updated" footnotes: put the date in the log.

Site: index.md + products/ render via GitHub Pages (Jekyll). Each product page now has a **Scale read** row (30-day units and trend, margin vs supplier cost, supplier reliability, Meta).

Snapshot taken Wed 2026-11-11, ~10:30 AM CT. Shopify reads (status, price, buyable colors, open orders) are from the Admin API at that time; open orders are a full sweep of open unfulfilled/partial orders since 09-25 (counted as orders and units). 30-day sales are Shopify analytics net units (run-analytics-query) for 2026-10-13 to 2026-11-11 (today partial); last 7 days (11-05 to 11-11) vs prior 7 days (10-29 to 11-04) for trend. Analytics nets out returns, so it can read a little under the order count. **Meta was NOT re-read this run:** Pipeboard Free weekly AI tool limit is exceeded (100 of 30) and resets 2026-11-16, so every Meta number below is carried forward from `Meta 11-10`. Slack and WhatsApp were not re-read. **Highlights vs 11-10 (nothing new blocked, nothing urgent new):** Maris weekly units **40 vs 16** (up from 36 vs 23), 281 in 30d, 20 open (oldest 12428, 8 days); main campaign last seen off since 10-30. Enzo weekly **30 vs 16** (up), 147 in 30d, 20 open (was 18); still a scale candidate (last Meta read 7d 2.10, 30d 2.06, 3d 1.59). Maren **1 vs 8**, still flat. Denver **-1 vs 3**, 12435 cleared (no open orders). Freya 12472 cleared, **5 open**, oldest 11832 now 29 days. Camille has a **new open order 12769** (Apricot L, 11-10). Beck 11943 **25 days**; Linnea 11661 **36 days**. Not tracked here yet: **Faye Brushed Pullover** ($39.99, 9 colors, Active; 280 net units 30d, **163 in the last 7 days** vs 116; 112 open orders / 186 units, oldest 12421 on 11-03 (8 days), all paid except 12680 partly refunded; supplier/cost not in this log; Meta last read 3d ROAS 1.33, 7d 1.68), Orso Animal Bag ($54.99; 221 units 30d, 96 in 7d vs 89; 63 open orders / 81 units, oldest 11-05; Meta last read 7d 1.65, 30d 1.56), Bram Rib Cardigan ($59.99; 65 units 30d, 20 in 7d vs 17; 11 open orders / 14 units, oldest 11-06; Meta last read 7d 1.91, 30d 2.27), Brielle Bow Pullover (**listing still Draft**, $39.99; 5 units 30d; 4 paid open orders 12078, 12079, 12214, 12301, oldest ~20 days).

## Sourcing gaps

As of 2026-10-28, Maren row updated 2026-10-31. Rechecked 2026-11-11: no change on Sage/Terracotta confirmation (still shipped 10-30, supplier not recorded). Freya now 5 open (oldest 11832, 29 days; 12472 cleared).

| Product | Gap | Who said no | Next |
|---|---|---|---|
| [Maren Lantern Pullover](products/maren-lantern-pullover.md) | Sage Green and Brick/Terracotta. All 22 backlog orders with them marked shipped 10-30 (YT tracking), supplier not recorded (10-31). | Lay: not available (10-28) | Confirm who shipped, cost, and that the colors match |
| [Beck Waffle Polo](products/beck-waffle-polo.md) | Light Blue, Light Green, Mustard (M, order 11943) | Lay: not available (10-28) | Ask Hart, then Cherry |
| [Camille Knit Sweater](products/camille-knit-sweater.md) | Colors beyond Black/Apricot (11686 Burgundy L, 11756 White S) | Cherry: only Black/Apricot (10-27). Hart: no (10-11) | Lay to confirm her 4 colors |
| [Freya Zip Pullover](products/freya-zip-pullover.md) | Temu colors (Butter, Grey, Olive, Pink); 11868 refunded; 12472 Grey S cleared 11-11 | see page | Abby: switch or refund |
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
| [Maris Drape Sweater](products/maris-drape-sweater.md) | Cherry. Hart pitched | $17.41 Cherry (PLW) vs $20.30 Hart landed | 8 colors, XS–5XL | Live | 20 open (12428–12773), oldest 8 days | 281 (7d 40 vs 16, up) · Meta 11-10 (not re-read 11-11): main campaign still $0 (off since 10-30), Stack Testing 3d ROAS 1.74 on $345, 7d 2.06 | Scale product on 30d, weekly up (40 vs 16) with main campaign last seen off. ~$32.58 margin | Kevin: decide whether to turn the main campaign back on. Finish Cherry vs Hart comparison | Kevin |
| [Enzo Button Knit](products/enzo-button-knit.md) | Cherry. Hart pitched | $14.76 Cherry (PLW) vs $14.40 Hart landed | Olive, Coffee, Black (2 listings; `enzo-button-knit` $49.99, `enzo-knit` $39.99) | Live | 20 open (12431–12770), oldest 8 days | 147 across both (7d 30 vs 16, up) · Meta 11-10 (not re-read 11-11): 3d ROAS 1.59 on $452 (9 purchases), 7d 2.10, 30d 2.06, CBO shared with Orso | Scale candidate, holding: weekly up (30 vs 16), 7d/30d ROAS above 1.49 at last read, 3d cooled from 3.72. ~$35.23 margin at $49.99 | Kevin decides whether to give Enzo its own budget. Check whether 11941/11942 needs a refund | Kevin |
| [Maren Lantern Pullover](products/maren-lantern-pullover.md) | unknown. Sage/Terracotta backlog shipped 10-30 (supplier not recorded) | unknown | 6 colors, XS–5XL, all buyable | Partial | 12646 (Sky Blue XL, 4 days) | 50 (7d 1 vs 8) · Meta 11-10: $0 in 7d (stopped) | Not a scale call: weekly flatlined (1 vs 8), cost unknown | Confirm who shipped Sage/Terracotta, cost and color match | Kevin |
| [Beck Waffle Polo](products/beck-waffle-polo.md) | unknown. Lay no on Light Blue/Light Green/Mustard | unknown | 10 colors, S–4XL, all buyable | Blocked | 11943 (Light Blue, Light Green, Mustard M, **25 days**) | 3 (one order) · Meta 11-10: 7d $7 / 0, 30d $25 / 1 purchase | Not a candidate | Ask Hart, then Cherry. Else exchange or store credit | Kevin, Abby |
| [Camille Knit Sweater](products/camille-knit-sweater.md) | Lay (again). Cherry Black/Apricot only | unknown | Coffee, Apricot, White, Black (Emerald, Burgundy off) | Partial | 12769 (Apricot L, new 11-10, 1 day) | 17 (7d 1 vs 0) · Meta 11-10: 7d $8 / 0, 30d ~$548 / ROAS ~1.8 | Strong prior ROAS, supply-blocked (Lay only, cost unknown) | Kevin asks Lay her colors, price, lead time; confirm 11686/11756 went to Lay | Kevin, Abby |
| [Freya Zip Pullover](products/freya-zip-pullover.md) | Cherry (1688 colors). Lay/Hart asked for Temu colors | $18.91 US 1pc (Cherry quote) | Temu listing: Camel, Navy only (Butter, Grey, Olive, Pink off). 1688 listing `freya-pullover`: 8 colors | Partial | 11832, 11874, 11888, 11893, 11934 (oldest 29 days) | 14 (7d 0 vs 0) · Meta 11-10: $0 in 7d; 30d ROAS ~1.3 | No: most open orders unmatchable on Temu listing, no sales in 7d | Abby: Butter/Grey buyers switch or refund. Ship 11832 (Navy S, 29 days) | Abby |
| [Denver Knit Pullover](products/denver-knit-pullover.md) | Cherry (new cream version) | $9.36/unit bulk ex-shipping. Sample price "very high", exact unknown | Cream only (Grey/Black off) | Partial | none (12435 cleared) | 29 (7d -1 vs 3) · Meta 11-10: main campaign off, 30d ROAS 1.04; test ad set $43 / 0 in 7d | No: weekly 0, far off Axel's 5+/day at ≤ $21 CPA | Hold the 250 bulk | Kevin |
| [Milan Leopard Dress](products/milan-leopard-dress.md) | Cherry | $23.40 (PLW) | Navy, Sky | Partial | none | -1 net in 30d, 0 in 7d · Meta 11-10: 30d ~$26 / 0, no 7d spend | Cooled off. Not a scale call now | Confirm the 11556 customer knows only one dress shipped | Abby |
| [Milo Lattice Polo](products/milo-lattice-polo.md) | Cherry (no Emerald) | $14.14 (PLW) | 6 colors (Emerald off) | Partial | none | 0 · Meta 11-10: 30d ~$5 / 0 | No traction | none | Abby |
| [Willa Crop Jacket](products/willa-crop-jacket.md) | Cherry (no Orange). Hart max size L | $18.60 (PLW) | Cream, Red, Orange still buyable | Partial | none. 11807 refunded $96.13 (settled) | 0 · Meta 11-10: no spend (ad set off) | No traction | Ads are off, so draft (Leandro/Kevin) | Leandro |
| [Veylan Pullover](products/veylan-pullover.md) | Hart (alt style). Cherry discontinued | $13.30 Hart alt | Black, White (S–3XL on listing; Hart is M–3XL) | Partial | none | 0 · Meta 11-10: off | Not a candidate | Watch the new tracking move | Kevin |
| [Kian Rivet Short](products/kian-rivet-short.md) | Hart (US-shipped alt). Cherry discontinued | $25.50–$28.70 each | Grey, Black (listing Unlisted) | Drafted | none | 0 · Meta 11-10: off | Not a candidate | Keep Unlisted | Kevin |
| [Elisa Flat Loafers](products/elisa-flat-loafers.md) | unknown | unknown | none (Draft) | Drafted | none | 0 · none (checked 11-11) | Parked for GMC | Bring back with clean photos after GMC review clears | Kevin, Leandro |
| [Leif Stripe Trouser](products/leif-stripe-trouser.md) | none. Cherry has no exact match | $19.34 (PLW) | Khaki (listing still Active) | Blocked | none | 0 · Meta 11-10: off, ~$1 in 30d | Not a candidate | Decide whether to draft the listing | Kevin, Leandro |
| [Linnea Pearl Top](products/linnea-pearl-top.md) | unknown (Cherry pointed to Lay) | $15.87 (PLW) | Black, Light Cyan, Peach, Cream | Blocked | 11661 (**36 days**) | 0 · Meta 11-10: off | Not a candidate | Confirm with Lay or refund | Abby |

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
| `Shopify 11-11` | Shopify Admin API read (products + variants availability + full open unfulfilled/partial order sweep since 09-25) plus analytics net units (run-analytics-query, 10-13 to 11-11, 11-05 to 11-11, 10-29 to 11-04), 2026-11-11 ~10:30 AM CT |
| `Meta 11-11` | **Not read.** Pipeboard Free weekly AI tool limit exceeded (100 of 30); resets 2026-11-16. Carry-forward from `Meta 11-10`. |
| `Shopify 11-10` | Shopify Admin API read (products + variants availability + full open unfulfilled/partial order sweep since 09-25) plus analytics net units (run-analytics-query, 10-12 to 11-10, 11-04 to 11-10, 10-28 to 11-03), 2026-11-10 ~10:05 AM CT |
| `Meta 11-10` | Meta Ads read-only, account act_731553569252529, ad set insights 10-12 to 11-10, 11-04 to 11-10 and 11-07 to 11-09, read 2026-11-10 ~10:05 AM CT. |
| `Shopify 11-09` | Shopify Admin API read (products + variants availability + full open unfulfilled/partial order sweep since 09-25) plus analytics net units (run-analytics-query, 10-11 to 11-09, 11-03 to 11-09, 10-27 to 11-02), 2026-11-09 ~10:20 AM CT |
| `Shopify 11-08` | Shopify Admin API read (products + full open unfulfilled/partial order sweep since 09-25) plus analytics net units (run-analytics-query, 10-10 to 11-08, 11-02 to 11-08, 10-26 to 11-01), 2026-11-08 ~10:15 AM CT |
| `Shopify 11-07` | Shopify Admin API read (products + unfulfilled orders) plus analytics net units (run-analytics-query, 10-09 to 11-07, 11-01 to 11-07, 10-25 to 10-31), 2026-11-07 ~10:00 AM CT |
| `Shopify 11-03` | Shopify Admin API read (products + orders 10-05 to 11-03) plus analytics net units (run-analytics-query, 10-05 to 11-03, 10-28 to 11-03, 10-21 to 10-27), 2026-11-03 ~10:10 AM CT |
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
| `Meta 11-09` | Meta Ads read-only, account act_731553569252529, campaign and ad set insights 10-11 to 11-09, 11-03 to 11-09 and 11-06 to 11-08, plus daily campaign spend 11-03 to 11-09, read 2026-11-09 ~10:20 AM CT (Pipeboard limit cleared). |
| `Meta 11-08` | **Not read.** Pipeboard Free weekly AI tool limit still exceeded (31/30); resets 2026-11-09 00:00 UTC (11-08 ~6 PM CT). Carry-forward from `Meta 11-03`. |
| `Meta 11-07` | **Not read.** Pipeboard Free weekly AI tool limit exceeded (31/30); resets 2026-11-09. Carry-forward from `Meta 11-03`. |
| `Meta 11-03` | Meta Ads read-only, account act_731553569252529, 10-04 to 11-02, 10-27 to 11-02 and 10-31 to 11-02, plus daily spend 11-02 and 11-03, read 2026-11-03 |
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
