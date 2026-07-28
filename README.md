# Hi, I'm Costin

**Full-stack developer, CS graduate (Babeș-Bolyai University, Cluj-Napoca)**

I build and ship real products end to end: from a live, paid events platform to mobile apps, web tools, and the occasional game. I care about clean architecture, practical UX, and things people actually use.

- Founder and developer of **[Host4R](https://host4r.ro)**, a live events platform that has processed **10,000+ RON** in real payments
- Based in Cluj-Napoca, Romania. Open to remote
- [joldescosti@yahoo.com](mailto:joldescosti@yahoo.com) | [LinkedIn](https://www.linkedin.com/in/costincj/)

---

## Tech I work with

**Web:** TypeScript, Next.js, React, Tailwind CSS, Node.js
**Desktop:** Electron
**Mobile:** Flutter, Dart, Firebase
**Backend & Data:** PostgreSQL, Prisma, Stripe, NextAuth, REST APIs
**Languages:** Python, C++, C#, JavaScript
**Tools:** Git, Cloudflare R2

---

## Featured projects

### [Host4R](https://host4r.ro), Founder & Full-Stack Developer
An invite-only, full-stack events platform connecting verified hosts with a curated guest community. **Live in production with real users and 10,000+ RON processed.** Subscription tiers, host payouts, application vetting, reviews, and a referral system, all built and shipped solo.
`Next.js 16` `React 19` `TypeScript` `Tailwind` `PostgreSQL` `Prisma` `NextAuth` `Stripe` `Cloudflare R2`

### [CampConnect](https://github.com/CostinCJ/CampConnect)
A multi-organiser summer-camp app for guides and kids, bilingual in Romanian and Hungarian plus English. Guides register an organisation, create camp sessions, manage teams, post announcements and schedules, run a points leaderboard and send emergency alerts; kids join with a `CAMP-XXXX` code over anonymous sign-in and keep an on-device journal. Roles and camp membership are assigned server-side by Cloud Functions rather than trusted from the client, and the org-scoped Firestore rules have their own test suite.
`Flutter` `Dart` `Riverpod` `go_router` `Firebase Auth` `Firestore` `Cloud Functions` `FCM`

### [Lache (pi-ai)](https://github.com/CostinCJ/pi-ai)
A self-hosted, proactive AI companion that runs on a Raspberry Pi 5 and talks over Telegram. It keeps persistent memory in SQLite, durable facts with time decay, full history, rolling weekly profiles, and an autonomy loop that starts conversations on its own from schedule, music, weather and presence triggers, with quiet hours and engagement-aware back-off so it never turns spammy. Built test-first with 40+ test modules and a CI pipeline, and deployed as four systemd services on the Pi.
`Python` `SQLite` `Telegram Bot API` `Groq (Llama 3.3 / Llama 4)` `Whisper` `systemd` `pytest`

### [Diploma Maker](https://github.com/CostinCJ/diploma-maker)
An offline desktop app that reads participant names from a photo of a printed list and prints one camp diploma per person, replacing an evening of hand-writing them. It handles children's names, so privacy is a functional requirement, not a feature: the Romanian OCR model ships inside the installer, no HTTP code exists anywhere in the app, and it runs correctly with networking disabled. Five ways to get the list in (photo OCR, paste, `.docx`/`.xlsx`/`.csv`, typing, by hand), editable templates with live preview, and atomic saves so a crash can't truncate the list.
`Electron` `JavaScript` `Tesseract.js` `Vitest` `electron-builder`

### [TunesLayer](https://github.com/CostinCJ/TunesLayer)
An anti-cheat-safe music overlay for Windows that controls Spotify, Apple Music, YouTube Music and anything else reporting to Windows Media Session: no login, no DLL injection, no game hooks. Global hotkeys keep working inside exclusive-fullscreen games, next to five themes, Discord presence and a now-playing widget for OBS. It stays under 50 MB of RAM and about 0.1% CPU, and excludes itself from screen capture so it never shows up in a recording.
`C#` `.NET 8` `Windows Media Session (SMTC)`

### [StringTracker](https://github.com/CostinCJ/StringTracker)
A guitar inventory app for players and small shops, with full CRUD over the collection and filtering by manufacturer, type, condition, string count and price. A price analytics view surfaces statistics and category highlights across the whole inventory, so it answers what the collection is worth and not just what is in it.
`Next.js` `React` `TypeScript` `Node.js`

---

## A bit about me

I enjoy the full journey from idea to shipped product. I spend my summers as a camp guide, which is where CampConnect and Diploma Maker come from; both are tools for work I actually do. Outside of code I record guitar music and edit video, which is probably why I keep building things related to it.

Reach me at **[joldescosti@yahoo.com](mailto:joldescosti@yahoo.com)**
