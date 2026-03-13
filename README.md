# Macro Calculator

A single-file PWA for tracking daily macros, built for a 1700-cal cut from 220 to 190 lbs.

**Live:** [mnorton77.github.io/Macro-calculator](https://mnorton77.github.io/Macro-calculator)

## Features

- **4 animated macro rings** (cal / protein / carbs / fat) with real-time +/- goal diffs in green or red
- **1700 cal · 200g P · 100g C · 55g F** targets baked in
- **Add Food** modal with search across 200+ offline foods, 10 Sioux Falls restaurants, and the full USDA FoodData Central API
- **UPC barcode lookup** via USDA + Open Food Facts fallback
- **Gram / Oz / Serving toggle** with per-100g math on every item
- **20 protein powders** (ON Gold Standard, Dymatize, Ghost, MyProtein, Isopure, etc.)
- **End of Day Check** button — asks if you had a protein shake, auto-detects if one's already logged, lets you pick & log one in 2 taps
- **Today's food log** with per-item macro tags and swipe-to-delete
- **7-day calorie bar chart** + macro averages with progress bars
- **30-day calorie trend** + macro averages
- **Weight tracking** — 220 to 190 progress bar, trend chart, honest "X lbs up from start" in red if you gain
- **Monday / Friday weigh-in banner** reminder
- **Restaurants:** The Attic, Culver's, Chick-fil-A, Jimmy John's, Jersey Mike's, Potbelly, Tavern Grill, Looks Eatery, Tinners Public House, Texas Roadhouse
- **Recent foods** tab for quick re-logging

## Tech

Single `index.html`, no build step. Dark mode, DM Sans + DM Mono fonts, Chart.js 4.4.0 from CDN, localStorage for everything. Deployed via GitHub Pages on `main`.

## APIs

| Service | Purpose |
|---------|---------|
| [USDA FoodData Central](https://fdc.nal.usda.gov/) | Food search + UPC lookup |
| [Open Food Facts](https://world.openfoodfacts.org/) | UPC barcode fallback |

