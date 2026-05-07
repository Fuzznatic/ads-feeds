# ads-feeds

Automated feed cache for Atolls / Pepper ad creatives. A GitHub Actions workflow fetches live deal data from the Pepper Marketing API every 6 hours and commits the results as static JSON files. Banners served via GAM fetch from this repo — no API key is ever exposed in the creative.

## Feed URLs (use these in banners)

| Locale | URL |
|--------|-----|
| UK (hotukdeals) | `https://raw.githubusercontent.com/Fuzznatic/ads-feeds/main/feeds/uk.json` |
| DE (mydealz) | `https://raw.githubusercontent.com/Fuzznatic/ads-feeds/main/feeds/de.json` |
| FR (dealabs) | `https://raw.githubusercontent.com/Fuzznatic/ads-feeds/main/feeds/fr.json` |
| ES (chollometro) | `https://raw.githubusercontent.com/Fuzznatic/ads-feeds/main/feeds/es.json` |

## Setup (one-time)

### 1. Add the API key as a GitHub Secret

1. Go to **Settings → Secrets and variables → Actions** in this repo
2. Click **New repository secret**
3. Name: `PEPPER_API_KEY`
4. Value: your Pepper Marketing API key
5. Click **Add secret**

### 2. Push this folder to the repo

Make sure the `.github/workflows/refresh-feeds.yml` file and the `feeds/` folder are committed and pushed to the `main` branch.

### 3. Trigger the first run manually

1. Go to **Actions → Refresh Pepper Ad Feeds**
2. Click **Run workflow → Run workflow**
3. Wait ~30 seconds — the feeds folder will be updated with live data

After that, the workflow runs automatically every 6 hours.

## How it works

```
GitHub Actions (every 6h)
  └─ curl marketing.pepper.com/feeds/ads/uk  (with secret API key)
  └─ curl marketing.pepper.com/feeds/ads/de
  └─ curl marketing.pepper.com/feeds/ads/fr
  └─ curl marketing.pepper.com/feeds/ads/es
  └─ commit feeds/*.json to main branch

GAM banner (user's browser)
  └─ fetch raw.githubusercontent.com/Fuzznatic/ads-feeds/main/feeds/uk.json
       (public, CORS-open, no key needed)
  └─ render live deals
```

## Workflow schedule

The cron runs at `0 */6 * * *` — midnight, 06:00, 12:00, 18:00 UTC.
To change frequency, edit `.github/workflows/refresh-feeds.yml` and update the cron expression.
