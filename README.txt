SÉSAME D’ESPRIT — PWA PACKAGE

CONTENTS
- index.html: your student management app, prepared for installation
- manifest.webmanifest: app name, icon, and standalone display settings
- service-worker.js: basic app-shell caching (the Supabase data still needs internet)
- icon-192.png and icon-512.png: Android/PWA icons

NEXT STEPS (PHONE-ONLY)
1. Upload ALL five files to the ROOT of a GitHub repository (not inside another folder).
2. In GitHub, open Settings > Pages. Choose Deploy from a branch, select main and /(root), then Save.
3. Wait for GitHub Pages to publish the HTTPS website.
4. Open the published HTTPS URL in PWABuilder (https://www.pwabuilder.com/).
5. Follow its Android package flow. Review signing/package options; do not share signing keys.

IMPORTANT SECURITY NOTE
This HTML app contains a Supabase client configuration. Before making the repository public, confirm that the Supabase key is only the publishable/anon key and that Row Level Security is enabled with restrictive policies on every table. Never publish a service_role/secret key. A public website makes its HTML source viewable.

OFFLINE NOTE
The service worker caches the app shell only. Supabase login and database operations still require an internet connection.
