# Tulnix — mobile-first price comparison prototype

## Included
- `index.html`: responsive, mobile-first web app prototype.
- `manifest.webmanifest`: PWA manifest.
- `sw.js`: basic service worker for shell caching.
- `products_template.csv`: blank import/template schema.
- `README.txt`: this file.

## Current working features
- Search product listings by name, store, or category.
- Category filters and sorting.
- Add/edit product listings locally in the browser.
- Optional price, source status, last-checked timestamp, and merchant URL.
- External store link button.
- No seeded prices or invented live offers.

## Important limitations
- Listings are saved in the current browser's local storage only. They are not shared with other users/devices and may be lost if browser storage is cleared.
- No retailer API is connected. Do not describe this as live price comparison yet.
- “Verified feed/API” is a user-selected label in this prototype, not automatic proof. Use it only after your source actually verifies the listing.
- No Android APK is included. This is an installable PWA shell when hosted over HTTPS; Android browser install support varies.
- Production requires an approved data source, shared backend/database, monitoring, privacy policy, terms, and affiliate disclosures.

## Test locally
Open `index.html` in a browser. Some PWA features (service worker and installability) require HTTPS hosting or localhost. Local file opening may disable those features.

## Suggested free deployment path
1. Create a GitHub account and repository.
2. Upload `index.html`, `manifest.webmanifest`, and `sw.js` to the repository root.
3. Enable GitHub Pages in repository Settings > Pages, deploy from the main branch/root.
4. Open the published HTTPS URL in Chrome on Android.
5. Use Chrome menu > Add to Home screen / Install app, if available.
Check current GitHub Pages terms and usage limits before commercial launch.

## Next steps before public launch
1. Pick a final brand name and check trademarks, company names, and domain/social handles.
2. Apply for retailer affiliate programs and confirm data/API rights.
3. Connect approved data feeds via a secure backend; do not expose secret API keys in client-side HTML.
4. Build a shared database and reliable product-variant matching.
5. Add price freshness rules, delivery/fee handling, clear “last checked” labels, and error handling.
6. Publish privacy policy, terms, affiliate disclosure, and contact details.
7. Consider a native Android package only after the PWA and data model are validated.
