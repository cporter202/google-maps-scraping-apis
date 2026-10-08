<div align="center">

<img src="./assets/hero.svg" alt="Google Maps Scraping APIs — local business data, reviews, and lead lists" width="100%" />

<br />

# 🗺️ Google Maps Scraping APIs

**Local business data, reviews, and ready-made lead lists — powered by production-ready Apify actors.**

[![GitHub stars](https://img.shields.io/github/stars/cporter202/google-maps-scraping-apis?style=for-the-badge)](https://github.com/cporter202/google-maps-scraping-apis/stargazers)
[![License](https://img.shields.io/github/license/cporter202/google-maps-scraping-apis?style=for-the-badge)](LICENSE)

<p>
  <a href="catalog/README.md"><strong>Browse the Actor Catalog</strong></a> ·
  <a href="#start-with-a-job-to-be-done"><strong>Start Building</strong></a>
</p>

</div>

## What this repo is

A focused directory of Google Maps scraping APIs for building local lead lists, reputation monitors, market-intelligence dashboards, and location-based research tools. Every actor is a ready-to-run [Apify](https://apify.com?fpr=p2hrc6) worker — no scrapers to build, no proxies to manage, no blocks to fight.

The main content of this repository:

- [Browse the actor catalog](catalog/README.md) — every Google Maps actor, verified live, one entry per actor with what it extracts and what it costs.

| Coverage snapshot | This directory |
|---|---:|
| Verified Google Maps actors | **8** |
| Typical fields per place | **20–30** |
| Starting cost | **Free tier + pay-per-result** |

## Start with a job to be done

| If you need to… | Start here |
|---|---|
| Build a list of local businesses with phones + websites | [Actor catalog](catalog/README.md) → place scrapers |
| Monitor a business's Google reviews over time | [Review monitoring playbook](playbooks/review-monitoring.md) |
| Generate leads for an agency or sales team | [Local lead pipeline playbook](playbooks/local-lead-pipeline.md) |
| Compare actors before spending a dollar | [Actor catalog](catalog/README.md) — pricing notes per actor |

## Common build paths

- **Local lead generation** — scrape "dentists in Dallas TX", get names, phones, websites, ratings → enrich → outreach. The [local lead pipeline playbook](playbooks/local-lead-pipeline.md) walks through it end to end.
- **Reputation monitoring** — track new reviews for your business or your clients' businesses on a schedule, get alerted to 1-star reviews the same day.
- **Market intelligence** — map every competitor in a category across a metro area: ratings, review velocity, price positioning.
- **Review-pitch prospecting** — find businesses with bad reviews, then pitch them reputation help with the evidence in hand.

## Why Apify actors instead of building your own scraper

Google Maps actively fights scrapers: fingerprinting, rate limits, CAPTCHAs, layout changes. Maintaining your own Maps scraper is a full-time job. These actors run on Apify's infrastructure with proxy rotation, retries, and maintenance handled by the actor authors — you pay per result and get clean JSON back.

**[→ Get started on Apify (free tier)](https://apify.com?fpr=p2hrc6)**

## Disclosure

Links to Apify in this repo include my affiliate code (`fpr=p2hrc6`). You pay exactly the same price — it supports keeping this directory updated and verified.

## Contributing

Found a Google Maps actor that belongs here? Open a PR adding it to `catalog/README.md` with a verified `apify.com` URL and a one-line description. Only actors you have confirmed exist on the Apify Store, please.

## License

MIT — see [LICENSE](LICENSE).
