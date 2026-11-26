# Craby.AI landing page

Single-file landing page for Craby.AI. Open `index.html` in a browser. There's no build step. Fonts load from Google Fonts.

```
index.html              page, styles and scripts (self-contained)
assets/craby-mark.svg   Craby mascot / logomark, standalone
```

## Design system

- **Palette, "ocean depth":** the page gets darker as you scroll, like diving.

  | Role | Colour |
  |---|---|
  | Sky (hero) | `#BDE2F1` |
  | Sea-foam (page) | `#F2F8FB` |
  | Navy (ink, bands) | `#171E52` |
  | Deep navy (CTA, footer) | `#0E1340` |
  | Crab orange (mascot, CTA, data) | `#F2713A` |
  | Peach (tints) | `#FF9B6E` |

  - Buttons use navy text on orange, at 5.4:1 contrast. White on that orange only reaches 2.9:1, which fails.
  - Orange used as text on white is `#C94E1C`, at 4.6:1.
- **Type:** Instrument Sans for headlines and body, Geist Mono for labels and code.
- **Radius:** 2px everywhere. Fully rounded only for the nav pill, badges and chips.
- **Nav (morphing bar):**
  - At the top it's a full-width bar.
  - After 80px of scroll it becomes a frosted pill, hides when you scroll down and comes back when you scroll up.
  - It turns navy over dark sections, marks the active section with an orange dot, and has a Product mega-menu that works with hover, click and keyboard.
- **Crab motion:** every part of the `#craby` symbol is grouped (`claw-l/r`, `legs-l/r`, `shell`), so inline copies (`svg.crab-live`) can animate.
  - **Privacy snip:** a claw pinches each sensitive word into its `[TOKEN]`. It runs in the hero card and in the Privacy section.
  - **Scroll progress:** Craby walks along the line under the nav pill.
  - **Logo:** the claws pinch on hover.
  - **Hero:** sea lines drift and bubbles rise behind it. Bubbles also rise in the final CTA.
  - **Halftone crab:** ripples like water.
  - **Primary buttons:** let out bubbles on hover.
  - **Footer:** the giant "Craby.AI" wordmark in crab orange sits on the bottom edge of the page, with bubbles rising behind it.
- **Brand pillars, taken from crab biology:**
  - **Shell = Privacy Protect.** Every prompt gets a shell.
  - **Molt = continuous fine-tuning.** Each nightly version is a molt, kept only if it's stronger.
  - **Claws = ownership.** You choose the data, roll back any molt and export your weights.

  Use the pillars in headlines, eyebrows and microcopy. Keep the literal feature names for clarity.
- **CTA vocabulary:** "Start free" as the primary and "Book a demo" as the secondary.
- **Nav stays visible:** the bar morphs into a pill after 80px and never auto-hides.
- **Colour blends:** the navy band and the final CTA fade in and out of the sea-foam over roughly 190px, so there are no hard lines between light and dark sections.
  - **Reduced motion:** every animation stops and the page shows static states.

## Before launch: replace every placeholder

Search the file for `PLACEHOLDER` and `PROOF NEEDED`. None of these numbers are real yet.

- [ ] **Hero live stat + bottom ticker** (`TICKER`): connect them to real usage or delete them.
- [ ] **Accuracy chart** (`FT`), **comparison tabs** (`BARS`) and **model card** latencies.
- [ ] **Picker** (`PICKS`) and **calculator pricing** (`PRICING`).
- [ ] **Receipts wall**: commented out until you have named design-partner quotes.
- [ ] **Compliance pills**: only list what you actually hold.
- [ ] **Product claims to confirm**:
  - live in under 5 minutes
  - weight export
  - values restored after masking
  - OpenAI-compatible endpoint
  - credit from $10
  - unlimited chat seats
  - uptime SLA
- [ ] **Domain** `api.craby.ai`, every `href="#"`, and the sign-up form (front-end demo only).
