# Florida Keys RV campground length limits

The published RV length limit of every RV campground in the Florida Keys covered by
[flkeysrvrental.com](https://flkeysrvrental.com/), from Key Largo to Key West, in one table: 22
campgrounds (21 that take RVs, plus Long Key State Park, which takes none), each with its own source
URL and the date it was read.

Compiled by Florida Keys RV Rental, a finder for Outdoorsy RVs whose hosts deliver to the Keys.
Rules read 2026-10-08; map coordinates added 2026-10-14.

## What it shows

- **Bahia Honda State Park's Sandspur loop takes rigs up to 23 ft, measured hitch to bumper.** It is
  the tightest published length limit in the Keys.
- **15 of the 21 RV campgrounds publish no maximum length at all.** Five publish one (Pennekamp 40 ft
  on most sites, Curry Hammock 70 ft, Bahia Honda Sandspur 23 ft, Leo's 42 ft including racks, Boyd's
  45 ft in select sites). Big Pine Key RV Park asks you to call above 36 ft. Bluewater Key publishes
  only a 16 ft minimum.
- **Two official figures disagree at Pennekamp:** 40 ft on most sites per the park page, 62 in the
  reservation system. Both are recorded.

## Files

| File | What it is |
|---|---|
| `data/campgrounds.csv` | One row per campground, 26 columns (described in `METHOD.md`) |
| `data/campgrounds.json` | The same rows, plus a `meta` block with dates and licence |
| `METHOD.md` | How the set was compiled, what counts as a mile marker, how coordinates were placed |
| `SOURCES.md` | Every source URL with its read date |

## Licence

[CC BY 4.0](https://creativecommons.org/licenses/by/4.0/). Reuse it, with credit. Geocoded
coordinates derive from OpenStreetMap (© OpenStreetMap contributors, ODbL); if you reuse the
`latitude` and `longitude` of rows whose `coordinate_method` is `geocoded`, credit OpenStreetMap too.
The campground rules are facts published by each campground or agency; this set is the compilation.

## How to cite

> Florida Keys RV Rental (2026). *Florida Keys RV campground length limits* [Data set]. Rules read
> 8 October 2026. https://github.com/popnetmedia/florida-keys-rv-campground-limits. See also
> https://flkeysrvrental.com/destinations.

## Before you rely on a row

Campgrounds change their rules without notice. Each row carries the date its page was read. Call the
campground with your RV's overall length, hitch and rear rack included, before you book.

## Corrections

Open an issue with the campground, the rule as published now, and the URL. A correction is made only
from the campground's or agency's own page.

Florida Keys RV Rental owns no RVs, takes no campsite bookings, and is not affiliated with Florida
State Parks, Monroe County, the City of Key West or any campground listed.
