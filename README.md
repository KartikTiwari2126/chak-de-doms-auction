# Chak De DoMS 2026 — GitHub Pages + Supabase Live Auction

## Files
- `index.html` — landing page
- `admin.html` — auction operator screen
- `display.html` — projector/public live screen
- `config.js` — Supabase URL + publishable key
- `schema_and_seed.sql` — database, RLS, Realtime and 96-player seed

## 1. Supabase
Your Supabase project is already configured in `config.js`. In the Supabase SQL Editor, run `schema_and_seed.sql` once.

Create one admin user under Authentication → Users.

## 2. Configure the site
The supplied Supabase Project URL and **publishable key** are already filled into `config.js`. Do not replace them with a `service_role` or secret key.

## 3. GitHub Pages
Create a GitHub repository and upload all files/folders from this directory. Then:
Settings → Pages → Deploy from branch → `main` → `/ (root)` → Save.

Your URLs will be:
- `https://YOUR-USERNAME.github.io/YOUR-REPO/`
- `https://YOUR-USERNAME.github.io/YOUR-REPO/admin.html`
- `https://YOUR-USERNAME.github.io/YOUR-REPO/display.html`

## Important
The Supabase Realtime connection handles live updates between the Admin and Display pages. Keep the auction tab active during the event because the free Supabase project can pause after prolonged inactivity.

The credential-looking text sent in chat was NOT added to this repository. If it is a password or secret key, do not publish it; rotate it in Supabase.
