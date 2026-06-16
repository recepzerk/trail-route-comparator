# Trail Route Comparator 🏔️

**Know what to expect. Before race day.**

Trail Route Comparator analyzes two GPX files side by side and tells you how your target race compares to a course you've already run — in effort, not just distance. Upload a reference route with your finish time and get a science-backed estimate for the new one.

🔗 **[Live Demo](https://recepzerk.github.io/trail-route-comparator)**

---

## What It Does

Upload two GPX files — a reference route you've already run and a target route you're preparing for — and get:

- **Effort Verdict** — how much harder or easier the target route is, as a percentage
- **Finish Time Estimate** — projected time based on your reference performance and the effort difference
- **Key Metrics** — distance, elevation gain, flat-equivalent distance, effort ratio, runnable terrain, walk zones
- **Terrain Distribution** — side-by-side breakdown of runnable, uphill, walk zone, and steep descent sections
- **Effort Distribution** — first half vs second half effort ratio for both routes, with gain/loss asymmetry
- **Race Strategy Advice** — plain-language guidance based on how the course is structured
- **Elevation Profiles** — visual comparison of both routes
- **Descent Warning** — flags higher leg damage risk when steep descents increase significantly

---

## Critical Zone Criteria

All thresholds are derived from Minetti's research on the metabolic cost of gradient running.

| Zone | Gradient | What it means |
|---|---|---|
| ⚡ Runnable | −8% to +10% | Efficient terrain for most trail runners |
| ⬆️ Moderate Uphill | 10–15% | Runnable for strong trail runners — others should walk |
| 🚶‍♂️ Walk Recommended | 15–20% | Walking is more efficient for most runners |
| 🚶 Walk Here | 20%+ | Running is metabolically counterproductive |
| ⚠️ Protect Your Legs | ≤ −15% | Steep descent — eccentric muscle damage risk |

---

## Effort Ratio Scale

Based on Minetti flat-equivalent ratio (actual effort vs flat-ground equivalent):

| Ratio | Level |
|---|---|
| < 1.05 | Easy |
| 1.05 – 1.20 | Moderate |
| 1.20 – 1.45 | Challenging |
| 1.45+ | Extreme |

---

## How to Use

1. Export your **reference GPX** from Strava, Komoot, Garmin Connect, or the official race website
2. Export your **target race GPX** from the same sources
3. Open [Trail Route Comparator](https://recepzerk.github.io/trail-route-comparator)
4. Upload the reference GPX and enter your finish time on that route
5. Upload the target GPX
6. Click **Compare Routes**
7. Review your effort comparison, time estimate, and race strategy

**Tip:** Official race GPX files tend to have better elevation accuracy than GPS watch recordings.

---

## Data Limitations

- Elevation data comes from the GPS device, not a barometric altimeter — accuracy may vary ±5–10%
- Surface conditions (mud, snow, loose rock) can increase actual effort by 10–30% beyond what gradient alone suggests
- This tool does not account for individual fitness level, heat, hydration, or cumulative fatigue
- Time estimates assume consistent relative effort across both routes
- All outputs are guidelines, not prescriptions

---

## Scientific References

This tool's critical zone thresholds and flat-equivalent calculations are based on the following peer-reviewed research:

- Minetti AE, Ardigò LP, Reinach E, Saibene F. (1994). *Mechanical determinants of the minimum energy cost of gradient running in humans.* Journal of Experimental Biology, 195, 211–225.
- Minetti AE, Moia C, Roi GS, Susta D, Ferretti G. (2002). *Energy cost of walking and running at extreme uphill and downhill slopes.* Journal of Applied Physiology, 93, 1039–1046.

---

## Tech Stack

Vanilla HTML, CSS, and JavaScript. No dependencies, no frameworks, no backend.
Works entirely in the browser — your GPX files never leave your device.

---

## Part of a Series

This tool is part of a collection of running tools built for the running community:

- 🏔️ [Trail Run Grader](https://recepzerk.github.io/trail-run-grader) — analyze a single GPX for critical zones
- 🎵 [Pace → Playlist](https://recepzerk.github.io/pace-to-playlist) — running music matched to your pace
- 🌤️ [What to Wear?](https://recepzerk.github.io/running-outfit-weather) — outfit recommendations by weather
- ✍️ [Name Your Run](https://recepzerk.github.io/name-your-run) — AI-generated run names and motivational quotes

---

## License

MIT License — free to use, modify, and share.
