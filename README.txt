# Craeven Dragonlord PWA

This package converts the iPhone-optimized Craeven character sheet into a Progressive Web App (PWA).

## What is included
- `index.html` — the app itself
- `manifest.webmanifest` — app metadata
- `service-worker.js` — offline support
- `icons/` — Home Screen / app icon files made from your uploaded Craeven artwork

## How to use it
1. Upload all files in this folder to a small HTTPS host (GitHub Pages, Netlify, or Cloudflare Pages all work).
2. Open the hosted `index.html` URL in Safari on your iPhone.
3. Tap **Share** → **Add to Home Screen**.
4. The app will install with the Craeven icon and run in standalone mode.

## Notes
- The character sheet keeps using local browser storage on the device where it is installed.
- If you install it on a new device/browser, it starts fresh unless you restore from backup JSON.
- After you change app files in the future, you may need to refresh once online so the service worker can update the cached copy.
