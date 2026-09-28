# Hi, I'm Costin

**Full-stack developer · M.Sc. Software Engineering student at Babeș-Bolyai University, Cluj-Napoca**

I build and run real products end to end, from a live payments platform to mobile apps, LLM agents and desktop tools. I care most about correctness: payments that never double-charge, data that stays where it should, and tests in CI that catch it when something breaks.

- Founder and sole developer of **[Host4R](https://host4r.ro)**, a live events marketplace that has processed **10,000+ RON** in real payments
- Hands-on with LLMs: a tool-calling agent that runs unattended on a Raspberry Pi, a real-time voice coach, and an on-device model I evaluated and deliberately retired when it wasn't reliable enough
- Based in Cluj-Napoca, Romania · **Open to remote** · Romanian (native), English (C1–C2)

[joldescosti@yahoo.com](mailto:joldescosti@yahoo.com) · [LinkedIn](https://www.linkedin.com/in/costincj/) · [host4r.ro](https://host4r.ro)

---

## Tech I work with

**Languages:** TypeScript, JavaScript, Python, SQL, Dart, C#, C++, PHP  
**Frontend & mobile:** React, Next.js (App Router), Tailwind CSS, Zustand, React Native (Expo), Flutter, Riverpod  
**Backend & data:** Node.js, Express, REST, WebSockets, PostgreSQL, Prisma, Redis, Firebase / Firestore, Supabase, Stripe, NextAuth / JWT  
**AI & LLMs:** tool-calling agents, prompt and context engineering, grounding and evaluation, OpenAI Realtime API, Groq / Llama, Whisper, llama.cpp  
**Testing & ops:** Vitest, Jest, Playwright, pytest, GitHub Actions, Docker, Sentry, Vercel, AWS, Cloudflare R2, Linux / systemd

---

## Featured projects

### [Host4R](https://host4r.ro): Founder & Full-Stack Developer · *live in production*
An invite-only events marketplace with separate user, host and admin roles, built and launched solo. **10,000+ RON processed** through Stripe Checkout, subscriptions and Connect payouts.
- **Reliability:** idempotent Stripe webhooks (retries never double-process), a transactional email outbox with dead-lettering, serializable-transaction retries, and Redis-based cron locks after finding that Postgres advisory locks silently fail behind Supabase's connection pooler
- **Quality:** 50+ Vitest test files, Playwright end-to-end suites per role, GitHub Actions CI with a coverage gate, Sentry, 38 Prisma migrations, a production runbook and GDPR documentation (DPIA, RoPA, breach response)

`Next.js 16` `React 19` `TypeScript` `PostgreSQL` `Prisma` `Stripe` `Redis` `NextAuth` `Vercel` `Sentry`

*The source is private because it's a live commercial product. I'm happy to walk through it in an interview.*

### [Lache: AI Companion](https://github.com/CostinCJ/pi-ai)
A self-hosted, proactive LLM agent on Telegram running on a Raspberry Pi 5. It uses tool calling (web search, reminders), keeps persistent SQLite memory with time-decaying facts, and runs an autonomy loop that starts conversations from context triggers (schedule, music, weather, presence), with quiet hours and engagement-aware back-off. Responses are validated with a single corrective retry, and it runs unattended as systemd services with encrypted backups, alerting and a hardened server.

`Python` `Groq (Llama 3.3 70B / Llama 4 Scout)` `Whisper` `SQLite` `pytest` `systemd` `GitHub Actions`

### [CampConnect](https://github.com/CostinCJ/CampConnect)
A multi-organisation summer-camp app (Romanian / Hungarian / English) **used at real camps**: announcements, schedules, points leaderboards, a camp map and emergency alerts. Tenant isolation is enforced server-side through custom claims set by Cloud Functions, never trusted from the client, and the Firestore rules have their own test suite. I also built an on-device LLM assistant (Qwen2.5-0.5B via llama.cpp) with an evaluation harness for recall, out-of-scope and hallucination cases, then retired it after evaluation for child-safety and build-reliability reasons.

`Flutter` `Dart` `Riverpod` `Firebase` `Cloud Functions` `Firestore rules tests` `Crashlytics`

### [Ciuri](https://github.com/CostinCJ/Ciuri) · [play it](https://ciuri.vercel.app)
A real-time, four-player online card game with a Hungarian deck, featuring two-stage bidding, turn timers, chat and computer players. The server is authoritative: a pure, unit-tested TypeScript game engine validates every move, and Postgres row-level security means each player can only ever read their **own** hand.

`Next.js 16` `TypeScript` `Supabase (Postgres, Realtime, RLS)` `Zod` `Vitest` `Playwright`

### [Apex Live](https://github.com/CostinCJ/Apex-Live)
An AI voice fitness coach for iOS and Android built on the OpenAI Realtime API, reached through a key-protecting server proxy. It uses JWT-authenticated WebSockets with heartbeat and exponential-backoff reconnection, an offline sync queue, HealthKit / Health Connect data and crash-safe workout state.

`React Native (Expo)` `TypeScript` `Express` `PostgreSQL` `Prisma` `WebSockets` `Jest` `GitHub Actions`

### [Diploma Maker](https://github.com/CostinCJ/diploma-maker)
An offline Electron app that reads names from a photo of a printed list with on-device OCR and prints one camp diploma per person. It handles children's names, so there's no network access by design and the data never leaves the machine. It ships as a Windows installer with in-app updates.

`Electron` `JavaScript` `Tesseract.js` `Vitest` `electron-builder`

### More
- **[TunesLayer](https://github.com/CostinCJ/TunesLayer):** an anti-cheat-safe music overlay for Windows games, with global hotkeys, Discord presence and an OBS widget · `C#` `.NET 8` `WPF`
- **[StringTracker](https://github.com/CostinCJ/StringTracker):** a guitar inventory app with auth, filtering and price analytics, Dockerized and deployed to AWS ECS · `Next.js` `TypeORM` `PostgreSQL` `Docker` `AWS`

---

## Experience & education

- **Founder & Full-Stack Developer**, Host4R · *Oct 2025 – present*
- **Analyst (part-time)**, Fiind Yourself S.R.L. · *Jan 2026 – present*
- **M.Sc. Software Engineering**, Babeș-Bolyai University · *2026 – 2028, in progress*
- **B.Sc. Computer Science**, Babeș-Bolyai University · *2023 – 2026*

## Outside of code

I spent last summer as a camp guide in the Apuseni Mountains, which is where CampConnect and Diploma Maker come from: both are tools for work I actually did. I've played guitar and bass for four years and record at home in Ableton Live.
