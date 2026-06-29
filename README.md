# Croatia · Dubrovnik → Split · 19–25 September

A single-page trip-planning board to kick around with the crew. It lays out a
**fixed shape** for the week — three nights in Dubrovnik while everyone arrives,
then a flight home from Split — and offers **three "roads north"** to choose
between (or decide on mid-trip, off the weather).

Open `index.html` in any browser. Everything is in that one file.

## What's in it

- **Who's-coming strip** — the staggered arrivals (you land the 19th, the last
  friend on the 21st) mapped across the week.
- **Maps** (Leaflet + OpenStreetMap) — an overview of all three routes, a
  Dubrovnik day-trip map, and a focused map per route with the drive (solid)
  and ferry (dashed) legs.
- **Day-by-day schedule** — every day from Sept 19–25 broken into
  **morning / afternoon / evening**, with a category filter (lookout, old town,
  food, swim, hidden gem, on the road).
- **Photos** of the key places, and a local-first **food guide** (konobas,
  markets, one splurge max).
- American units throughout (miles, feet, °F).

## Three routes

- **A — Mountains & Coast** *(best fit)*: Dubrovnik → Makarska (Biokovo) → Omiš → Split.
- **B — Central Dalmatia & Islands**: Dubrovnik → Split → Brač / Hvar.
- **C — Southern Slow Road**: Dubrovnik → Korčula → Split.

## Publishing it online

It's a static site, so any static host works. The simplest is **GitHub Pages**:

1. Push this repo to GitHub (already on the working branch).
2. In the repo's **Settings → Pages**, set the source to the branch (or `main`)
   and the root folder.
3. Pages serves `index.html` at the published URL.

## Notes

- Maps need an internet connection (tiles from OpenStreetMap, Leaflet from a CDN).
- Photos load from **Wikimedia Commons** contributors (various Creative Commons
  licenses); if any single image can't load it falls back to a captioned tile,
  so nothing shows broken. Swap in your own photos by editing the `PH` object in
  `index.html`.
- It's a discussion draft — some days (the islands especially) are alternatives
  you won't all do together. Reconfirm 2026 ferry schedules, Biokovo hours
  (pp-biokovo.hr) and opening times close to travel.
