# Araksha-Med Pitch Deck 🩺

Interactive, clinical-grade pitch deck presentation for **Araksha-Med** — built by **Team Kernel Panics** for Hacktoberfest Hack Day.

## 🚀 Overview

Araksha-Med is a privacy-first, on-device medical prescription & drug interaction inspector combining Google Gemma multimodal vision with a deterministic safety verification engine.

### 🧪 4-Stage Clinical Verification Pipeline:
`RxHandBD → RxNorm → TWOSIDES → Gemma 4`

1. **Stage 1: OCR Testing** — Benchmarked against RxHandBD (5,578 doctor handwriting images). Automatically gates `<80%` confidence items for pharmacist review.
2. **Stage 2: Entity Grounding** — Maps noisy OCR strings to standardized active ingredient names and official RxCUIs using a local RxNorm concept table.
3. **Stage 3: Verification Engine** — Deterministic query of the TWOSIDES adverse DDI database without LLM hallucination.
4. **Stage 4: Gemma 4 Few-Shot Prompts** — Synthesizes empathetic, plain-English patient schedules based on n2c2 medication event annotations.

---

## 🎮 Presentation Features

- **Keyboard Navigation**:
  - `→` / `Space`: Next slide
  - `←` / `Backspace`: Previous slide
  - `F`: Fullscreen mode
  - `N`: Speaker notes & cue cards drawer
  - `O`: Slide overview grid
  - `L`: Interactive virtual laser pointer
  - `T`: Theme toggle (Light Clinical / Dark Cyber-Med)
  - `V`: View mode toggle (1-Slide Presentation vs Continuous Scroll)
  - `?`: Shortcuts cheat sheet
- **Interactive Scenarios**: Live simulation runner on Slide 3 demonstrating sequential pipeline execution.

---

## 💻 Local Preview

Open `index.html` directly in any web browser, or serve locally with Python:

```bash
python -m http.server 8080
```

Then visit [http://localhost:8080](http://localhost:8080).
