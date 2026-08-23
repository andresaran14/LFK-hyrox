# HYROX LFK Tracker

A training tracker, workout generator, and multi-format interval timer (Interval, Tabata, EMOM, AMRAP, For Time) for Louisa & Andrés's HYROX prep — covering HYROX stations, CrossFit movements, and strength lifts. Installable as an app on iPhone/iPad/Android.

## Deploy to GitHub Pages

1. Create a new repository on GitHub (e.g. `hyrox-lfk-tracker`). Public is easiest (private repos need a paid plan for Pages).
2. Upload **all** the files in this folder to the repo — they all sit at the top level, no subfolders, so select/drag them all at once:
   ```
   index.html
   manifest.json
   service-worker.js
   apple-touch-icon-180.png
   favicon-32.png
   icon-16.png
   icon-120.png
   icon-152.png
   icon-167.png
   icon-192.png
   icon-512.png
   README.md
   ```
   On the repo page: **Add file → Upload files**, select/drag them all in together, then Commit.
3. Go to **Settings → Pages**.
4. Under **Source**, choose **Deploy from a branch** → branch `main`, folder `/ (root)` → Save.
5. After a minute or two you'll get a link like:
   `https://YOUR-USERNAME.github.io/hyrox-lfk-tracker/`

## Install on iPad / iPhone (Safari)

1. Open the link in **Safari** (must be Safari, not Chrome, for this to work on iOS).
2. Tap the **Share** icon → **Add to Home Screen**.
3. It installs with the LFK icon, opens full-screen — no browser bars.

If the icon looks wrong right after installing, it's almost always Safari caching the old page: delete the home-screen icon, go to **Settings → Safari → Advanced → Website Data**, delete the entry for your `github.io` domain, then reopen the link fresh in Safari and re-add it.

## Install on Android (Chrome)

Open the link in Chrome → **⋮** menu → **Add to Home screen** / **Install app**.

## How data is stored

This version saves sessions **locally in the browser on each device** — GitHub Pages only hosts static files, there's no shared database. That means:

- Louisa's phone and Andrés's phone each keep their own separate log.
- Use **Export data** (Progress tab) on one device to download a `.json` file, then **Import data** on the other to merge it in — imports are additive and won't duplicate sessions.
- Clearing Safari/Chrome site data or reinstalling erases local sessions, so export a backup occasionally.

## Updating later

If the app gets updated again, just re-upload the changed files to the same repo (overwrite `index.html` etc.) — Pages redeploys automatically, and your installed home-screen icon will load the new version next time it's opened.
