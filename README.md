# Craby.AI landing page

Single-file, coming-soon landing page for Craby.AI. Open `index.html` in a browser. There's no build step. Fonts load from Google Fonts.

```
index.html              page, styles and scripts (self-contained)
assets/craby-mark.svg   Craby mascot / logomark, standalone
```

## Page structure

Nine blocks, about 8,200px on desktop. Every section gets one headline, one visual and one idea.

| # | Block | What it does |
|---|---|---|
| 1 | Nav | Logo, five anchors, "Request access". A full bar at the top, then a frosted pill after 80px. It never hides, turns navy over dark sections, and marks the active section with an orange dot. |
| 2 | Hero | "Coming soon" badge, "Most AI is rented. This one's yours.", the early-access email form, a reassurance row, the console tagged **Product preview**, and a 4-step strip (Register, Add credit, Deploy, Build and roll out). |
| 3 | 01 · Shell | Privacy Protect. The 3-stage masking flow. The claw snips each sensitive value once, on scroll. |
| 4 | 02 · Molt | Continuous fine-tuning. Accuracy step chart (legend, tooltip, arrow keys, table view) and the "Next molt" data bar. |
| 5 | 03 · Claws | Deploy and own. OpenAI-compatible code and team chat, regions US · EU · GCC · Asia, serverless by default, dedicated GPUs on Enterprise, weight export. |
| 6 | 04 · The math | Cost calculator, clearly labelled as illustrative pricing. |
| 7 | 05 · Enterprise | Navy band: "Open weights. Closed doors.", halftone crab, 8 controls, compliance pills. |
| 8 | 06 · FAQ | Six questions, including access timing and launch models. |
| 9 | Final CTA + footer | Second early-access form, footer links, dotted "Craby.AI" wordmark. |

## Design system

- **Palette, "ocean depth":** sky at the top, sea-foam through the story, deep navy at the bottom.

  | Role | Colour |
  |---|---|
  | Sky (hero) | `#BDE2F1` |
  | Sea-foam (page) | `#F2F8FB` |
  | Navy (ink, band) | `#171E52` |
  | Deep navy (CTA, footer) | `#0E1340` |
  | Crab orange (mascot, CTA, data) | `#F2713A` |
  | Peach (tints) | `#FF9B6E` |

  - Buttons use navy text on orange, at 5.4:1 contrast. White on that orange only reaches 2.9:1, which fails.
  - Orange used as text on white is `#C94E1C`, at 4.6:1.
  - **Accent budget:** orange appears only on the primary CTA, chart highlights, the mascot and the footer wordmark.
- **Type:** Instrument Sans for headlines and body, Geist Mono for section labels ("01 · SHELL"), data and code.
- **Radius:** 2px everywhere. Fully rounded only for the nav pill, its button and the hero badge.
- **Depth:** hairline borders first, one light shadow on cards. Story sections sit open on the canvas; only the calculator is a panel.
- **Brand pillars, from crab biology:**
  - **Shell = Privacy Protect.** Every prompt gets a shell.
  - **Molt = continuous fine-tuning.** A molt runs once enough approved data has built up, and ships only if it beats the current version.
  - **Claws = ownership.** You choose the data, roll back any molt and export your weights.
- **Signature crab moments (only these four):**
  1. Logo claws pinch on hover.
  2. The claw snips private data into `[TOKENS]` in the Shell section, once.
  3. The halftone crab builds in, once, in the Enterprise band.
  4. The footer wordmark is drawn in halftone dots, peach to orange.
- **Reduced motion:** every animation stops and the page shows static, fully revealed states.
- **CTA vocabulary:** "Request early access" (primary) and "Talk to the founders" (secondary link).

## Before launch: replace every placeholder

Search the file for `PLACEHOLDER`. None of these numbers are real yet.

- [ ] **Launch date** and the early-access copy ("opens in waves").
- [ ] **The 2 launch models:** name them in the FAQ and, if you want, in the console mock.
- [ ] **Molt threshold:** "1,840 of 2,500 approved examples" in the Molt section.
- [ ] **Accuracy chart data** (`FT`) and the console mock numbers.
- [ ] **Calculator rates** (`PRICING`).
- [ ] **Compliance pills:** only list what you actually hold.
- [ ] **"Talk to the founders" link** (every `href="#"`), plus About, Careers and the legal pages.
- [ ] **Early-access form:** front-end demo only. Wire both forms to your waitlist (for example a form endpoint or your CRM).
- [ ] **Domain** `api.craby.ai` in the code sample.
