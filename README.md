# Gurmeet Singh — GoHighLevel Demo Suite

Client-facing portfolio demos you attach to a proposal so prospects can *see* the finished
system before they hire you. The GoHighLevel demos are the focus; two HubSpot demos serve a
second Upwork profile.

**Each demo is one self-contained file. No dependencies, no build step, no server.**
Double-click it, email it, or host it anywhere. Every GHL demo cross-links back to the hub, and
appending `?for=Their Business` to any link personalizes it for a prospect (see `ghl/UPWORK-KIT.md`).

| File | Platform | Demo |
|---|---|---|
| `ghl/index.html` | **GoHighLevel** | **Demo hub** — animated landing page with a live systems console, linking every demo; per-prospect personalization via `?for=` |
| `ghl/ai-employee.html` | **GoHighLevel** | **AI Employee for local business** — missed-call text-back at a med spa: books a real calendar slot, takes a deposit by text-to-pay, routes medical questions to humans |
| `ghl/dental-snapshot.html` | **GoHighLevel** | **Dental practice snapshot** — a complete pre-built system: interactive $99 new-patient funnel, clickable patient-journey map, 8 plain-English automations, pipeline and message templates |
| `ghl/reputation.html` | **GoHighLevel** | **Reputation & review engine** — live review dashboard, interactive happy/unhappy routing, before/after with a Google Map-Pack climb; built Google-compliant (no gating) |
| `ghl/UPWORK-KIT.md` | — | **Sales kit** — profile copy, portfolio blurbs, proposal templates, Loom scripts, personalized-link guide |
| `index.html` | HubSpot | **Full portal build** — CRM, pipeline, automation map, lead scoring, reports, audit mode |
| `ai-speed-to-lead.html` | HubSpot | **AI Speed-to-Lead / AI SDR** — an AI answers, qualifies and books an inbound lead in seconds, with human-approval mode and guardrails |

**GoHighLevel is the primary focus** (that Upwork profile is the one being built up); the HubSpot demos serve the second profile. The GHL hub has a `CONFIG` object at the bottom of the file — paste your existing client-app demo URL and your real booking link there.

## Hosting on GitHub Pages

The demos are plain static files, so GitHub Pages hosts them for free:

1. Repo → **Settings → Pages** → Source: **Deploy from a branch** → pick this branch, folder **/ (root)** → Save.
2. After a minute your links are live:
   - **GHL hub** (the one to share): `https://<username>.github.io/<repo>/ghl/`
   - HubSpot portal: `https://<username>.github.io/<repo>/`
3. Renaming the repo (e.g. to `ghl-demos`) makes the URL prettier — GitHub auto-redirects the old one.

A `.nojekyll` file is included so Pages serves the files exactly as-is. Once the hub is live,
paste its URL into `ghl/UPWORK-KIT.md` wherever it says `[HUB]`.

## What's inside

| Screen | What it demonstrates |
|---|---|
| **Contacts** | Clean CRM data — owners, lifecycle stages and scores on every record |
| **Contact record** | HubSpot-style 360° record with activity timeline, plus **two custom CRM cards** (Stripe billing + product usage) that signal developer-level UI-extension work |
| **Deals** | Pipeline board where every stage has a ⚡ icon explaining, in plain English, what happens automatically at that stage |
| **Automation map** | Every workflow in the portal drawn as one clickable flowchart — capture → qualify → route → sell → post-sale |
| **Lead Scoring** | An animated replay of a lead's 11-day journey: points accumulate, the MQL threshold trips, sales gets notified |
| **Reports** | KPI row, lifecycle funnel, revenue by source, monthly trend and rep leaderboard — hoverable charts, each with a "view data" table |
| **Audit mode** | A toggle that flips the whole portal into its "unmaintained" state — duplicates, dead workflows, stalled deals — plus a graded audit report with a prioritized 30-day fix plan |
| **Guided tour** | A 13-step spotlight walkthrough that sells the whole build in ~2 minutes |

## What's inside `ai-speed-to-lead.html`

| Screen | What it demonstrates |
|---|---|
| **Live Console** | An inbound lead handled end-to-end in real time: enrichment, intent scoring, ICP fit, a personalized draft — each step with an expandable "Why?" showing the AI's reasoning. **Copilot mode** pauses for a human "Approve & send"; **Autopilot** sends in seconds |
| **Lead Queue** | Nine leads triaged by AI — booked, qualified, nurtured, binned as spam, or routed to a human (legal question). Click any row for the reasoning |
| **Results** | Before/after KPIs (42 min → 28 sec first response) and charts with a go-live annotation |
| **How It Works** | The HubSpot plumbing (workflow → webhook → AI agent → CRM writes) plus six plain-English guardrails — the objection killer |

## Re-branding it

Open `index.html` and edit the `BRAND` object near the top of the `<script>`:

```js
const BRAND = {
  consultant: "Your Name",
  title: "HubSpot Expert",
  clientName: "BrightDesk",
  ctaLine: "…"
};
```

Everything else (top bar, footer, audit report, CTA button) re-brands itself.

## Hosting on GitHub Pages

Repo → Settings → Pages → deploy from branch → root. The demo is a single static file,
so it works instantly. Send prospects the link with the note: *"Click 'Start guided tour'."*

---

*Fictional company and sample data. Independent portfolio demo replicating the HubSpot user
experience — not affiliated with or endorsed by HubSpot, Inc.*
