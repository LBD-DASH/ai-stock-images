# AI Stock Images (Adobe Stock and similar sites)

_Repo: `ai-stock-images`. Side venture, separate from YardOps, 6HN and LBD. Background research: `blackvault/new-income-ideas-2026-09-27.md` (27 Sep 2026)._

## The idea
We generate commercially useful AI stock images, curate and upscale them, write strong titles and keywords, and sell licences through stock sites, starting with Adobe Stock. Every image is **clearly disclosed as AI-generated**, as the stock sites require. Buyers license them and we earn a royalty on each download. We track what gets accepted and downloaded, and do more of whatever sells.

## Target platform
Adobe Stock Contributor first (web upload or SFTP bulk upload). Other sites earned about 1/200th of Adobe's revenue in the case study, so we ignore them at first. Before adding any other site, check its current AI policy: some accept AI images only with disclosure, and some don't accept AI-generated uploads at all.

## How money is made
- Adobe Stock royalty (research notes, check current terms): 33% per licence, at least $0.33 a download ($0.36 after 1,000 downloads, $0.38 after 10,000). Extended licences occasionally pay about $26.
- Paid out in USD once earnings pass $25 (PayPal or Skrill; to confirm), then to an SA bank through PayPal/FNB.
- Case-study benchmark (Junpei): month 1 $52 (71 downloads, 534 accepted), month 3 $298, month 6 $432, month 9 $590. Our estimate: month 1 R0–900, month 3 R1,000–5,000, month 6 R2,000–8,000.

## First 30 days
- **Day 1:** Research demand in Adobe Stock search (top themes, seasonal themes for Dec–Feb and Valentine's, Q1 business). Write a do-not-generate list: real people, brands, logos, artists' styles, trademarked landmarks and anything that could be mistaken for a real news event.
- **Days 2–3:** Generate about 300 candidates across 5 themes (for example weddings, beauty, business/lifestyle, backgrounds, seasonal). Curate, upscale, and check for artefacts (hands, text).
- **Day 4:** Keyword them: titles under 70 characters, 25–49 keywords ordered by relevance, **'Created using generative AI' box ticked on every upload**. Upload about 150.
- **Days 5–30:** Upload 30–50 a day, staying under the roughly 1,000-a-month review ceiling. Log acceptances and rejections each day, and resubmit rejects with rewritten metadata. Move effort to the themes with the best acceptance and downloads per 1,000 images.

## Success and kill criteria
**Success (keep going and scale):**
- Day 30: 500+ accepted images, acceptance rate 50% or better, and at least 1 download.
- Month 3: 2,000+ accepted and $150+ earned in the month (half the case-study pace). Then keep scaling toward the 1,000/month ceiling.

**Kill (stop or change direction):**
- Acceptance below 30% for 3 weeks running after metadata fixes: change themes or generator.
- Fewer than 10 downloads by day 60 with 1,000+ accepted: re-research demand, and kill at day 90 if still below $25 a month.
- Any account warning about IP, likeness or AI disclosure: stop uploads and review with Kevin.

## What only Kevin can do
- Create the Adobe Stock Contributor account and verify ID.
- Complete the W-8BEN form (SA treaty) and link PayPal.
- Approve any paid image-generation or upscaler subscription (about R400–800 a month), after checking its licence allows commercial stock use.

## Risks and policy rules
- **AI disclosure is mandatory:** Adobe accepts generative AI only if it's disclosed (tick the AI box and follow their title rules). Never show real people, brands, logos or artists' styles, or the account can be closed.
- The image generator's terms must allow commercial use and resale of outputs.
- Nearly all revenue depends on one platform, and Adobe controls pricing and review.

## Repo layout
- `README.md`: this plan
- `assets/`: source files and exports (keep large binaries out of git where you can)
- `prompts/`: plain-markdown prompts that work pasted into Claude, ChatGPT or any other assistant
  - `daily-progress-check.md` and `daily-next-content.md` run every day
  - `weekly-metrics-review.md` is run by hand once a week
- `from-cto-new/`: material carried over from cto.new (the prompt runner includes any text files here as context)
- `scripts/run_prompts.py`: runs prompts through OpenAI or Anthropic and appends the output to `logs/YYYY-MM-DD.md`
- `logs/`: one file per day (`YYYY-MM-DD.md`). Agents append output; Kevin pastes real metrics in by hand.
- `.github/workflows/daily-prompts.yml`: runs the two daily prompts at 04:17 UTC (06:17 SAST) every day, or by hand from the Actions tab

## Automation
The daily workflow only calls an LLM if a repo secret `OPENAI_API_KEY` or `ANTHROPIC_API_KEY` exists. Without one it prints `skipped: no API key` and finishes cleanly without committing anything. To switch it on, add one of the secrets under Settings → Secrets and variables → Actions. Optional repo variables: `OPENAI_MODEL` or `ANTHROPIC_MODEL` to pick the model, and `LLM_PROVIDER=anthropic` to prefer Anthropic when both keys are set.

Run locally: `python scripts/run_prompts.py` (daily prompts), `python scripts/run_prompts.py weekly-metrics-review`, or `python scripts/run_prompts.py --all`.

The prompts can only reason over the README, logs and `from-cto-new/`. They can't see platform dashboards, so paste real numbers into the day's log, or the reviews will say "unknown".
