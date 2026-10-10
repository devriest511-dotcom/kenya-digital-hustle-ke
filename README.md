# Kenya Digital Hustle KE — website starter

A responsive, installable Progressive Web App (PWA) starter for a Kenya-first opportunity directory. This version is a front-end MVP, not yet a live multi-user service.

## Included now
- Responsive website layout for mobile and desktop
- Search and category/work-mode filters
- Save/bookmark listings in the current browser
- Opportunity submission form that stores pending suggestions in the current browser only
- Resource directory linking to official platform pages
- PWA manifest, service worker and app icon
- Basic privacy notice

## Important status note
The directory currently contains **resource links, not verified live vacancies**. Availability, country eligibility, pay and deadlines must be checked on the official source. User submissions remain local to the browser until a backend is configured. There is no shared admin dashboard, live database, automated ingestion, push notification system, or Play Store package in this starter.

## Preview locally
Open `index.html` in a browser. For PWA/service-worker testing, serve this folder over HTTPS or localhost. Example if Python is installed:

```bash
python -m http.server 8000
```

Then open `http://localhost:8000`.

## Publish free with GitHub Pages
1. Create/sign in to a GitHub account and create a public repository, e.g. `kenya-digital-hustle-ke`.
2. Upload all files and folders from this project (keep the root `index.html` in the repository root).
3. In repository Settings → Pages, choose deploy from branch, select `main` and `/ (root)`, then Save.
4. Wait for GitHub Pages to provide the public HTTPS URL. Test the site on your phone.
5. To install on Android, open the HTTPS website in Chrome and use the browser menu → **Install app** or **Add to Home screen** (wording varies).

## Next build stage: shared data and moderation
Use Supabase or another backend for authentication, listings, submissions and moderator roles. The public browser must never contain a service-role/secret key. Add an admin queue where all incoming opportunities begin as `pending`, moderators verify the official source and eligibility, and only approved records are publicly visible. Automated feeds should create pending records, not publish automatically.

## Brand channel
Telegram: https://t.me/KenyaDigitalHustleKE
