# BrightDesk — Interactive HubSpot Portal Demo

A fully clickable, pixel-faithful replica of a **completely built-out HubSpot portal** for a
fictional B2B software company (BrightDesk). Built as a client-facing portfolio piece: attach it
to a proposal and prospects can *see* the finished product before they hire you.

**Everything is one file — `index.html`. No dependencies, no build step, no server.**
Double-click it, email it, or host it anywhere.

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
