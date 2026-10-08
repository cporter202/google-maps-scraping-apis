# Playbook: Google Review Monitoring

A bad review sitting unanswered for a week costs real customers. This playbook sets up automated review monitoring for your business or your clients' businesses — new reviews pulled on a schedule, alerts the moment a 1-star lands.

## What you get

Scheduled pulls of complete review histories for any Google Maps listing, with review text, ratings, dates, and reviewer info. Pipe it into Slack, email, or a dashboard.

## Step 1 — Pick your actor

- [Google Maps Reviews Scraper (Compass)](https://apify.com/compass/google-maps-reviews-scraper?fpr=p2hrc6) — complete review histories including review images, 4.8/5 rating. Best for deep reputation work.

Feed it the direct Google Maps URL of the business listing.

## Step 2 — Schedule it

In the Apify Console, use the actor's **Schedules** feature: run weekly (or daily for high-volume businesses). Each run appends new reviews to the dataset.

Via API with a cron job or scheduled workflow:

```bash
curl -X POST "https://api.apify.com/v2/acts/compass~google-maps-reviews-scraper/run-sync-get-dataset-items?token=YOUR_APIFY_TOKEN" \
  -H "Content-Type: application/json" \
  -d '{
    "startUrls": ["https://www.google.com/maps/place/?q=place_id:YOUR_PLACE_ID"],
    "maxReviews": 100
  }'
```

## Step 3 — Alert on what matters

Compare each run against the previous one. Alert conditions worth wiring up:

- **New 1–2 star review** → immediate Slack/email alert so you can respond same-day
- **Review velocity drop** → nobody's reviewing; time to ask happy customers
- **Competitor review spike** → someone's running a review campaign; investigate

Apify webhooks fire on run completion — point one at a small script, Make.com scenario, or Zapier to handle the diffing and alerting.

## Step 4 — Turn it into a service (agencies)

Review monitoring is one of the easiest retainers to sell: businesses know reviews matter, nobody wants to watch them manually. Package it as "reputation watch" — weekly review digest + instant bad-review alerts + suggested responses. Your cost per client per month is pennies in actor runs.

## Responding well

The data is half the job. When a bad review lands: respond publicly within 24 hours, acknowledge specifically, take it offline ("please call us at…"), never argue. A well-handled 1-star review converts more readers than a 5-star one.

**[→ Set up monitoring on Apify](https://apify.com?fpr=p2hrc6)**
