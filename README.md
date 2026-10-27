# Yapper

A modern, responsive chat website powered by Supabase.

## Features
- Email/password sign-up and sign-in
- Public chat rooms: lobby, gaming, and memes
- Realtime message updates
- Responsive layout for desktop and mobile

## Backend
- Supabase project ref: `stofcbzyuxvkycjmxudk`
- Region: Canada Central
- The website uses the public publishable key only. Never put a Supabase `service_role` key in browser code.

## Run locally
1. Download or clone this repository.
2. Open a terminal in the repository folder.
3. Run `py -m http.server 8000` (or `python -m http.server 8000`).
4. Open http://localhost:8000.

## Deploy to GitHub Pages
1. Open this repository's **Settings → Pages**.
2. Set the source to **GitHub Actions**.
3. The workflow in `.github/workflows/pages.yml` deploys the site when you push to `main`.

## Notes
This is an initial build, not a production-audited messaging platform. Supabase Auth redirect URLs and email confirmation should be configured for the final website domain. The message query expects a `public.messages` table with `room_name`, `user_id`, `content`, and `created_at` fields, plus appropriate Row Level Security policies.