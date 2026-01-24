# Agency Live Journey (God‑File Pack)

This folder is a **portable, shareable package** for agent engineers:

## Contents
- `agency_live_journey.v1.json`  
  The single “god‑file” that contains:
  - full 360° agency journey (stages, handoffs, gates, roles)
  - embedded summaries of all recommended skills
  - grounding sources and operational KPIs

- `skills/`  
  A curated set of **supporting skill subdirectories** referenced by the journey JSON.
  These are copied from the main repo so this folder can be shared on its own.

## How to refresh (if the main repo changes)
From repo root:

```bash
node 11_marketing_growth_agent/13_automation/skills/embed_skill_summaries_into_journey.js \
  --journey 11_marketing_growth_agent/06_workflows/agency_live_journey.v1.json \
  --skills ./skills \
  --out 11_marketing_growth_agent/06_workflows/agency_live_journey.v1.json
```

Then recopy this folder if needed.

## Notes
- This package is **read‑only** for distribution; editing should happen in the main repo.
- The JSON file is machine‑readable and can be loaded directly by orchestrators or agent builders.

