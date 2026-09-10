# Corner Card Executive Demo

Interactive story deck — **Acquisition · Retention · Referral** (Act 03 Deepening hidden in presenter mode).

**Live demo:** [https://zkorczyc.github.io/corner-card-demo/](https://zkorczyc.github.io/corner-card-demo/)

Navigate with **← →**, **space**, or **click**. Jump to a slide with **`#18`** (1-based, visible slides only — hidden deepening slides are skipped).

---

## Preview locally

```bash
python3 -m http.server 8080
# Open http://localhost:8080
```

## Four acts

| Act | Persona | Tagline |
|---|---|---|
| **01 Acquisition** | Marc Weber | Win the right customer |
| **02 Retention** | Sofia Müller · Amex Gold | Win back with relevance |
| **03 Deepening** | Marc Weber | *(hidden in deck)* Grow every relationship |
| **04 Referral** | Marc → Lukas | Close the loop |

**Practitioner:** Claudia Meier (all acts)

## Deploy (GitHub Pages)

This repo **is** the site — `index.html` at the root, no build step.

1. Push to `main` on [zkorczyc/corner-card-demo](https://github.com/zkorczyc/corner-card-demo).
2. **Settings → Pages** → Source: **Deploy from branch** → `main` → **`/ (root)`**.
3. Wait ~1–2 minutes. Site: `https://zkorczyc.github.io/corner-card-demo/`

`.nojekyll` is included so GitHub Pages serves assets as-is.

## Repository layout

| Path | Purpose |
|---|---|
| `index.html` | Self-contained interactive deck |
| `assets/` | Persona portraits, device mocks, creatives |
| `adobe-wordmark-red.svg` | Footer wordmark |

Planning docs (story, steps, validations) live in the parent monorepo under `corner-card/` — not required to run the deck.

## Live demo (hybrid)

For sessions that switch from this deck into **live RTCDP / AJO / CJA**:

| Doc | Purpose |
|---|---|
| [../live-demo-runbook.md](../live-demo-runbook.md) | Slide ↔ live ↔ fallback, timing, rehearsal |
| [../live-demo-sandbox-setup.md](../live-demo-sandbox-setup.md) | Profiles, audiences, bookmarks |
| [../live-demo-journeys-setup.md](../live-demo-journeys-setup.md) | AJO canvas specs |
| [../live-demo-cja-setup.md](../live-demo-cja-setup.md) | CJA funnel + CPA panels |
| [talk-track.md](talk-track.md) | Live transition cues |

## Maintenance notes

- **Act 03 Deepening:** slides use class `slide-hidden` — remove to restore in navigation.
- Replace remaining `img-ph` placeholders with Adobe UI screenshots when ready.
