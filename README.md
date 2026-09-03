# NEET Preparation Website

Mobile-first student + admin UI starter.

## Run
Open `index.html` in a browser or deploy the folder to GitHub Pages/Netlify/Vercel.

## Supabase
Add the project URL and public anon key in `config.js`, then connect authentication/database/RLS/RPCs.

The UI already includes:
- Student dashboard
- Physics/Chemistry/Biology chapters
- Study material management
- Tests/quizzes
- Progress
- Bookmarks
- Wallet and coin economy UI
- Reward ad and daily bonus demo flows
- Admin material publishing and coin settings UI

For production, coin deductions, rewarded-ad verification, PDF access, test entry, refunds, and admin permissions must be enforced server-side with Supabase RPC/Edge Functions and RLS.
