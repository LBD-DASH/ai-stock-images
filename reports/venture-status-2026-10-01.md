# Venture status report: ai-stock-images (1 Oct 2026)

Prepared: Thursday 1 Oct 2026, about 03:30 SAST, for Kevin Britz (via the CEO agent). Repo state read at commit `fbce2a6e51bc3ee271e2a54da1f16f0d1cce1a4c` (1 Oct 2026, 02:37 SAST). All dates and times are SAST (UTC+2). Estimates are marked **estimate**. Anything without a source says **unknown**.

## Summary

- The venture has earned nothing and spent nothing: no Contributor account, no generator, 0 images made, 0 submitted, 0 accepted ([logs/2026-10-01.md](../logs/2026-10-01.md), `assets/` holds only `.gitkeep`).
- Five days of planning are done (about 170 drafted prompts, a 10-prompt pilot shortlist, a ZA setup checklist), but nothing can be tested until Kevin opens the Adobe Stock Contributor account and approves tools.
- The tool cost in the logs (about R283/month) is out of date: it used a Firefly plan Adobe no longer sells. A like-for-like setup now costs about **R368/month (estimate)**, and "Firefly Premium" today is a US$199.99/month video plan, so do not approve it by name.
- Break-even on R368/month is about **23 downloads a month** at Adobe's own example royalty of US$0.99 per download (range 12 to 68).
- Recommendation: keep the venture alive only if Kevin clears the blockers by 31 Oct 2026. Then run a 30-image pilot and decide 90 days after the first accepted upload.

## Status with evidence

| Platform | Produced | Submitted | Accepted | Earnings | Source |
|---|---|---|---|---|---|
| Adobe Stock (only target platform) | 0 | 0 | 0 | None (no Contributor account exists) | [logs/2026-10-01.md](../logs/2026-10-01.md) ("no images generated, curated, upscaled or uploaded, for the fifth day running"), [logs/2026-09-28.md](../logs/2026-09-28.md) weekly review (all metrics unknown, no account) |
| Shutterstock, other sites | 0 | 0 | 0 | None (not targeted yet) | [README.md](../README.md) ("we ignore them at first") |
| Image files in repo | 0 | n/a | n/a | n/a | Repo tree at `fbce2a6`: `assets/` contains only `.gitkeep`; no images or output folders anywhere in the repo |
| Cash spent | R0 | n/a | n/a | n/a | [logs/2026-09-30.md](../logs/2026-09-30.md) ("no money spent"); no purchase recorded in any log |

Other metrics (acceptance rate, downloads, revenue per image): unknown, because nothing has been uploaded. Agent run cost of the daily routine: unknown (not recorded in the repo).

## Work done so far

