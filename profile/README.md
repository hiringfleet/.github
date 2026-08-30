# HiringFleet

**The career platform for international students in the US.**

More than a million F-1 students study in the US, and most graduate into the same wall: a 90-day OPT unemployment clock, a job market where the majority of employers don't sponsor visas, and no reliable way to tell which ones do.

HiringFleet turns that search into something you can manage. It tracks your full F-1 timeline, from CPT limits through the OPT clock to the H-1B lottery, and points your applications at employers with a real record of sponsoring.

**[hiringfleet.com](https://hiringfleet.com)** — free to start, no credit card required.

### What's in the platform

- **Sponsor database** — verified H-1B sponsors from public DOL and USCIS filings, so you can check a company before spending an application on it.
- **F-1 timeline tracker** — CPT limits, the 90-day OPT unemployment count, and STEM OPT extension deadlines on one dashboard with a live countdown.
- **Resume optimization** — AI rewrites that translate international experience into US-standard titles and measurable bullet points, scored against ATS parsing.
- **Cold outreach** — find the hiring manager, draft an email that mentions OPT eligibility without apologizing for it, then track replies and follow-ups.
- **Application pipeline** — Kanban-style tracking from first save to signed offer, tied to your visa deadlines.

### How it's built

TypeScript end to end. Next.js (App Router) on Vercel, Postgres on Neon through Prisma, Auth.js v5 with TOTP two-factor, Cloudflare R2 for file storage, and Gemini behind the AI features. Background jobs run on n8n and QStash, and every change ships through Playwright end-to-end suites on our own CI runner.

Most of our repositories are private while we build. If you're an international student and want to try the platform, start at [hiringfleet.com](https://hiringfleet.com).
