# KP Muhurat — Android Installable Web App

This is a separate project from the original KP Muhurat Web 2.0 repository.

## Files
- `index.html` — application
- `manifest.webmanifest` — Android/PWA name, display mode, theme and icons
- `kp-icon-192.png`, `kp-icon-512.png` — app icons
- `sw.js` — service worker for app-shell caching

## Publish with GitHub Pages
1. Upload all five files to the root of the `kp-muhurat-daily-schedule` repository (not only `index.html`).
2. Keep GitHub Pages enabled for the `main` branch and `/(root)`.
3. Open the published HTTPS site in Google Chrome on Android.
4. Tap the page's **Install app** button, or Chrome menu `⋮` → **Install app** / **Add to Home screen**.
5. Confirm the name and tap Install. The KP Muhurat icon should appear on the home screen/app list.

## Notes
- The site must be served over HTTPS for service workers and PWA installation; GitHub Pages provides HTTPS.
- The service worker caches the local app shell. Features depending on external services or resources may still need an internet connection.
- This is an installable web app (PWA), not a Play Store APK.
- Calculation logic is not intentionally changed by the PWA packaging. Validate important calculations against your reference before operational use.

## Date-range behavior (updated)
- Selecting **Date** or **To date** does not run a calculation and does not switch tabs.
- Select both dates and any other inputs, then tap **Show**. The app calculates the selected range and opens **Results**.
- After updating the files in GitHub Pages, refresh the site. The service-worker cache version is bumped so the corrected app shell can replace the older cached copy.
