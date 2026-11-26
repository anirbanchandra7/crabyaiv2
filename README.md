# Craby.AI landing page

Single-file landing page for Craby.AI. Open `index.html` in a browser. There's no build step. Fonts load from Google Fonts.

```
index.html              page, styles and scripts (self-contained)
assets/craby-mark.svg   Craby mascot / logomark, standalone
```

## Design system

- **Direction:** OpenLake + Ramp.
  - From OpenLake: dark cinematic hero, floating pill nav, white document panels on a grey page, tabbed comparison charts, struck-through metric cards.
  - From Ramp: live stat, email capture, product UI as hero art, bottom live ticker, recommendation picker, two-tone statements.
- **Palette:** black, grey and white for every layout. Coral is used only for the mascot, the primary CTA and chart highlights.

  | Token | Hex |
  |---|---|
  | Page | `#F5F5F4` |
  | Panels | `#FFFFFF` |
  | Ink | `#0A0A0A` |
  | Muted | `#6B6B73` |
  | Hairline | `#E4E4E7` |
  | Dark | `#050507` / `#17191D` |
  | Coral | `#D4401F` (4.6:1 with white text) |

- **Type:** Instrument Sans 500 for headlines (tracking -0.035em) and body. Geist Mono only for eyebrows, tickers, metric captions and code.
- **Radius:** 2px everywhere (technical). Fully rounded only for the nav pill, badges and chips.
- **Layout rhythm:**
  1. Dark left hero with a glass card on the right
  2. Model strip
  3. Overlapping console
  4. Split header with sticky steps
  5. Tabs left, chart right
  6. Model cards row
  7. Visual left, text right (Privacy Protect)
  8. Centred bento
  9. Centred statement
  10. Dark band
  11. Centred picker
  12. Calculator
  13. Three-up use cases
  14. Centred pricing
  15. Split FAQ
  16. Dark CTA
  17. Black footer
- **Mascot:** a geometric Craby on a 64px grid, single coral, with a 3px stroke.
- **Charts:** hand-built SVG.
  - Hairline gridlines and 2px lines.
  - Direct labels plus a legend.
  - Coral marks the highlighted series; context series are grey.
  - Tooltips, arrow-key navigation and a table view.

## Before launch: replace every placeholder

Search the file for `PLACEHOLDER` and `PROOF NEEDED`. None of these numbers are real yet.

- [ ] **Hero live stat + bottom ticker** (`TICKER`): connect them to real usage or delete them. Invented traction on a site YC reviewers will open is a credibility risk.
- [ ] **Accuracy chart** (`FT`) and **comparison tabs** (`BARS`): both are labelled illustrative.
- [ ] **Model cards**: the latency figures.
- [ ] **Picker** (`PICKS`): models, policies and token estimates.
- [ ] **Calculator pricing** (`PRICING`).
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
