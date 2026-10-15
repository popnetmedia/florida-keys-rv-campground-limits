# Method

## Scope

Every RV campground in the Florida Keys that flkeysrvrental.com covers on its campground and area
pages, as of 2026-10-14: 22 rows. A campground is in the set when its own page, or the agency's,
could be read on the read date. Left out: El Mar RV Resort (website redirected to a parking page),
Breezy Pines RV Estates (no website found), Sun Outdoors Sugarloaf Key (its page redirected to an
index that does not list it). Long Key State Park is included because it takes no RVs, and people
book it expecting it does.

## Reading the rules

Each campground's own website, or for state parks the Florida State Parks park page and its
reservation system (reserve.floridastateparks.org), read on 2026-10-08. Several of these sites refuse
automated requests and were read in a normal browser session. Limits are quoted or closely
paraphrased. Where two official pages disagree, both are recorded in the same cell. Where a page is
silent, the cell says `not published`. Nothing is estimated and no third-party directory figure is
used as a limit (Grassy Key's directory claim of 62 ft is noted, not used).

## Mile markers

Recorded only where a source states one, with that source in `mile_marker_source`. An Overseas
Highway street number (for example 102601) is close to a mile marker in practice, but no source says
so for these addresses, so it is not converted.

## Coordinates

Read 2026-10-14. In order of preference:

1. `operator`: coordinates the campground operator publishes on its own page (a GPS line,
   schema.org GeoCoordinates, a property map marker, or its own directions link). 6 rows.
2. `geocoded`: OpenStreetMap Nominatim, from the published street address; where the address did not
   resolve, from the campground's name, and the row says so. 11 rows (8 by address, 3 by name). One
   request per 1.2 seconds, descriptive User-Agent, 48 requests.
3. `none`: neither worked; latitude and longitude are blank. 5 rows.

No government page read publishes coordinates for these parks.

## Columns

| Column | Meaning |
|---|---|
| `id` | Stable slug |
| `name` | Campground name as published |
| `area` | Upper Keys, Middle Keys, Lower Keys or Key West |
| `key` | The key it sits on, from its address or page |
| `operator_type` | state park, private, owner community, military |
| `mile_marker`, `mile_marker_source` | Only where a source states it |
| `address` | As published |
| `length_limit` | The published limit in words, or `not published` |
| `length_limit_ft` | The number in feet where one is published (Bahia Honda: the tightest loop; Long Key: 0, no RV sites); blank where none |
| `limit_type` | What the number means: prohibited above, site capacity, call first above, select sites only, minimum only |
| `height_limit` | Published clearance limits |
| `hookups`, `pets`, `generator`, `stay_rules`, `delivered_rentals`, `other_rules` | As published, or `not published` |
| `owning_page` | The flkeysrvrental.com page that covers this campground |
| `source_url`, `source_url_2` | Where the rule was read |
| `read_date` | Date the rule was read |
| `latitude`, `longitude`, `coordinate_method`, `coordinate_note` | See Coordinates above |

## Related measurement (not in the CSV)

flkeysrvrental.com counts the Outdoorsy RVs whose host's published delivery radius reaches each
campground and compares each listed length with the campground's cap. On 2026-10-14, 11 of the 68
RVs that could reach Bahia Honda listed 23 ft or less. That count is live and recomputed every six
hours on https://flkeysrvrental.com/destinations/bahia-honda, so it is not frozen into this set.
