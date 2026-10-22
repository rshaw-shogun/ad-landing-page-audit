# Ad-to-Landing Page Audit: a free Claude skill

A Claude skill that checks your active Meta ads against their landing pages and flags mismatches, such as an offer, product or creator from the ad that's missing after the click. It ranks the problems by ad spend, so you know what to fix first.

Made by [Shogun](https://getshogun.com).

## Download

**[Download SKILL.md](https://github.com/rshaw-shogun/ad-landing-page-audit/releases/latest/download/SKILL.md)**

It's a single plain-text file with no code or scripts. You can read it in full in this repo ([SKILL.md](SKILL.md)) before downloading. The skill only reports and suggests fixes. It never changes your ads, budgets or pages.

## What it checks

For every active ad and its landing page, Claude scores six things from 0 to 2:

| Area | What it looks for |
| --- | --- |
| Offer | The ad's discount, code or free shipping shows on the first screen |
| Product | The exact product from the ad is featured, including collection pages personalized by the ad's link |
| Creator | The influencer or UGC creator from the ad appears on the page |
| Message | The ad's main claim is repeated in the page headline |
| Look and tone | The page feels like the same brand moment as the ad |
| Details | Urgency, shipping, price, currency and language all match |

You get a report of every flagged ad with screenshots and a suggested fix, ranked by spend.

## Set it up in three steps

1. Download `SKILL.md`. Keep the file name as it is.
2. Open a new chat in Claude, attach the file and ask: "Save this as a skill." Then click **Save skill**.
3. Ask Claude: "Run the ad–landing page audit." The first time, Claude asks for a few settings, such as who should get the report.

To run it every week, ask Claude: "Create a scheduled task that runs the ad–landing page audit every Monday morning."

## What you'll need connected

- **Your Meta Ads account**, through a Meta Ads connector or a scheduled Ads Manager export
- **Shopify or your analytics tool**, for conversion rates by landing page
- **A browser**, either Claude in Chrome or Claude's built-in browser, so Claude can open each landing page like a shopper

## Updates

New versions are published under [Releases](https://github.com/rshaw-shogun/ad-landing-page-audit/releases). The download link above always gets the latest one.

Questions or ideas? Email [ryan@getshogun.com](mailto:ryan@getshogun.com).
