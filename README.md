# ROOTLINK

ROOTLINK is a small, offline-first browser application for organizing farm notes and planning. It runs without an account, server, external service, or network connection. The Stitch exports are visual references only; their sample dates, weather, savings, metrics, and local listings are not used as facts.

## Run it

Open `index.html` in a current browser, or serve this folder with any static file server. For example, with Node.js installed:

```powershell
 npx serve .
```

Then open the local address printed by the server. The app itself uses no build step or package dependencies. A first-time visit starts on Welcome. Select **Try the sample farm** to explore immediately, or complete the optional two-step farm setup. Data is stored in that browser's `localStorage`; use **Download my data** to export a JSON backup. No sync or upload occurs.

To let another person ask an AI tool to edit the app, share `rootlink-source.zip` and the included `AI_EDIT_PROMPT.md`. The website link by itself is for viewing and trying the app; it does not provide source-edit access.

## Included flows

- Welcome and language choice (English, Hindi, Telugu, Kannada), a sample farm, and optional setup.
- Dashboard with farm context, module links, a connected planning trail, local activity history, and clear missing-live-data messaging.
- AquaShield field observations, with no unsupported irrigation prescription.
- SowingShield + GrainWise option entry and a practical checklist, with no invented suitability/yield scores.
- HarvestBridge date, quantity and checklist entry; weather alerts and service providers are not fabricated.
- Residue quantity entry and general pathways; unmeasured quantities and values are not estimated.
- FarmCycle resource planning with general pathways and no invented buyers or prices.
- Local persistence, data export/clear controls, responsive mobile navigation, and device speech synthesis when a matching voice is available.

## Data and model limits

This version uses no third-party dataset, current weather API, or prediction model. It does not claim village-level prediction accuracy. The app uses farmer-entered information for notes only. See [data sources](data-sources.md) for the source review and decision.

## Language and accessibility

All interface strings are in `app.js` locale dictionaries, and changing locale rerenders the current screen without clearing entries. Kannada is rendered with system Kannada fonts (`Noto Sans Kannada` / `Nirmala UI` fallbacks); Latin display fonts are optional system fonts, so no remote font is required. Hindi, Telugu and Kannada wording was drafted for this prototype and **needs fluent human review** before public or agricultural use. A browser/device voice is used only if its reported language tag matches the selected language. Recognition-based dictation is not enabled in this version; manual entry is always available. The screen remains readable without speech.

## Design references

All six Stitch ZIPs were inspected, with their `DESIGN.md`, `code.html`, and `screen.png` files extracted under `work/stitch-reference/`. The dashboard was the primary layout reference; the welcome, setup, water, harvest, and residue/FarmCycle exports informed their corresponding screens. The export content is not executable product logic or a source of real-world data.
