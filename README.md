<h1 align="center">Logan Pinel</h1>

<p align="center">
  <strong>Full-Stack Software Engineer</strong> · Computer Science @ University of Tampa
</p>

<p align="center">
  <a href="mailto:loganpinel@outlook.com"><img src="https://img.shields.io/badge/Email-loganpinel%40outlook.com-0A66C2?style=for-the-badge&logo=microsoftoutlook&logoColor=white" alt="Email" /></a>
  <a href="https://www.linkedin.com/in/logan-pinel-2609ab291/"><img src="https://img.shields.io/badge/LinkedIn-Logan%20Pinel-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn" /></a>
  <a href="https://cremedium.com"><img src="https://img.shields.io/badge/Live-cremedium.com-FF6A00?style=for-the-badge&logo=vercel&logoColor=white" alt="CREM" /></a>
</p>

---

I build production software end to end: data model, API, auth, UI, and deployment. I designed and built **CREM**, a commercial real estate marketplace now live in production, **on my own**. I'm looking for **software engineering internships** where I can ship real features alongside a strong team.

## Featured project: CREM, a commercial real estate marketplace

**[cremedium.com](https://cremedium.com)** · Next.js 16 · TypeScript · PostgreSQL · Prisma · Supabase · Python/FastAPI · Vercel · Render

A marketplace where licensed brokers list commercial properties (multifamily, retail, office, industrial, and more) and buyers find, analyze, and sign NDAs to access deal documents. I built both codebases myself, a Next.js web app and a Python service, and took them from an empty repo to production. I used **Claude Code** as an AI pair programmer throughout. I direct the architecture, review every change, and record design decisions in ADRs, while the agent speeds up implementation, debugging, and code review. That is the AI-assisted workflow the industry is moving toward.

**Highlights**

- **AI listing extraction.** Brokers upload an Offering Memorandum PDF. A FastAPI service reads it with the Gemini API and pre-fills about 40 listing fields for review. Uploads go straight to storage through pre-signed URLs, which keeps them under serverless body limits.
- **Automated public-records verification.** Before a listing goes live, a headless-browser service (Playwright + Chromium) reads the county appraiser's website and uses an LLM to extract parcel ownership, assessed value, and sales history. The results are matched against the listing's address. Counties that can't be scraped fall back to a bulk-data CLI I wrote that streams multi-GB county files.
- **Legally auditable NDA gating.** Confidential documents unlock only after a click-wrap NDA is signed. Each signature records the exact agreement version by SHA-256 hash and produces a PDF Acceptance Certificate. The feature also supports broker countersignature, per-buyer redline negotiation, and separate agreements for principals and brokers.
- **Analytics and lead reporting.** Brokers see per-listing Views, Leads, and CA Signed funnel metrics that exclude insider and bot traffic. Brokerage-wide reports export to Excel.
- **AI assistant integration.** A Model Context Protocol (MCP) server lets users search listings and pull market statistics from Claude or ChatGPT.
- **Production hardening.** Role-based access control, CSP and security headers, CSRF protection, rate limiting, row-level security, Sentry monitoring, versioned database migrations, and written architecture decision records (30+ ADRs).

## Tech stack

**Languages**
<p>
  <img src="https://skillicons.dev/icons?i=ts,js,python,html,css" alt="Languages" />
</p>

**Frameworks & Libraries**
<p>
  <img src="https://skillicons.dev/icons?i=nextjs,react,nodejs,tailwind,fastapi,flask" alt="Frameworks and libraries" />
</p>

**Databases, Cloud & Developer Tools**
<p>
  <img src="https://skillicons.dev/icons?i=postgres,prisma,supabase,vercel,docker,git" alt="Databases, cloud and developer tools" />
</p>

## Hackathons

| Event | Project | |
|---|---|---|
| **[HackJam 2025](https://hackjam2025.devpost.com/)**, Nov 2025 | **UniCal**: an AI-powered calorie tracker for college students | Solo, 12 hours |
| **[Hackabull 2025](https://lu.ma/9e1x29r4?tk=MlpLlM)**, Apr 2025 | **ZomBeFit**: an AI fitness tracker that analyzes macro trends and gives personalized health recommendations | Team of 4, 24 hours |

## Education

**University of Tampa**, B.S. Computer Science
Relevant coursework: Advanced Data Structures & Algorithms · Operating Systems & Systems Programming · Software Design & Engineering · Computer Organization & Architecture · Web Development · Global Business

---

<p align="center"><em>Open to Summer 2027 software engineering internships. Let's talk.</em></p>