| Date | Work | Source |
|---|---|---|
| Sat 27 Sep (Day 1) | Repo scaffold, do-not-generate list, 36 prompts (holiday copy-space, Q1 business planning, abstract textures), live Adobe Stock saturation check, generator and upscaler comparison, Adobe generative AI rules summary | [logs/2026-09-27.md](../logs/2026-09-27.md), [from-cto-new/theme-validation-2026-09-27.md](../from-cto-new/theme-validation-2026-09-27.md) |
| Sun 28 Sep (Day 2) | 36 prompts (Diwali still-life, wedding still-life with no people, terrazzo/marble/linen textures); first weekly metrics review (every metric unknown; verdict "adjust": keep going, stop drafting new themes until account and generator exist); 10-prompt pilot shortlist | [logs/2026-09-28.md](../logs/2026-09-28.md), [from-cto-new/pilot-prompt-shortlist-2026-09-28.md](../from-cto-new/pilot-prompt-shortlist-2026-09-28.md) |
| Mon 29 Sep (Day 3) | 36 prompts (Q1 wooden-blocks growth desk, beauty/skincare still-life, soft late-year festive); Firefly stock-resale check (yes, allowed); ZA Contributor setup checklist | [logs/2026-09-29.md](../logs/2026-09-29.md), [from-cto-new/firefly-stock-resale-2026-09-29.md](../from-cto-new/firefly-stock-resale-2026-09-29.md), [docs/adobe-contributor-setup.md](../docs/adobe-contributor-setup.md) |
| Tue 30 Sep (Day 4) | 36 prompts (soft Valentine's/romance still-life, calm workspace still-life, soft paper and pastel wash backgrounds); three follow-up runs with no new work | [logs/2026-09-30.md](../logs/2026-09-30.md) |
| Thu 1 Oct (Day 5) | Progress check plus a smaller batch of 24 prompts (minimal autumn/Halloween still-life, black and gold sale backgrounds) | [logs/2026-10-01.md](../logs/2026-10-01.md) |

Automation: the GitHub Action `.github/workflows/daily-prompts.yml` always prints `skipped: no API key` because no `OPENAI_API_KEY` or `ANTHROPIC_API_KEY` secret is set ([README.md](../README.md), Automation section). All logs above were written by the daily agent routine described in [CLAUDE.md](../CLAUDE.md).

## Next batch plan

Runs only after the blockers below are cleared. Three themes, all already drafted in the repo. Diwali is dropped from this batch: Diwali 2026 is 8 Nov ([ShubhPanchang](https://shubhpanchang.in/festivals/diwali-2026?lang=en)), which is closer than Adobe's advice to upload about three months ahead of a holiday ([Adobe Stock Artist Hub, Create what's in demand](https://stock.adobe.com/pages/artisthub/get-started/create-stock-content-that-sells-stock-contributor-guide-pt-1)). Keep the Diwali prompts for 2027. Halloween (1 Oct batch) is out of the window for the same reason.

### Theme 1: Q1 wooden-blocks growth desk (10 keepers)
- Prompts: pilot shortlist #1 plus Day 3 Theme 1 ([logs/2026-09-29.md](../logs/2026-09-29.md)).
- Demand evidence:
  - Saturation proxy (search result counts, not downloads): `wooden blocks steps growth desk` about 1,917 Adobe Stock results, against about 312,966 for `new year business planning`, checked 27 Sep 2026 ([from-cto-new/theme-validation-2026-09-27.md](../from-cto-new/theme-validation-2026-09-27.md)).
  - "concept" is a top-20 download keyword for AI images on Adobe Stock (third-party, May 2023 data: [Stock Performer](https://www.stockperformer.com/blog/is-ai-killing-the-stock-industry-a-data-perspective/)).
- Timing: brands prepare promotions ahead, so upload about three months before use ([Artist Hub](https://stock.adobe.com/pages/artisthub/get-started/create-stock-content-that-sells-stock-contributor-guide-pt-1)). That puts the New Year and Q1 window at roughly now, so this theme goes first.

### Theme 2: Soft Valentine's / romance still-life, no people (10 keepers)
- Prompts: Day 4 Theme 1 ([logs/2026-09-30.md](../logs/2026-09-30.md)). The pilot shortlist has none, so pick 10 from that list.
- Demand evidence:
  - Adobe says to upload seasonal content about three months ahead ([Artist Hub](https://stock.adobe.com/pages/artisthub/get-started/create-stock-content-that-sells-stock-contributor-guide-pt-1)), and two to three months before a holiday "significantly" raises ranking chances ([Artist Hub, Smart content submission strategies](https://stock.adobe.com/pages/artisthub/get-started/stock-content-submission-strategies-stock-contributor-guide-pt-4)).
  - "celebration" is a top-20 download keyword for AI images (third-party, May 2023: [Stock Performer](https://www.stockperformer.com/blog/is-ai-killing-the-stock-industry-a-data-perspective/)).
  - Saturation count: unknown (Adobe Stock search did not return results to an automated check on 1 Oct 2026).
- Timing: Valentine's Day is 14 Feb 2027, so the three-month mark is mid-Nov 2026. Reviews can take up to 8 weeks (community member claim, third-party: [Adobe Community](https://community.adobe.com/questions-38/is-there-any-shot-list-for-upcoming-months-329020)), so aim to submit by end Oct 2026.

### Theme 3: Material textures (terrazzo, marble, linen) (10 keepers)
- Prompts: pilot shortlist #6 to #10 plus Day 2 Theme 3 ([logs/2026-09-28.md](../logs/2026-09-28.md)).
- Demand evidence:
  - "background" is the number 2 download keyword for AI images on Adobe Stock, with "design", "abstract", "decoration" and "interior" also in the top 20 (third-party, May 2023: [Stock Performer](https://www.stockperformer.com/blog/is-ai-killing-the-stock-industry-a-data-perspective/)).
  - Adobe says evergreen content "is always in demand" ([Artist Hub](https://stock.adobe.com/pages/artisthub/get-started/create-stock-content-that-sells-stock-contributor-guide-pt-1)).
  - Saturation proxy: `terrazzo pattern background` about 105,359 results, against about 61,421,057 for `abstract background texture` (27 Sep 2026, [theme validation](../from-cto-new/theme-validation-2026-09-27.md)).
- Timing: evergreen, so any time.

### Count, rules and cost
- **Count:** 30 keepers (10 per theme), matching the pilot size in [logs/2026-09-28.md](../logs/2026-09-28.md) and [the shortlist](../from-cto-new/pilot-prompt-shortlist-2026-09-28.md). Generate extra candidates and curate down to 30 distinct images.
- **Adobe rules that apply:**
  - Tick "Created using generative AI tools" on every file and add the keyword "generative AI".
  - No artist names, real people, brands or third-party IP ([Generative AI content guidelines](https://helpx.adobe.com/stock/contributor/submit-your-content/submit-generative-ai-content/generative-ai-content-guidelines.html)).
  - Commercially released Firefly output may be submitted ([Firefly FAQ for Adobe Stock](https://helpx.adobe.com/stock/contributor/submit-your-content/submit-generative-ai-content/firefly-faq.html)).
- **Royalty:** 33% of the net price for photos and illustrations. Adobe's worked example gives US$0.99 per licensed photo ([Royalty rates](https://helpx.adobe.com/stock/contributor/payments-earnings/royalties-pricing/royalty-rates-assets.html)). Per-download earnings range from US$0.33 (large-plan minimum) to US$3.30, depending on the buyer's plan ([Adobe Stock Contributor royalties](https://contributor.stock.adobe.com/royalties)).
- **Payout:** US$25 minimum and 45 days after the first sale ([docs/adobe-contributor-setup.md](../docs/adobe-contributor-setup.md), citing [Payment requirements](https://helpx.adobe.com/stock/contributor/payments-earnings/payment-taxes/payment-requirements.html)).

**Monthly tool cost (estimate, at R16.42 per US$, USD/ZAR close on 30 Sep 2026 per [exa.ai markets](https://exa.ai/library/markets/forex/USDZAR?date=2026-09-30); ZA local prices and VAT may differ):**

| Option | US$ | Rand per month (estimate) | Price source |
|---|---|---|---|
| Firefly Standard (unlimited standard image generations, 2,000 premium credits) | 9.99/month | about R164 | Plan contents: [Adobe generative credits FAQ](https://helpx.adobe.com/creative-cloud/apps/generative-ai/generative-credits-faq.html) (updated 30 Sep 2026). Price: third-party trackers ([TechSifted](https://techsifted.com/guides/adobe-firefly-pricing-2026/), [Krea](https://www.krea.ai/blog/is-adobe-firefly-free-what-it-is-and-how-it-compares-in-2026)); adobe.com was unreachable from this check |
| Topaz Gigapixel Personal, paid annually | 149/year | about R204 | [Topaz pricing](https://www.topazlabs.com/pricing) (also US$19/month on an annual commitment, about R312, or US$29 month-to-month, about R476) |
| **Recommended: Firefly Standard plus Topaz Personal (annual)** | about 22.41/month | **about R368** | Sum of the two rows above |
| Firefly Standard only (skip Topaz if native output passes Adobe's size checks; unknown until tested) | 9.99/month | about R164 | As above |
| For reference: current "Firefly Premium" | 199.99/month | about R3,284 | [TechSifted](https://techsifted.com/guides/adobe-firefly-pricing-2026/) (third-party) |

Why the old R283 figure no longer works: [logs/2026-09-27.md](../logs/2026-09-27.md) priced "Firefly Premium" at US$4.99 for 100 credits (about R81). Adobe's FAQ lists the 100-credit Firefly plan as "Legacy" and no longer available to buy since 12 Feb 2025 ([generative credits FAQ](https://helpx.adobe.com/creative-cloud/apps/generative-ai/generative-credits-faq.html)). The Topaz half (about R202 to R204) still holds.

**Cost per accepted image (estimate):**
- If all 30 pilot images are accepted: R368 / 30 = about **R12 per accepted image** in month 1.
- At 15 accepted (the README's 50% acceptance target, which is a target, not data): about R25 per accepted image.
- At README pace (500 or more accepted a month), it falls below R1 per image.
- Kevin's own time is not costed (unknown).

## Break-even and decision checkpoint

**Break-even downloads per month to cover about R368 (US$22.41) of tools:**

| Royalty per download | Source | Downloads per month to break even |
|---|---|---|
| US$0.99 (main case) | Adobe worked example ([Royalty rates](https://helpx.adobe.com/stock/contributor/payments-earnings/royalties-pricing/royalty-rates-assets.html)) | **23** |
| US$0.33 (floor, large plans) | [Adobe Contributor royalties](https://contributor.stock.adobe.com/royalties) | 68 |
| US$1.94 (average for AI images, third-party, May 2023) | [Stock Performer](https://www.stockperformer.com/blog/is-ai-killing-the-stock-industry-a-data-perspective/) | 12 |

With Firefly Standard only (about R164), break-even is about 11 downloads a month at US$0.99.

**Portfolio needed (estimate from third-party averages):** Stock Performer measured revenue per image per month on Adobe Stock (May 2023) at US$0.0375 for all files and US$0.17 for AI images. Per year that is about US$0.45 and US$2.04 per image. Stock Performer said the AI figure was early and expected to fall. On those numbers, R368 a month needs roughly 130 (AI average) to 600 (all-files average) accepted images. **A 30-image pilot will not break even on its own.** It tests acceptance and early demand. Typical earnings per image for this repo: unknown until uploads happen.

**Keep/kill framing:**
- **Now:** zero revenue and zero cash cost, because nothing is set up. There is nothing to judge yet. The only cost is the daily agent routine (cost unknown), which keeps drafting prompts that cannot be used.
- **Gate 1, Sat 31 Oct 2026 (recommendation):** if the Contributor account and tool approval are still not done, pause the daily routine and the venture. This also misses the Valentine's upload window.
- **Gate 2, 60 days after the first accepted upload:** check the acceptance rate. If it is below 30% after metadata fixes, change themes or generator (the [README.md](../README.md) kill rule).
- **Decision checkpoint, 90 days after the first accepted upload:**
  - Keep and scale if downloads average **23 or more a month** in the last 30 days, or royalties cover about R368 a month.
  - Adjust if downloads are 10 to 22 a month.
  - Kill if downloads are below 10 a month with 300 or more accepted images, or royalties stay under US$25 a month (in line with the README's day-90 kill rule).

## Blockers only Kevin can clear

1. **Create the Adobe Stock Contributor account.**
   - Steps: Adobe ID, Contributor signup, verify email and phone, Form W-8BEN (without it Adobe withholds 30%), link Payoneer (listed by Adobe as the required payment provider for South Africa).
   - Source: [docs/adobe-contributor-setup.md](../docs/adobe-contributor-setup.md).
   - Note: [README.md](../README.md) still says PayPal; the checklist and Adobe's page say Payoneer for ZA.
2. **Approve tools: Firefly Standard plus Topaz Gigapixel Personal at about R368/month (estimate), or Firefly Standard alone at about R164/month.**
   - Do not approve "Firefly Premium" by name: it is now about R3,284/month.
   - Backup option in the logs: Leonardo plus Topaz, about R398/month (27 Sep prices, not re-checked) ([logs/2026-09-27.md](../logs/2026-09-27.md)).
3. **Add `blackvault/new-income-ideas-2026-09-27.md` to `from-cto-new/`, or confirm it is not needed.**
   - It is cited in [README.md](../README.md) but absent from the repo ([logs/2026-10-01.md](../logs/2026-10-01.md)).
   - The README's case-study earnings benchmark (Junpei) depends on it and has no public source in the repo, so treat that benchmark as unverified.

## Sources

Repo (LBD-DASH/ai-stock-images, main at `fbce2a6`):
- [README.md](../README.md), [CLAUDE.md](../CLAUDE.md), `.github/workflows/daily-prompts.yml`
- [logs/2026-09-27.md](../logs/2026-09-27.md), [logs/2026-09-28.md](../logs/2026-09-28.md), [logs/2026-09-29.md](../logs/2026-09-29.md), [logs/2026-09-30.md](../logs/2026-09-30.md), [logs/2026-10-01.md](../logs/2026-10-01.md)
- [docs/adobe-contributor-setup.md](../docs/adobe-contributor-setup.md)
- [from-cto-new/pilot-prompt-shortlist-2026-09-28.md](../from-cto-new/pilot-prompt-shortlist-2026-09-28.md), [from-cto-new/firefly-stock-resale-2026-09-29.md](../from-cto-new/firefly-stock-resale-2026-09-29.md), [from-cto-new/theme-validation-2026-09-27.md](../from-cto-new/theme-validation-2026-09-27.md)

Official Adobe (checked 1 Oct 2026):
- Royalty rates: https://helpx.adobe.com/stock/contributor/payments-earnings/royalties-pricing/royalty-rates-assets.html
- Earnings per download by buyer plan: https://contributor.stock.adobe.com/royalties
- Generative AI content guidelines: https://helpx.adobe.com/stock/contributor/submit-your-content/submit-generative-ai-content/generative-ai-content-guidelines.html
- Firefly FAQ for Adobe Stock: https://helpx.adobe.com/stock/contributor/submit-your-content/submit-generative-ai-content/firefly-faq.html
- Generative credits FAQ (Firefly plans, legacy plan status): https://helpx.adobe.com/creative-cloud/apps/generative-ai/generative-credits-faq.html
- Payment requirements: https://helpx.adobe.com/stock/contributor/payments-earnings/payment-taxes/payment-requirements.html
- Artist Hub, Create what's in demand: https://stock.adobe.com/pages/artisthub/get-started/create-stock-content-that-sells-stock-contributor-guide-pt-1
- Artist Hub, Smart content submission strategies: https://stock.adobe.com/pages/artisthub/get-started/stock-content-submission-strategies-stock-contributor-guide-pt-4

Third-party (labelled as such above):
- Stock Performer, May 2023 data (RPI, RPD, sell-through, AI keywords): https://www.stockperformer.com/blog/is-ai-killing-the-stock-industry-a-data-perspective/
- Firefly plan prices: https://techsifted.com/guides/adobe-firefly-pricing-2026/ and https://www.krea.ai/blog/is-adobe-firefly-free-what-it-is-and-how-it-compares-in-2026
- Topaz pricing: https://www.topazlabs.com/pricing
- USD/ZAR, 30 Sep 2026: https://exa.ai/library/markets/forex/USDZAR?date=2026-09-30
- Diwali 2026 date: https://shubhpanchang.in/festivals/diwali-2026?lang=en
- Review time claim (community member): https://community.adobe.com/questions-38/is-there-any-shot-list-for-upcoming-months-329020

Unknown or unsourced:
- Current Adobe Stock search counts for Valentine's themes
- Firefly price in ZAR from adobe.com directly (site unreachable from this check)
- Earnings per image for this portfolio
- Daily agent run cost
- Whether Firefly native output meets Adobe's size checks without upscaling
