# Playbook: Local Lead Pipeline from Google Maps

Turn Google Maps into an unlimited source of local business leads. Total build time: about an hour. No scraper maintenance, ever.

## What you get

A repeatable pipeline: **search → scrape → enrich → export → outreach**. Example output: 500 plumbers in the Dallas–Fort Worth metro with business name, phone, website, address, rating, and review count.

## Step 1 — Pick your actor

For bulk place scraping, start with the highest-volume option:

- [Google Maps Scraper (Compass)](https://apify.com/compass/crawler-google-places?fpr=p2hrc6) — best for thousands of places, full reviews + images
- [Google Maps Scraper (Thirdwatch)](https://apify.com/thirdwatch/google-maps-scraper?fpr=p2hrc6) — best when you want predictable $0.002/result pricing

Both take a search string + location. Example searches that work well:

- `"dentists in Austin TX"`
- `"roofing companies in Miami FL"`
- `"coffee shops in Portland OR"`

## Step 2 — Run the scrape

In the Apify Console, paste your search into the actor input. Set `maxCrawledPlacesPerSearch` to control volume and cost (start with 50–100 while testing). Run it.

For repeatable pipelines, use the API instead:

```bash
curl -X POST "https://api.apify.com/v2/acts/compass~crawler-google-places/run-sync-get-dataset-items?token=YOUR_APIFY_TOKEN" \
  -H "Content-Type: application/json" \
  -d '{
    "searchStringsArray": ["dentists in Austin TX"],
    "maxCrawledPlacesPerSearch": 100
  }'
```

## Step 3 — Filter for your ideal customer

Raw Maps data includes everyone. Your money is in the filter. Common winning filters:

- **No website** → pitch web design (huge market: ~30–40% of small businesses have no site or a bad one)
- **Rating below 4.0 with 20+ reviews** → pitch reputation management
- **No recent reviews** → pitch review generation
- **Specific categories** → verticalize your offer (dentists, roofers, salons)

Export to CSV from the Apify dataset, filter in Google Sheets.

## Step 4 — Enrich (optional but powerful)

Phone numbers come with most place results. For email outreach, pair with an email-finder actor. For direct mail, you already have the address.

## Step 5 — Outreach

Push the filtered list into your CRM, cold email tool, or SMS platform. Track which search + filter combos convert, then scale the winners.

## Cost math

At ~$0.002–$0.004 per place, 1,000 leads costs $2–$4. One closed client pays for roughly 10,000 leads. The math is why this playbook exists.

**[→ Start scraping on Apify](https://apify.com?fpr=p2hrc6)**
