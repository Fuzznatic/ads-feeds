# ads-feeds

Automated feed cache for Atolls / Pepper ad creatives.
GitHub Actions fetches from the Pepper Marketing API every 6 hours using a secret API key
and commits the results as static JSON. Banners fetch from raw GitHub URLs — no API key
is ever exposed in any creative.

> Last updated: **2026-07-11 03:30 UTC**

---

## Feed URLs (use these in banners)

### Locale Feeds
| Feed | Raw URL |
|------|---------|
| AMAZONMX2026 (Amazonmx2026) | `https://raw.githubusercontent.com/Fuzznatic/ads-feeds/main/feeds/Amazonmx2026.json` |
| DE (DE) | `https://raw.githubusercontent.com/Fuzznatic/ads-feeds/main/feeds/DE.json` |
| GAMING (Gaming) | `https://raw.githubusercontent.com/Fuzznatic/ads-feeds/main/feeds/Gaming.json` |
| DE-CAR-MOTORCYCLE (DE-Car-Motorcycle) | `https://raw.githubusercontent.com/Fuzznatic/ads-feeds/main/feeds/DE-Car-Motorcycle.json` |
| DE-ELECTRONICS (DE-Electronics) | `https://raw.githubusercontent.com/Fuzznatic/ads-feeds/main/feeds/DE-Electronics.json` |
| DE-FASHION-ACCESSORIES (DE-Fashion-Accessories) | `https://raw.githubusercontent.com/Fuzznatic/ads-feeds/main/feeds/DE-Fashion-Accessories.json` |
| DE-GAMING (DE-Gaming) | `https://raw.githubusercontent.com/Fuzznatic/ads-feeds/main/feeds/DE-Gaming.json` |
| DE-HEALTH-BEAUTY (DE-Health-Beauty) | `https://raw.githubusercontent.com/Fuzznatic/ads-feeds/main/feeds/DE-Health-Beauty.json` |
| DE-HOME-LIVING (DE-Home-Living) | `https://raw.githubusercontent.com/Fuzznatic/ads-feeds/main/feeds/DE-Home-Living.json` |
| DE-SPORTS-OUTDOOR (DE-Sports-Outdoor) | `https://raw.githubusercontent.com/Fuzznatic/ads-feeds/main/feeds/DE-Sports-Outdoor.json` |
| DE-TRAVEL (DE-Travel) | `https://raw.githubusercontent.com/Fuzznatic/ads-feeds/main/feeds/DE-Travel.json` |
| FR-CAR-MOTORCYCLE (FR-Car-Motorcycle) | `https://raw.githubusercontent.com/Fuzznatic/ads-feeds/main/feeds/FR-Car-Motorcycle.json` |
| FR-ELECTRONICS (FR-Electronics) | `https://raw.githubusercontent.com/Fuzznatic/ads-feeds/main/feeds/FR-Electronics.json` |
| FR-FASHION-ACCESSORIES (FR-Fashion-Accessories) | `https://raw.githubusercontent.com/Fuzznatic/ads-feeds/main/feeds/FR-Fashion-Accessories.json` |
| FR-GAMING (FR-Gaming) | `https://raw.githubusercontent.com/Fuzznatic/ads-feeds/main/feeds/FR-Gaming.json` |
| FR-HOME-LIVING (FR-Home-Living) | `https://raw.githubusercontent.com/Fuzznatic/ads-feeds/main/feeds/FR-Home-Living.json` |
| FR-TRAVEL (FR-Travel) | `https://raw.githubusercontent.com/Fuzznatic/ads-feeds/main/feeds/FR-Travel.json` |
| MX-CAR-MOTORCYCLE (MX-Car-Motorcycle) | `https://raw.githubusercontent.com/Fuzznatic/ads-feeds/main/feeds/MX-Car-Motorcycle.json` |
| MX-ELECTRONICS (MX-Electronics) | `https://raw.githubusercontent.com/Fuzznatic/ads-feeds/main/feeds/MX-Electronics.json` |
| MX-FASHION-ACCESSORIES (MX-Fashion-Accessories) | `https://raw.githubusercontent.com/Fuzznatic/ads-feeds/main/feeds/MX-Fashion-Accessories.json` |
| MX-GAMING (MX-Gaming) | `https://raw.githubusercontent.com/Fuzznatic/ads-feeds/main/feeds/MX-Gaming.json` |
| MX-HEALTH-BEAUTY (MX-Health-Beauty) | `https://raw.githubusercontent.com/Fuzznatic/ads-feeds/main/feeds/MX-Health-Beauty.json` |
| MX-HOME-LIVING (MX-Home-Living) | `https://raw.githubusercontent.com/Fuzznatic/ads-feeds/main/feeds/MX-Home-Living.json` |
| MX-SPORTS-OUTDOOR (MX-Sports-Outdoor) | `https://raw.githubusercontent.com/Fuzznatic/ads-feeds/main/feeds/MX-Sports-Outdoor.json` |
| MX-TRAVEL (MX-Travel) | `https://raw.githubusercontent.com/Fuzznatic/ads-feeds/main/feeds/MX-Travel.json` |
| NL-CAR-MOTORCYCLE (NL-Car-Motorcycle) | `https://raw.githubusercontent.com/Fuzznatic/ads-feeds/main/feeds/NL-Car-Motorcycle.json` |
| NL-ELECTRONICS (NL-Electronics) | `https://raw.githubusercontent.com/Fuzznatic/ads-feeds/main/feeds/NL-Electronics.json` |
| NL-FASHION-ACCESSORIES (NL-Fashion-Accessories) | `https://raw.githubusercontent.com/Fuzznatic/ads-feeds/main/feeds/NL-Fashion-Accessories.json` |
| NL-GAMING (NL-Gaming) | `https://raw.githubusercontent.com/Fuzznatic/ads-feeds/main/feeds/NL-Gaming.json` |
| NL-HEALTH-BEAUTY (NL-Health-Beauty) | `https://raw.githubusercontent.com/Fuzznatic/ads-feeds/main/feeds/NL-Health-Beauty.json` |
| NL-HOME-LIVING (NL-Home-Living) | `https://raw.githubusercontent.com/Fuzznatic/ads-feeds/main/feeds/NL-Home-Living.json` |
| NL-SPORTS-OUTDOOR (NL-Sports-Outdoor) | `https://raw.githubusercontent.com/Fuzznatic/ads-feeds/main/feeds/NL-Sports-Outdoor.json` |
| NL-TRAVEL (NL-Travel) | `https://raw.githubusercontent.com/Fuzznatic/ads-feeds/main/feeds/NL-Travel.json` |
| PL-ELECTRONICS (PL-Electronics) | `https://raw.githubusercontent.com/Fuzznatic/ads-feeds/main/feeds/PL-Electronics.json` |
| PL-FASHION-ACCESSORIES (PL-Fashion-Accessories) | `https://raw.githubusercontent.com/Fuzznatic/ads-feeds/main/feeds/PL-Fashion-Accessories.json` |
| PL-GAMING (PL-Gaming) | `https://raw.githubusercontent.com/Fuzznatic/ads-feeds/main/feeds/PL-Gaming.json` |
| PL-HOME-LIVING (PL-Home-Living) | `https://raw.githubusercontent.com/Fuzznatic/ads-feeds/main/feeds/PL-Home-Living.json` |
| PL-TRAVEL (PL-Travel) | `https://raw.githubusercontent.com/Fuzznatic/ads-feeds/main/feeds/PL-Travel.json` |
| UK-CAR-MOTORCYCLE (UK-Car-Motorcycle) | `https://raw.githubusercontent.com/Fuzznatic/ads-feeds/main/feeds/UK-Car-Motorcycle.json` |
| UK-CORSAIR (UK-Corsair) | `https://raw.githubusercontent.com/Fuzznatic/ads-feeds/main/feeds/UK-Corsair.json` |
| UK-ELECTRONICS (UK-Electronics) | `https://raw.githubusercontent.com/Fuzznatic/ads-feeds/main/feeds/UK-Electronics.json` |
| UK-FASHION-ACCESSORIES (UK-Fashion-Accessories) | `https://raw.githubusercontent.com/Fuzznatic/ads-feeds/main/feeds/UK-Fashion-Accessories.json` |
| UK-GAMING (UK-Gaming) | `https://raw.githubusercontent.com/Fuzznatic/ads-feeds/main/feeds/UK-Gaming.json` |
| UK-HOME-LIVING (UK-Home-Living) | `https://raw.githubusercontent.com/Fuzznatic/ads-feeds/main/feeds/UK-Home-Living.json` |
| UK-SPORTS-OUTDOOR (UK-Sports-Outdoor) | `https://raw.githubusercontent.com/Fuzznatic/ads-feeds/main/feeds/UK-Sports-Outdoor.json` |
| UK-TRAVEL (UK-Travel) | `https://raw.githubusercontent.com/Fuzznatic/ads-feeds/main/feeds/UK-Travel.json` |
| AT-AMAZONFEED (at-AmazonFeed) | `https://raw.githubusercontent.com/Fuzznatic/ads-feeds/main/feeds/at-AmazonFeed.json` |
| AT (pepper.com AT) | `https://raw.githubusercontent.com/Fuzznatic/ads-feeds/main/feeds/at.json` |
| DE-ALIBABAFEED (de-AlibabaFeed) | `https://raw.githubusercontent.com/Fuzznatic/ads-feeds/main/feeds/de-AlibabaFeed.json` |
| DE-AMAZONFEED (de-AmazonFeed) | `https://raw.githubusercontent.com/Fuzznatic/ads-feeds/main/feeds/de-AmazonFeed.json` |
| DE (mydealz) | `https://raw.githubusercontent.com/Fuzznatic/ads-feeds/main/feeds/de.json` |
| ES (chollometro) | `https://raw.githubusercontent.com/Fuzznatic/ads-feeds/main/feeds/es.json` |
| FR-AMAZONFEED (fr-AmazonFeed) | `https://raw.githubusercontent.com/Fuzznatic/ads-feeds/main/feeds/fr-AmazonFeed.json` |
| FR (dealabs) | `https://raw.githubusercontent.com/Fuzznatic/ads-feeds/main/feeds/fr.json` |
| MX-AMAZONFEED (mx-AmazonFeed) | `https://raw.githubusercontent.com/Fuzznatic/ads-feeds/main/feeds/mx-AmazonFeed.json` |
| MX (promodescuentos) | `https://raw.githubusercontent.com/Fuzznatic/ads-feeds/main/feeds/mx.json` |
| NL-AMAZONFEED (nl-AmazonFeed) | `https://raw.githubusercontent.com/Fuzznatic/ads-feeds/main/feeds/nl-AmazonFeed.json` |
| NL (pepper.com NL) | `https://raw.githubusercontent.com/Fuzznatic/ads-feeds/main/feeds/nl.json` |
| PL-AMAZONFEED (pl-AmazonFeed) | `https://raw.githubusercontent.com/Fuzznatic/ads-feeds/main/feeds/pl-AmazonFeed.json` |
| PL (pepper.com PL) | `https://raw.githubusercontent.com/Fuzznatic/ads-feeds/main/feeds/pl.json` |
| SE (pepper.com SE) | `https://raw.githubusercontent.com/Fuzznatic/ads-feeds/main/feeds/se.json` |
| UK-ALIBABAFEED (uk-AlibabaFeed) | `https://raw.githubusercontent.com/Fuzznatic/ads-feeds/main/feeds/uk-AlibabaFeed.json` |
| UK-AMAZONFEED (uk-AmazonFeed) | `https://raw.githubusercontent.com/Fuzznatic/ads-feeds/main/feeds/uk-AmazonFeed.json` |
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
