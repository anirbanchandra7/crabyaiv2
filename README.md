# Craby AI landing page

Single-file landing page for Craby AI. Open `index.html` in a browser. There's no build step. Fonts load from Google Fonts.

```
index.html              page, styles and scripts (self-contained)
assets/craby-mark.svg   Craby mascot / logomark, standalone
```

## Design system

- **Art direction:** warm brand. Sand canvas `#F8F5F0`, deep-sea ink `#0E1A2B`, crab coral accent `#CF4426`.
- **Type:** Frank Ruhl Libre for display (weight 400, -0.032em tracking) and Roboto Flex for UI, the Origami pairing from the design skill. Geist Mono only for small eyebrows, tickers and code.
- **Layout rhythm:** left hero › left sticky steps › text left / chart right › visual left / text right › centred API + chat › split chips › left dark band › centred calculator › split header + 3-up › centred pricing › split FAQ › split CTA card.
- **Radius family:** soft, 6 / 10 / 16 / 24px for surfaces, pill for buttons and inputs.
- **Mascot:** a geometric Craby built on a 64px grid with one coral colour and a 3px stroke, so it still reads at 24px. It's used as the logo, the app icon, the chat avatar, and a halftone version in the "Why now" band.
- **Charts:** hand-built SVG. They use hairline solid gridlines and 2px lines, carry direct end labels plus a legend, and give the highlighted series the accent colour with context series in grey. They have a crosshair tooltip, arrow-key navigation and a table view.

## Section order

Announcement › Nav › Hero (email capture + console mock + live ticker) › Model strip › How it works (sticky 4 steps: register, add credit, deploy, build) › Continuous fine-tuning (chart) › Privacy Protect › API + team chat › Capability chips › "Open weights. Closed doors." band › Cost calculator › Use cases › Pricing › FAQ › Final CTA › Footer

## Before launch: replace every placeholder

Search the file for `PLACEHOLDER`. None of these numbers are real yet.

- [ ] **Live ticker** (`TICKER` in the script): connect it to real usage, or delete the block. Invented traction on a site YC reviewers will open is a credibility risk.
- [ ] **Announcement bar**: the $25 beta credit.
- [ ] **Fine-tuning chart** (`FT`): it's labelled "Illustrative". Swap in a real eval run as soon as you have one.
- [ ] **Calculator pricing** (`PRICING`): closed API $5/1M, $30 per seat, Craby $1.50/1M, 0.8M tokens per chat user.
- [ ] **Compliance pills**: only list what you actually hold.
- [ ] **Product claims to confirm**: live in under 5 minutes, weight export, values restored after masking, OpenAI-compatible endpoint, credit from $10, unlimited chat seats, uptime SLA, new models within days.
- [ ] **Domain** `api.craby.ai` in the code samples.
- [ ] **Links**: every `href="#"` (Docs, Sign in, Book a demo, footer).
- [ ] **Sign-up form**: it's a front-end demo only. Connect it to your auth or waitlist.
