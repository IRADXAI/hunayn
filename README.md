# Hunayn

AI radiology dictation assistant. Dictate key findings; Hunayn drafts the complete, guideline-correlated report.

Named for Hunayn ibn Ishaq (809–873), the Assyrian Christian physician-translator of Baghdad's House of Wisdom and author of the first systematic treatise on the eye — reportedly paid in gold by the weight of his manuscripts, because accuracy was the product.

## Contents

- `hunayn.jsx` — the app. React single-file artifact: modality selection, preset template support, dictation box with built in speech recognition, paste-a-screenshot capture of tech sheets and graphs, full or fragmented report output with per-section copy buttons, brief clinician message, timestamped quick text, NPI-gated registration (currently behind `LOGIN_ENABLED = false`).
- `hunayn-landing.html` — landing page for hunayn.ai. Self-contained, no build step.

## Features

- Report generation via the Anthropic API (Claude Sonnet), integrating dictated findings into complete reports with standard normals, calculations (volumes, interval growth), and named society guidelines (Fleischner, TI-RADS, LI-RADS, Bosniak, O-RADS, ACR incidental findings).
- NPI registration verified against the CMS NPPES registry; not offered in Michigan or Maine.
- Rex, the scroll-carrying skeleton mascot.

## Setup notes

- Flip `LOGIN_ENABLED` to `true` to enable NPI-gated registration.
- Landing page CTAs point at `#` until the app is hosted.

## Legal

Educational drafting aid for licensed physicians only. Not a medical device; does not diagnose or treat. Output may contain errors and must be independently verified in full by the signing physician. No PHI. Full terms in-app.

© 2026 · hunayn.ai
