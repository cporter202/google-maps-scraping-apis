# Google Maps Scraping APIs

**Organized APIs by category — every actor below is verified live on the Apify Store.**

| API Name | Description |
|----------|-------------|
| [🗺️ Google Maps Scraper (Compass)](https://apify.com/compass/crawler-google-places?fpr=p2hrc6) | The most-used Google Maps scraper on Apify: 39,000+ monthly users, 4.7/5 rating. Extract thousands of business listings with reviews, reviewer details, images, contact info, hours, and coordinates. Search by keyword + location or feed it direct place URLs. |
| [📍 Google Maps Scraper (Apify)](https://apify.com/apify/google-maps-scraper?fpr=p2hrc6) | Apify's official Google Maps actor. Business listings with phone, website, hours, rating, reviews count, category, and email extraction. Search strings like "accountants in Austin TX". |
| [💰 Google Maps Scraper (Thirdwatch)](https://apify.com/thirdwatch/google-maps-scraper?fpr=p2hrc6) | Pay-per-result pricing ($0.002/result). Name, phone, website, rating, GPS, and hours by search query + location. Built for lead-gen pipelines that need predictable per-lead costs. |
| [⚡ Google Maps Scraper (x_guru)](https://apify.com/x_guru/google-maps-scraper?fpr=p2hrc6) | Fast Google Maps place scraper: collect places by search term and location, enrich by Place ID, pull websites, phones, addresses, ratings, and coordinates for local lead lists. |
| [📊 Google Maps Business Scraper (Bovi)](https://apify.com/bovi/google-maps-scraper?fpr=p2hrc6) | 27 fields per place — name, address, phone, website, rating, reviews, category, lat/lng, hours, amenities, plus a parse-confidence score. $4 per 1,000 places. Built for lead generation and market research. |
| [⭐ Google Maps Reviews Scraper (Compass)](https://apify.com/compass/google-maps-reviews-scraper?fpr=p2hrc6) | Pull complete review histories for any Google Maps listing, including review text, ratings, dates, and reviewer photos. 4.8/5 rating. Ideal for reputation monitoring and review-pitch prospecting. |
| [🎯 Google Maps Extractor (Compass)](https://apify.com/compass/google-maps-extractor?fpr=p2hrc6) | Lightweight, lower-cost extractor for core place fields from direct URLs. Faster and cheaper when you don't need full reviews and images — 4.87/5 rating. |
| [🔎 Google Search Scraper (Apify)](https://apify.com/apify/google-search-scraper?fpr=p2hrc6) | Scrape Google search result pages with country/language targeting — organic results, paid results, AI overviews, and ads. 21,000+ monthly users. Pair with Maps scrapers for local SERP + listing coverage. |

## How to run any actor

1. Open the actor link above (my affiliate link — you pay the same, it supports this list).
2. Sign up for a free Apify account if you don't have one.
3. Paste your search (e.g. `"plumbers in Erie PA"`) into the actor's input and run.
4. Export results as JSON, CSV, or push them straight to Google Sheets, your CRM, or a webhook.

Or run from code with the [Apify API](https://apify.com?fpr=p2hrc6):

```bash
curl -X POST "https://api.apify.com/v2/acts/compass~crawler-google-places/run-sync-get-dataset-items?token=YOUR_APIFY_TOKEN" \
  -H "Content-Type: application/json" \
  -d '{"searchStringsArray": ["plumbers in Erie PA"], "maxCrawledPlacesPerSearch": 50}'
```

## More actors

This catalog grows as new Maps actors hit the Apify Store. Every link above was verified live. If an actor is missing, [search the Apify Store](https://apify.com/store?fpr=p2hrc6) — and if you sign up through any link on this page, it supports keeping this directory updated at no extra cost to you.
