# Product Power-Up — Landing Page CLAUDE.md

## What This Is
Marketing landing page for Pocket PM Coach (Product Power-Up), a gamified iOS PM interview coaching app. Purpose: App Store download CTAs, newsletter capture, plus App Store legal pages (Privacy Policy, Terms of Service, Support contact).

## Stack
- **Hosting**: GitHub Pages
- **Code**: Plain HTML/CSS — no frameworks
- **Email capture**: Newsletter form → Firebase `subscribeNewsletter` → Beehiiv API (key in Firebase secrets)
- **Domain**: Squarespace-managed domain pointing at GitHub Pages (`pocketpmcoach.app`)

## Repo
- GitHub username: andrewjwagner (andrewjwagner.dev email)
- Repo name: `product-power-up-site` (or similar)
- Pages branch: `main`, served from root

## File Structure
```
/
├── index.html         ← main landing page (App Store badge + newsletter + leaderboard teaser)
├── leaderboard.html   ← public all-time board (up to 100 real players)
├── app-store-badge.png ← official Apple Download on the App Store badge
├── privacy.html       ← Privacy Policy (required for App Store)
├── terms.html         ← Terms of Service (recommended for App Store)
└── support.html       ← Support/contact page (required for App Store)
```

## Beehiiv Integration
- Beehiiv account: andrewjwagner.dev email
- Newsletter publication ID: `pub_3ef727c3-7d46-48a1-a7b2-945e6c9146ac`
- Site POSTs `{ email }` to `https://product-power-up.web.app/subscribeNewsletter`
- API key stored as Firebase secret `BEEHIIV_API_KEY` (never in this repo)

## App Store
- Listing: https://apps.apple.com/us/app/pocket-pm-coach/id6767074466
- Privacy Policy URL → submitted in App Store Connect
- Support URL → submitted in App Store Connect

## Brand
- App name: Pocket PM Coach / Product Power-Up
- Design system: Mario-inspired, gamified
- Social: @shipwithandrew on X, Threads, Instagram
- Target user: Working PMs (L3–L7) prepping for interviews

## What's Done
- [x] GitHub account created
- [x] Repo created and Pages enabled
- [x] index.html designed and live
- [x] App Store badge CTAs + newsletter via Firebase proxy
- [x] privacy.html live
- [x] terms.html live
- [x] support.html live
- [x] Domain pointed at GitHub Pages
- [x] Dedicated public leaderboard page (real-player copy, top 100)

## Session Handoff
<!-- Update this section at the end of each session -->
Last completed: Pushed legal and leaderboard copy for default-on daily/public boards, independent opt-outs, private-by-default answers/AI feedback, and 18+ eligibility
Next up: Complete App Store age-rating/privacy checklist against these live URLs; rotate Beehiiv API key
