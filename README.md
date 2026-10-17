# TEAM KINSE Game Hub

## What's included
- `index.html` — landing page visitors can open.
- `lucky-zone.html` — Lucky Zone Showdown.
- `cultivation.html` — Cultivation All-in-One Calculator.
- Landing page also links to the external [Shops-Worgen site](https://worgen475-lab.github.io/Shops-Worgen/).

## Persistence
Both pages save progress using browser `localStorage`:
- Cultivation Calculator: input values and selected methods.
- Lucky Zone: fund balance, selected chip, lucky-zone hit/miss history and counters.

This is per browser/device, not a shared account database. A visitor who returns using the same browser on the same device should retain their saved state. If they clear site data, use private/incognito mode, or switch devices/browsers, their saved state may not be available. The Lucky Zone game refunds unfinished bets when reopened, while keeping saved funds and history.

## Publish it for visitors
1. Extract the ZIP.
2. Create a free static site on Netlify or GitHub Pages.
3. Upload the three HTML files to the site's publish folder (keep their filenames together).
4. Publish, then share the site's public URL.

No build step or server is needed for this browser-local version.

## If you need accounts and cross-device persistence
A static website cannot securely keep each person's progress on a server by itself. For users to log in and have their own sessions follow them across devices, add authentication and a database (for example Supabase or Firebase) and store each user's game state under their account. That requires backend configuration and privacy/security rules.

- Landing page also links to [WePlay Philippines](https://weplayapp.com/en-PH/).
