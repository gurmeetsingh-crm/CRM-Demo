# Gurmeet Singh — GoHighLevel Demo Suite

Client-facing portfolio demos you attach to a proposal so prospects can *see* the finished
system before they hire you. The **site homepage is the GoHighLevel hub**; the HubSpot demos
(a second Upwork profile) live under `/hubspot/`.

**Each demo is one self-contained file. No dependencies, no build step, no server.**
Every GHL demo cross-links back to the hub, and appending `?for=Their Business` to any link
personalizes it for a prospect (see `UPWORK-KIT.md`).

## Site layout (also the GitHub Pages URL paths)

| File | Serves at | Demo |
|---|---|---|
| `index.html` | `/` | **GHL Demo hub** — animated landing page with a live systems console; personalizes via `?for=` |
| `ai-employee.html` | `/ai-employee.html` | **AI Employee** — missed-call text-back at a med spa: books a slot, takes a deposit, routes medical questions to humans |
| `dental-snapshot.html` | `/dental-snapshot.html` | **Dental snapshot** — interactive $99 funnel, patient-journey map, 8 automations, pipeline & templates |
| `reputation.html` | `/reputation.html` | **Reputation & review engine** — live dashboard, happy/unhappy routing, before/after Map-Pack climb; Google-compliant (no gating) |
| `UPWORK-KIT.md` | — | **Sales kit** — profile copy, portfolio blurbs, proposal templates, Loom scripts, personalized-link guide |
| `hubspot/index.html` | `/hubspot/` | HubSpot **Full portal build** — CRM, pipeline, automation map, lead scoring, reports, audit mode |
| `hubspot/ai-speed-to-lead.html` | `/hubspot/ai-speed-to-lead.html` | HubSpot **AI Speed-to-Lead / AI SDR** |

**GoHighLevel is the primary focus.** The GHL hub (`index.html`) has a `CONFIG` object at the
bottom of the file — paste your existing client-app demo URL and your real booking link there.

## Hosting on GitHub Pages (already enabled)

Pages serves this repo from the branch root, so the homepage is the GHL hub. Current URLs
(replace `Claude` with the repo name if you rename it):

- **GHL hub (share this):** `https://gurmeetsingh-crm.github.io/Claude/`
- AI Employee: `https://gurmeetsingh-crm.github.io/Claude/ai-employee.html`
- Dental snapshot: `https://gurmeetsingh-crm.github.io/Claude/dental-snapshot.html`
- Reputation engine: `https://gurmeetsingh-crm.github.io/Claude/reputation.html`
- HubSpot portal: `https://gurmeetsingh-crm.github.io/Claude/hubspot/`

A `.nojekyll` file is included so Pages serves the files exactly as-is. To get a cleaner URL,
rename the repo (Settings → General) from `Claude` to e.g. `ghl-demos`; GitHub auto-redirects
the old links. Once the hub URL is final, paste it into `UPWORK-KIT.md` wherever it says `[HUB]`.
