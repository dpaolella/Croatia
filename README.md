# Croatia · Dubrovnik → Zagreb · 19–26 September

A single-page trip-planning board to kick around with the crew. It lays out a
**fixed shape** for the week — land in Dubrovnik Saturday morning the 19th,
converge on Split by Thursday the 24th, sleep at Plitvice Lakes Friday, and fly
home from Zagreb on Saturday evening the 26th — and offers **four itinerary
shapes** to choose between for the middle.

Open `index.html` in any browser. Everything is in that one file.

## What's in it

- **Who's-coming strip** — the staggered arrivals (you land the 19th, the last
  friend on Monday the 21st) mapped across the week, weekdays checked against
  the 2026 calendar.
- **Maps** (Leaflet + OpenStreetMap) — an overview of all four routes, a
  Dubrovnik day-trip map, a focused map per route, and the shared
  Split → Plitvice → Zagreb finale. Drive legs fetch real road geometry from
  OSRM at runtime; ferry legs are dashed.
- **Day-by-day schedule** — every day from Sept 19–26 broken into
  **morning / afternoon / evening**, with category filters and car/boat/foot
  mode pills.
- **Clickable photos** (lightbox) of the key places, a local-first **food
  guide**, a **car vs. boat cost comparison**, and logistics (timed-entry
  rules for Plitvice, Biokovo and Mljet included).
- American units throughout (miles, feet, °F).

## Four routes

- **D — Islands & Lakes** *(recommended)*: Dubrovnik → Mljet ×2 → Dubrovnik ×2
  → Korčula → Split → Plitvice. Car-free until Split; fits the staggered
  arrivals best (Mljet fills the solo window, and the ~11:10 Monday boat lands
  right as the last friend arrives).
- **A — Mountains & Coast**: Dubrovnik ×3 → Makarska (Biokovo) → Omiš → Split →
  Plitvice. The driver's trip.
- **B — Central Dalmatia & Islands**: Dubrovnik ×3 → Split → Brač / Hvar →
  Plitvice. The most swimming.
- **C — Southern Slow Road**: Dubrovnik ×3 → Korčula → Split → Plitvice. Food,
  wine, gentlest pace.

All four end the same way: everyone sleeps in Split on the 24th, drives to
Plitvice on the 25th (boat crews rent a car in Split; drivers already have
one), walks the lakes Saturday morning, and drops the car at Zagreb airport
for the evening flight home.

## Publishing it online

It's a static site, so any static host works. The simplest is **GitHub Pages**:

1. Push this repo to GitHub.
2. In the repo's **Settings → Pages**, set the source to `main` and the root
   folder.
3. Pages serves `index.html` at the published URL.

## Notes

- Maps need an internet connection (tiles from OpenStreetMap, Leaflet from a CDN).
- Photos load from **Wikimedia Commons** contributors (various Creative Commons
  licenses); if an image can't load it falls back to a captioned tile. Swap in
  your own photos by editing the `PH` object in `index.html`.
- It's a discussion draft — some days are alternatives you won't all do
  together. Reconfirm 2026 ferry schedules, Plitvice timed entry
  (np-plitvicka-jezera.hr), Biokovo hours (pp-biokovo.hr) and Mljet fees
  (np-mljet.hr) close to travel.
