# Daily next content: AI Stock Images (Adobe Stock and similar sites)

## Inputs
Use the repo's `README.md` (the plan, money model, 30-day plan and success/kill criteria), the most recent files in `logs/` (newest first) and anything in `from-cto-new/`. If you're pasting this prompt into a chat assistant, paste or attach those files below it. If no logs are supplied, treat today as Day 1 of the 30-day plan.

## Task
Plan **today's upload batch** (30–50 images).
1. From the README and logs, work out which themes have the best acceptance rate and downloads, which were rejected and why, and what's seasonal in the next 4–10 weeks.
2. Pick 2–4 themes for today and give the reason for each.
3. For each theme write:
   - 10–15 image-generation prompts that don't depend on any particular generator: subject, composition, lighting, style, aspect ratio and copy space, with no real people, brands, logos, artist names or trademarked landmarks
   - a title template (under 70 characters) and a list of 25–49 keywords ordered by relevance
4. List any rejected images from the logs worth resubmitting with rewritten metadata, and give the new metadata.
5. Give a QA checklist for today: hands, text artefacts, upscaling size, no IP or likeness issues, and **the generative-AI disclosure box ticked on every file**.

## Output
Reply with a single markdown section that starts with the heading `## Next content`. It gets appended to `logs/YYYY-MM-DD.md` (today's date), either by the daily workflow or by Kevin pasting it in.

Rules:
- Don't make up numbers. If a metric isn't in the logs, write "unknown" and say who needs to supply it.
- Keep it short and specific. Kevin should be able to act on it in under 5 minutes.
- Mark anything that needs Kevin personally (accounts, KYC, payments, approvals, reviews) with **[KEVIN]**.
