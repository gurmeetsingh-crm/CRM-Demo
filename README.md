# BrightDesk — Interactive HubSpot Demos

Client-facing portfolio demos built around one fictional B2B software company (BrightDesk).
Attach them to a proposal and prospects can *see* the finished product before they hire you.

**Each demo is one self-contained file. No dependencies, no build step, no server.**
Double-click it, email it, or host it anywhere. The two demos cross-link via the button
in the top control bar.

| File | Demo |
|---|---|
| `index.html` | **Full HubSpot portal build** — CRM, pipeline, automation map, lead scoring, reports, audit mode |
| `ai-speed-to-lead.html` | **AI Speed-to-Lead / AI SDR** — watch an AI answer, qualify and book an inbound lead in seconds, with human-approval mode and guardrails |

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
