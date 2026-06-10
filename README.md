# ads-feeds

Automated feed cache for Atolls / Pepper ad creatives.
GitHub Actions fetches from the Pepper Marketing API every 6 hours using a secret API key
and commits the results as static JSON. Banners fetch from raw GitHub URLs — no API key
is ever exposed in any creative.

> Last updated: **2026-06-10 04:23 UTC**

---

## Feed URLs (use these in banners)

### Locale Feeds
| Feed | Raw URL |
|------|---------|
| AMAZONMX2026 (Amazonmx2026) | `https://raw.githubusercontent.com/Fuzznatic/ads-feeds/main/feeds/Amazonmx2026.json` |
| DE (DE) | `https://raw.githubusercontent.com/Fuzznatic/ads-feeds/main/feeds/DE.json` |
| GAMING (Gaming) | `https://raw.githubusercontent.com/Fuzznatic/ads-feeds/main/feeds/Gaming.json` |
| AT (pepper.com AT) | `https://raw.githubusercontent.com/Fuzznatic/ads-feeds/main/feeds/at.json` |
| DE-ALIBABAFEED (de-AlibabaFeed) | `https://raw.githubusercontent.com/Fuzznatic/ads-feeds/main/feeds/de-AlibabaFeed.json` |
| DE-AMAZONFEED (de-AmazonFeed) | `https://raw.githubusercontent.com/Fuzznatic/ads-feeds/main/feeds/de-AmazonFeed.json` |
| DE (mydealz) | `https://raw.githubusercontent.com/Fuzznatic/ads-feeds/main/feeds/de.json` |
| ES (chollometro) | `https://raw.githubusercontent.com/Fuzznatic/ads-feeds/main/feeds/es.json` |
| FR (dealabs) | `https://raw.githubusercontent.com/Fuzznatic/ads-feeds/main/feeds/fr.json` |
| MX-AMAZONFEED (mx-AmazonFeed) | `https://raw.githubusercontent.com/Fuzznatic/ads-feeds/main/feeds/mx-AmazonFeed.json` |
| MX (promodescuentos) | `https://raw.githubusercontent.com/Fuzznatic/ads-feeds/main/feeds/mx.json` |
| NL (pepper.com NL) | `https://raw.githubusercontent.com/Fuzznatic/ads-feeds/main/feeds/nl.json` |
| PL (pepper.com PL) | `https://raw.githubusercontent.com/Fuzznatic/ads-feeds/main/feeds/pl.json` |
| SE (pepper.com SE) | `https://raw.githubusercontent.com/Fuzznatic/ads-feeds/main/feeds/se.json` |
| UK-ALIBABAFEED (uk-AlibabaFeed) | `https://raw.githubusercontent.com/Fuzznatic/ads-feeds/main/feeds/uk-AlibabaFeed.json` |
| UK (hotukdeals) | `https://raw.githubusercontent.com/Fuzznatic/ads-feeds/main/feeds/uk.json` |

### Merchant Feeds
| Feed | Raw URL |
|------|---------|
| mx-merchant-85 | `https://raw.githubusercontent.com/Fuzznatic/ads-feeds/main/feeds/mx-merchant-85.json` |

### Category Feeds
| Feed | Raw URL |
|------|---------|

---

## How to add a new feed

Edit `.github/workflows/refresh-feeds.yml` and add one line to the FEEDS array:

```bash
# Locale feed:    "locale/:locale"
# Merchant feed:  "locale/merchant/id/:locale-merchant-id"
# Category feed:  "locale/id/:locale-cat-id"
```

Then: **Actions -> Refresh Pepper Ad Feeds -> Run workflow**

Merchant filenames are set on the first run using the merchantName field
from the API and stay stable on all subsequent runs.

---

## How it works

```
GitHub Actions (every 6h, cron: 0 */6 * * *)
  fetch Pepper Marketing API with secret PEPPER_API_KEY
  save as feeds/*.json
  update this README

GAM banner (in user browser)
  fetch raw.githubusercontent.com/Fuzznatic/ads-feeds/main/feeds/NAME.json
  public, no API key needed, renders live deals
```

---

## Setup (one-time)

1. Settings -> Secrets and variables -> Actions -> New secret
   Name: PEPPER_API_KEY | Value: your Pepper Marketing API key
2. Commit .github/workflows/refresh-feeds.yml to main
3. Actions -> Refresh Pepper Ad Feeds -> Run workflow

Cron: 0 */6 * * * (00:00, 06:00, 12:00, 18:00 UTC)
