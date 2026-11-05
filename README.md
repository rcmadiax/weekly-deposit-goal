# Weekly Deposit Goal — iPhone PWA

A static, offline-capable weekly deposit calculator. No backend or third-party services required.

## Publish to GitHub Pages

1. Create a new **public** GitHub repository named `weekly-deposit-goal`.
2. Upload **all five app files** (`index.html`, `manifest.webmanifest`, `sw.js`, `icon-192.png`, `icon-512.png`) into the repository root. You may upload `README.md` too.
3. In repository **Settings → Pages**, under **Build and deployment**, choose **Deploy from a branch**, then **main** and **/(root)**. Save.
4. When GitHub Pages finishes publishing, visit `https://YOUR-USERNAME.github.io/weekly-deposit-goal/` on iPhone in Safari.
5. Tap **Share → Add to Home Screen → Add**.

## Data and backups

Entries auto-save to localStorage on the device. Use **Save weekly snapshot** for historical records, and **Export JSON backup** to save a portable backup in Files. Import replaces all locally saved data after confirmation. Data does **not** automatically sync between devices. Clearing site data, removing the PWA, or changing browsers can erase entries; keep exported backups.

The Shippo amount is an extra deduction; don't enter amounts already included in pending-order shipping estimates.

## Version 1.1 changes

- Added Mercari to available balances and the weekly total.
- Renamed pending PayPal orders to **Pending Shippo orders** (same $6.25/order shipping estimate).
- Fixed iPhone date field sizing in Weekly history.
- Existing saved data and JSON backups remain compatible; the previous `paypalOrders` value is migrated into `shippoOrders` when loaded.
- Updated offline cache to refresh the app after publishing.
