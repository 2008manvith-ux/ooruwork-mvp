# OoruWork

A mobile first hackathon MVP for Track 4 UnlockED, Problem Statement 3: Hyper-Local Job Matching for Informal & Semi-Skilled Workers.

> A worker shouldn’t need a resume to find work.

## Run locally

Requirements: Node.js 18.17+ and npm.

```bash
npm install
npm run dev
```

Open http://localhost:3000. For a production build, run `npm run build` then `npm start`.

## Demo walkthrough

1. Choose **Find work**, then add a worker profile with locality, skills, availability and daily pay preference.
2. Browse the sample listings. Open a job to review match factors or apply.
3. Choose **Hire workers**, post a role, then review applications and update status.
4. Visit `/faq` for common questions. Unknown routes show a custom 404 page.

## Matching rules

The deterministic match score uses skill fit (up to 45 points), exact locality (25), compatible availability (15), and meeting the worker's wage preference (15). Each factor is shown. A score helps sort opportunities, not guarantee employment.

## Data and scope

Profiles, listings and applications use browser `localStorage` on this device only. They do not sync across browsers. Five seeded listings are labeled sample data and are not real or verified offers. There is no authentication, backend, GPS, maps, voice AI, or blocked access page in this MVP.