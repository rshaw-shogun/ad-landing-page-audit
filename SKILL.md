---
name: ad-landing-page-audit
description: Use when auditing paid social ads against their landing pages, checking for offer, product, creator or message mismatches, or when asked for the weekly ad-to-page audit.
---

# Ad-to-landing page audit

Find ads whose landing page doesn't deliver what the ad promised, rank them by wasted spend, and suggest fixes. Report and draft only. Never change ads, budgets or live pages.

## Before the first run

Values in [brackets] are settings for this brand. If any are still in brackets when the audit starts, ask the user for them before going further, and suggest the default shown.

## 1. Gather the data

- From the Meta Ads connector [or the export folder: name it], pull every ad in the ad library that is currently active and delivering, with no spend minimum. Skip paused, archived and deleted ads, and ads in paused campaigns or ad sets. Use the last [14] days of data for each active ad: image or video, headline, primary text, call to action, full destination URL with UTMs, creator name or handle if any, spend, click-through rate.
- From [Shopify / your analytics tool], pull conversion rate and revenue per visitor for each landing page over the same dates.
- If a source can't be reached, say which one at the top of the report and continue with what you have. Never guess missing numbers.
- Audit every ad, not a sample. For large libraries, work in batches by campaign, highest spend first, and save progress to the results file after each batch. If a run ends early, the next run picks up where it stopped, and the report says how many ads are still unchecked.

## 2. Prepare each ad

- Group ads that share a destination URL and creative concept. Score each group once, but record every ad in it in the results file, so every ad in the library gets a score.
- For video ads, take frames at the start, middle and end, and transcribe the audio. Spoken offers count as part of the ad.

## 3. Capture each landing page

- Use the full destination URL exactly as the ad sends it, with every parameter kept: UTMs, discount codes, and any product, variant or collection parameters. Never shorten or clean up the URL. If the link is wrapped in a Facebook redirect (l.facebook.com), take the real destination from inside it, parameters included.
- Before loading, list the parameters and note any that could change what the page shows, such as a product ID, variant, handle, "featured", "pin" or sort parameter. Many stores use these to put the clicked product first on a collection page.
- Open that exact URL on a phone-sized screen (390 px wide). Wait until the page has fully loaded, including product grids that load after the page appears, since personalization often happens a few seconds in.
- If a parameter looks like it personalizes the page, also load the same page without it. If the ad's product moves to the top or is highlighted only with the parameter, the page is personalized: judge the personalized version.
- Close cookie banners. If a pop-up covers the first screen, screenshot it once, close it, then continue.
- Screenshot the first screen without scrolling, then the full page.
- Note redirects, out-of-stock products, errors, and region or currency changes.

## 4. Score each pairing

Score each area 2, 1 or 0, for a total out of 12.

- Offer. 2: the same discount, bundle or free shipping is on the first screen and applied automatically if the ad implied it. 1: present but below the fold, worded differently, or needs a manual code. 0: missing or contradicted.
- Product. 2: the exact product, colorway or bundle from the ad is the hero. 1: on the page but not featured, or a close variant. 0: generic collection or homepage, or out of stock. A collection page scores 2 if its URL parameters put the ad's product first or feature it on the first screen. Score it on the page as the ad's own link loads it, never on the plain collection URL.
- Creator (skip and score 2 if the ad has no creator). 2: the creator's name, quote, photo or video is on the first screen. 1: lower on the page. 0: absent. Identify creators only by the name or handle in the ad's metadata, never by face.
- Message. 2: the page headline repeats the ad's hook or main claim. 1: the claim appears but not in the headline. 0: not mentioned.
- Look and tone. 2: same visual style and energy. 1: noticeably different but clearly the same brand. 0: feels like a different company. Mark this score as a judgment call.
- Details. 2: urgency, shipping, price, currency and language all match. 1: one small difference. 0: a promise from the ad is missing or wrong, such as "ends Sunday" with no mention.

Any pairing with 0 on Offer or Product is a priority flag, whatever its total.

## 5. Rank

- Priority = weekly spend x (12 - score).
- Note pairings with above-average click-through but below-average conversion. These are the strongest signs the page is breaking the ad's promise.

## 6. Compare with last run

- Read [the results file, such as Ad audit results.csv in the shared folder].
- Mark each issue New, Still open or Fixed. If an ad from last run has since been paused, mark it Paused and drop it from the report, rather than counting it as Fixed. Then save this run's results to the same file.

## 7. Report

Use this format every time:

1. One-sentence summary: active ads in the library, ads checked, priority flags, and estimated spend on mismatched pages.
2. A table of every pairing with a priority flag or a score below [9] out of 12, sorted by priority: ad name, landing page, score, what's missing, weekly spend, status (New / Still open / Fixed), suggested fix.
3. Ad and first-screen screenshots side by side for each pairing in that table.
4. Fixed since last run.
5. Anything that couldn't be checked, and why, plus a link to the full results file with a score for every active ad.

Suggested fixes change the page, not the ad: add the offer to the hero, link to the product page, add a creator section, repeat the hook in the headline, or reuse the ad's own footage.

Send the report to [names or channel].
