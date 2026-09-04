# NavAI — Intelligent Offline Navigation

Offline-first Progressive Web App built from the supplied NavAI voice-navigation prototype.

## Included
- Installable PWA shell
- Service-worker caching for offline launch
- Offline navigation UI and simulated dead reckoning
- Voice turn announcements using the browser Web Speech API
- Device motion and orientation readings when the browser exposes them
- Online/offline status detection
- GPS-loss simulation and confidence decay
- Responsive desktop and mobile interface
- No external JavaScript libraries, CDNs, fonts, or network map tiles required

## Important limitation
This build works without internet as an **offline application**, but the supplied prototype does not contain a real offline road-routing engine or offline map database. The map shown is a local visual dashboard and the route/directions are simulated. Real offline navigation requires bundling map/routing data (for example, a local vector/raster map package and an offline routing engine).

## Run
Serve the repository from HTTPS or localhost so service workers can run. Open `index.html` through the server, install NavAI from the browser's install prompt/menu, then launch it once while online so the shell is cached. After that, the app shell can open without internet.

## GitHub Pages
Enable GitHub Pages for the `main` branch. The site can then be installed as a PWA on supported browsers. Service workers require a secure context; GitHub Pages provides HTTPS.
