# Data source and model manifest

Retrieval date for this review: 2026-11-24.

| Source | Publisher / license | Coverage and fields | Use in ROOTLINK |
|---|---|---|---|
| None integrated | — | — | This build includes no external dataset, API, trained model, or prediction. |

## Candidate review

The supplied project contained no datasets, credentials, or existing data pipeline. No Kaggle dataset was added: dataset-level license terms, Indian district/crop/season coverage, provenance, and target-field quality were not verified for any specific candidate, so using one to produce crop or yield advice would be unjustified. No public Git/GitHub dataset was added for the same reason: a public repository alone does not establish data reuse rights or reliable field-level provenance. No IMD endpoint or other current weather source is configured. Historical/reanalysis weather would not be treated as a live forecast. These are deliberate exclusions, not missing source attributions.

## Implemented behavior

- AquaShield stores the farmer's selected field observation and optional note. It calculates no irrigation demand, stress category, savings, or timing.
- SowingShield + GrainWise stores selected crop options and field inputs. It does not rank suitability, forecast planting windows, estimate yield, or simulate climate scenarios.
- HarvestBridge stores farmer-entered dates, production quantity, notes, and checklist state. It generates no harvest forecast or weather risk.
- Residue Intelligence stores farmer-entered production and measured residue. It does not derive residue quantity or value from generic factors.
- FarmCycle stores a resource note and presents general pathways only. There are no actual listings, rates, distances, or availability claims.

All saved data is local to the browser profile. It is not sent to a server or synchronized.
