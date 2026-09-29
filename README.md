# TalaStat: Stage 1 (GitHub Pages)

Compliance as a Service platform for micro enterprises. This folder is a static, installable web app (PWA). Data is stored on each user's own device (browser storage) for now.

## Files
- `index.html`: the app
- `manifest.webmanifest`: lets people install it to their home screen
- `service-worker.js`: makes it work offline
- `icons/`: logo and app icons

## Put it online with GitHub Pages
1. Sign in at github.com (create a free account if needed).
2. Click **+** (top right) > **New repository**. Name it `talastat`, set it to **Public**, and click **Create repository**.
3. Click **uploading an existing file**. Drag in **everything inside this folder**: `index.html`, `manifest.webmanifest`, `service-worker.js` and the whole `icons` folder. Click **Commit changes**.
4. Go to **Settings > Pages**. Under **Build and deployment**, choose **Deploy from a branch**, pick **main** and **/ (root)**, then **Save**.
5. Wait 1 to 3 minutes. Your app will be at `https://YOUR-USERNAME.github.io/talastat/`.

## Install on a phone
- **Android (Chrome):** open the link, tap the menu (three dots), then **Install app** or **Add to Home screen**.
- **iPhone (Safari):** open the link, tap **Share**, then **Add to Home Screen**.

## Updating the app later
1. Edit or replace the file on GitHub (open the file, click the pencil icon or **Add file > Upload files**, then commit).
2. In `service-worker.js`, change `CACHE_VERSION` (for example `talastat-v2`) so phones pick up the new version.

## Good to know
- Data lives only on the device and browser used. Clearing browser data, or switching phones, erases it.
- There are no user accounts yet. This is fine for demos and small pilots, but not for real bookkeeping.
- Tax figures are estimates. Have an accountant review the computations before real use.
- The next stage adds logins and a database (for example Supabase).
