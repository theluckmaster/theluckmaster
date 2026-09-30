### Hi, I'm Hampton

I build small SaaS products, browser extensions, and Python data systems. I care about getting the unglamorous parts right: server-side enforcement, idempotent billing, input validation, and tests that check what code must *not* do.

---

#### Typist · [trytypist.com](https://trytypist.com) · [case study](https://github.com/theluckmaster/typist-case-study)
A Chrome side panel (Manifest V3) that types prepared text into the field you choose at a set WPM.
- Typing engine handles plain inputs, React-controlled inputs, `contenteditable`, same-origin iframes, and Google Docs' hidden input iframe
- Cloudflare Workers + D1 backend: Google sign-in, server-enforced usage limits with idempotent reservations, Stripe billing with verified, de-duplicated webhooks
- Automated `node:test` suites for both the typing engine (run against a DOM harness) and the API

#### IsThisAScam · [isthisascam.fyi](https://isthisascam.fyi) · [case study](https://github.com/theluckmaster/isthisascam-case-study)
Paste a suspicious message and get a plain-language verdict, red flags, and next steps.
- Next.js 16 / TypeScript on Vercel; Gemini with a strict JSON response schema
- Per-IP rate limiting on Upstash Redis that fails closed; no server-side URL fetching; messages not stored
- Programmatic SEO: generated sitemap, JSON-LD (FAQPage kept in sync with the visible FAQ), 10 guide pages

#### Polymarket data research · [repo](https://github.com/theluckmaster/polymarket-data-research)
Python toolkit for short-horizon prediction-market research. It contains no trading code.
- Async WebSocket ingestion with backoff, stale-feed detection, and JSONL recording
- Ring-buffer features and a window backtester that makes look-ahead structurally impossible
- Tested against a random-walk null (must find no edge) and a planted-trend positive control (must find one)

---

300+ automated tests across current projects (`node:test`, `pytest`).

**Stack:** TypeScript/JavaScript · Python · Next.js · Chrome Extensions (MV3) · Cloudflare Workers/D1 · Vercel · Stripe · Redis · numpy · pytest / node:test

**Currently learning / building**
- Evaluating AI-generated code with tests plus written rubrics
- Agent-based simulation (a Kaggle simulation competition)
- CI for my existing projects (GitHub Actions)
