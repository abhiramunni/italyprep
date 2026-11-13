# ItalyPrep — Study in Italy Planner

A single-file web app that plans a master's degree in Italy, step by step — built for Indian students aiming at the September 2027 intake.

**Live:** https://abhiramunni.github.io/italyprep/

## What it does

- **Journey map** — 8 stations from November 2026 to September 2027 (shortlist → documents → IELTS → applications → MAECI window → offers/DSU → pre-enrolment & visa → fly). Tap a station's circle when it's done; the readiness score follows.
- **Scholarships worth chasing** — MAECI government grant (€10,800 / 9 months), Invest Your Talent (€1,200/month + internship), DSU regional scholarships, and university merit awards, with real amounts, statuses and official portal links. Tap **Track** to watch a call.
- **University shortlist** — 6 English-taught CS/web master's (Politecnico di Milano, Politecnico di Torino, Sapienza, Bologna, Padua, Milan) with indicative fees and city notes. Star favourites, add your own.
- **First-year cost ledger** — pick a city, set tuition, slide monthly living costs, choose a scholarship offset. Totals in euros and rupees with a donut breakdown, plus the visa proof-of-funds note (≈ €6,000).
- **Documents checklist** — 11 items across identity, academics, language & money, and visa, with a progress bar.
- **IELTS practice log** — log mock-test bands (Listening/Reading/Writing/Speaking), average vs your target (6.0–7.5).
- **Plain-language guides** — MAECI, ISEE Parificato, combining scholarships, the study visa, money to carry, and learning Italian.
- **Extras** — cinematic intro (tap-to-skip, quick on return visits), 3-step coach tour, copy-my-plan summary, erase-all, next-step bottom bar.

## Facts & sources

Amounts and dates come from the published 2026/27 calls (checked 13 Nov 2026):

- **MAECI 2026/27**: €10,800 total for 9 months (1 Nov 2026 – 31 Jul 2027); applications closed 26 Mar 2026, 14:00 CET; India on the eligible-countries list; master's age limit 28. Next call expected ~March 2027 (pattern from past calls, **not** a confirmed date).
- **Invest Your Talent 2026/27**: €1,200/month stipend + compulsory 3–4 month company internship; deadline 11 May 2026; India eligible.
- **DSU regional**: apply Aug–Sep, needs an ISEE Parificato from a CAF office; cannot be combined with MAECI.
- Tuition and living-cost figures are indicative ranges — every university's official fees page is the final source. Always verify on the official portals before applying.

## Tech

- One self-contained `index.html` — no backend, no signup, no build step.
- State lives only in `localStorage` (`italyprep.v1`). Nothing is uploaded anywhere.
- Fraunces + Inter, warm editorial palette (ivory paper, espresso ink, bronze/amber/terracotta), Ken Burns photography, inline SVG icons only, no emoji.
- QA: 56/56 headless jsdom functional assertions, `node --check` clean, zero uncaught JS errors.

## Run locally

Open `index.html` in any browser. To re-run the tests: `npm install jsdom && node qa-test.js`.
