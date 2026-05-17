# Augusta CSRA Commercial Listings Map

Auto-updated daily at 6:15 AM (weekdays). Covers all active commercial listings across 4 companies in the Augusta/CSRA market.

## Companies

| Company | Marker | Count |
|---|---|---|
| Jordan Trotter | Red | ~322 |
| Meybohm | Blue | ~168 |
| Sherman & Hemstreet | Green | ~29 |
| Southeastern | Yellow | ~19 |

## Open in Google Earth (one-time setup)

1. Go to [earth.google.com/web](https://earth.google.com/web/)
2. Sign in with your Google account
3. Click the menu (top left) → **Projects** → **New Project** → **Create KML file**
4. In the new project, click **Add to Project** → **Network Link**
5. Name: `Augusta CSRA Listings`
6. URL: `https://raw.githubusercontent.com/WatersJordan/augusta-listings-map/main/augusta_listings.kml`
7. Refresh: **Periodically** → every **24 hours**
8. Click OK — all listings load on the map
9. Click **Share** → **Anyone with the link can view** → copy and send the link

## Raw KML URL

```
https://raw.githubusercontent.com/WatersJordan/augusta-listings-map/main/augusta_listings.kml
```

## How it updates

Every weekday morning the sync script:
1. Scrapes all 4 companies
2. Updates `data/augusta_listings.db` and `data/augusta_listings.xlsx`
3. Regenerates `data/augusta_listings.kml` and pushes here
4. Google Earth refreshes automatically via the Network Link
