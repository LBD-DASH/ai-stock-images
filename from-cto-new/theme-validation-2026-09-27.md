# Theme validation — 2026-09-27

Live Adobe Stock search result counts (stock.adobe.com), checked 27 Sep 2026. These are total catalogue results, not accepted-per-day or download data, which Adobe doesn't expose publicly — treat the counts as a rough saturation signal only, not a demand forecast.

| Theme | Sample search term | Result count | Competition note |
|---|---|---|---|
| 1. Holiday backgrounds with copy space | `christmas background copy space` | ~2,938,180 | Extremely saturated broad term — expected, it's the single most competitive seasonal query on the platform. A generic "christmas background" upload will be buried on page 50+. |
| 1. Holiday backgrounds with copy space (niche) | `diwali diya flat lay` | ~3,948 | Far less saturated. The README's Theme 1 prompt #12 (Diwali flat lay) targets a genuine gap — worth prioritising over generic Christmas shots. |
| 2. New Year / Q1 business planning | `new year business planning` | ~312,966 | Moderately saturated but an order of magnitude less than Christmas. Still a lot of near-identical "planner + coffee + laptop" shots. |
| 2. New Year / Q1 business planning (niche) | `wooden blocks steps growth desk` | ~1,917 | Low saturation. README's Theme 2 prompt #3 (wooden blocks as rising steps) is a good differentiated pick. |
| 3. Evergreen abstract backgrounds/textures | `abstract background texture` | ~61,421,057 | By far the most saturated term checked — generic abstract backgrounds are the most oversupplied category on Adobe Stock. Broad "abstract background" uploads will get almost no visibility. |
| 3. Evergreen abstract backgrounds/textures (niche) | `terrazzo pattern background` | ~105,359 | Still saturated (100K+) but ~600x less than the broad term. Material-specific textures (terrazzo, marble veining, raw linen — README prompts #3, #9, #12) beat generic "abstract" every time. |

## Recommendation
The broad theme names in the README (used as search-volume proxies) are all heavily saturated, which is expected for evergreen/seasonal stock categories — this doesn't mean don't pursue them, it means **the specific, material/subject-led prompts already drafted in `logs/2026-09-27.md` matter more than the theme label**. Prioritise the niche variants already in the 36-prompt list (Diwali, wooden-blocks-growth, terrazzo/marble/linen textures) over the most generic version of each theme, since they sit in far shallower search results with the same buyer intent.

## Method / limits
- Counts read from the Adobe Stock public search page title ("Browse N Stock Photos, Vectors, and Video") via `stock.adobe.com/search?k=<term>`, no login.
- No visibility into acceptance rate, download counts, or how many of the top results are themselves AI-generated — Adobe doesn't expose that via public search.
- Region defaulted to South Africa (`stock.adobe.com/za/...`); counts may vary slightly by region/currency setting but should be directionally the same.
