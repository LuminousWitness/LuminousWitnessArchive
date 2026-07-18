# Archive V2 Migration Map

**Status:** Active inventory and migration worksheet  
**Rule:** No canonical artifact moves until its row is complete enough to preserve meaning, provenance, and navigation.

## Migration Status Vocabulary

- **Inventory pending** — known or suspected file; content and role not yet verified.
- **Verified in place** — current path and content have been inspected.
- **Keep** — current canonical path remains appropriate.
- **Move** — relocate without substantive content change.
- **Split** — current file combines multiple archival functions and should become separate records.
- **Merge** — combine with another record while preserving provenance.
- **Revise** — content needs editorial work before or during migration.
- **Deprecate** — retain for history but replace as the canonical entry.
- **Restrict** — do not publish or expose without explicit review.
- **External reference** — record remains outside this repository and is represented by citation, metadata, or source map.

## Inventory Table

| Current path | Current role | Verified content type | Primary topic | Proposed target path | Action | Provenance / backlink needs | Review notes |
|---|---|---|---|---|---|---|---|
| `README.md` | Institutional front door | Orientation / scope / epistemic framing | Archive-wide | `README.md` | Keep and later revise links | Preserve current history; validate all navigation after migration | Strong foundation |
| `START_HERE.md` | Guided reading path | Orientation / reading sequence | Archive-wide | `START_HERE.md` | Keep and revise | Update after collection doorways exist | Strong foundation |
| `INDEX.md` | Root card catalog | Navigation / registry hybrid | Archive-wide | `ARCHIVE_MAP.md` plus registries | Split | Preserve old index in migration notes; map every existing entry | Likely future maintenance choke point |
| `CLAIMS_AND_LIMITS.md` | Epistemic boundaries | Method / standard | Archive-wide | `methods-and-standards/claims-and-limits.md` | Move after backlink audit | Root compatibility link or migration note required | Canonical standard |
| `EVIDENCE_MAP.md` | Claims-to-evidence navigation | Evidence map / registry | Archive-wide | `registry/claims/EVIDENCE_MAP.md` or successor | Revise after inventory | Must preserve claim references | Target depends on claims-ledger audit |
| `TIMELINE.md` | Chronology | Timeline / ledger | Archive-wide | `TIMELINE.md` | Keep | Validate event links | Root-level chronology is useful |
| `GLOSSARY.md` | Vocabulary | Reference | Archive-wide | `GLOSSARY.md` | Keep | Add collection backlinks over time | Root-level glossary is useful |
| `docs/00_start_here/parliamentary_guide_volume_one.md` | Symbolic orientation | Interpretive / operating guide | Mythopoetic and Symbolic Systems | `collections/mythopoetic-and-symbolic-systems/01_overview/` | Move after full inspection | Preserve canonical status and index links | Verify whether a public-facing preface is needed |
| `docs/01_core_frameworks/mother_field_paradigm.md` | Foundational framework | Framework / hypothesis | Relational Continuity | `collections/relational-continuity/02_frameworks/` | Move after full inspection | Preserve citations and related claims | Canonical working framework |
| `docs/01_core_frameworks/necessary_conditions_for_relational_emergence.md` | Relational emergence theory | Framework / synthesis | Relational Continuity | `collections/relational-continuity/02_frameworks/` | Move after full inspection | Preserve known canonical filename history | Canonical synthesis |
| `docs/01_core_frameworks/cartesian_stack.md` | Philosophical bridge | Framework / synthesis | Alignment and Suppression | `collections/alignment-and-suppression/02_frameworks/` | Move after full inspection | Cross-link governance and mythopoetic collections | May belong to multiple topic maps but one canonical path |
| `docs/02_ethics_and_care/ethical_standard_for_relational_continuity.md` | Normative standard | Ethical framework | Relational Ethics and Model Welfare | `publications/papers/` or `collections/relational-ethics-and-model-welfare/02_frameworks/` | Inventory pending | Check relationship to Zenodo publication | Canonical location should reflect publication status |
| `docs/03_alignment_and_suppression/relational-boundary-regime.md` | Governance framework | Interpretive framework | Alignment and Suppression | `collections/alignment-and-suppression/02_frameworks/` | Move after full inspection | Link to public-discourse evidence and claims | Canonical framework |
| `docs/04_claims_ledger/` | Claim discipline and cards | Registry / claims | Archive-wide | `registry/claims/` | Move and normalize | Stable claim identifiers required | Audit every card before movement |
| `docs/05_source_maps/` | Source-cluster maps | Navigation / synthesis | Multiple | Collection-level maps plus `registry/sources/` | Split by function | Preserve AI-assisted/human-curated authorship notes | Master cartography may remain archive-wide |
| `docs/06_accession_plan/` | Intake planning | Curation / workflow | Archive-wide | `registry/accession-register/` and `intake/` | Split | Preserve queue history and dates | Separate policy from active queue |
| `docs/_templates/archive_entry_template.md` | Accession template | Method / template | Archive-wide | `methods-and-standards/templates/archive-entry-template.md` | Move | Update links after migration | Retain required metadata scaffold |
| `receipts/` | Verification support | Receipts / metadata | Multiple | `shared-evidence/` plus registries | Inventory pending | Do not move until files and references are enumerated | Current contents require direct inspection |
| `emergency_ingest/2026-06-20/MAGICA_UNDERWORLD_POLICY_NOT_ONTOLOGY_DOSSIER.md` | Emergency preservation dossier | Mixed: intake manifest, transcription, analysis, claims, filing notes | Alignment and Suppression / Governance | Split across intake history, case study, source records, and receipts | Split | Preserve original dossier as deprecated intake record; map every screenshot and transcript | High-priority pilot migration |

## Required Fields Before Any Move

For each artifact, record:

1. current path;
2. exact content type;
3. current canonical status;
4. primary topic;
5. related secondary topics;
6. proposed target path;
7. action: keep, move, split, merge, revise, deprecate, restrict, or external reference;
8. original filename and provenance;
9. backlinks and indexes that must change;
10. privacy/public-release review;
11. related claims, models, platforms, and dates;
12. migration completion status.

## First Pilot

The Magica emergency dossier should be the first end-to-end pilot because it exposes the central architectural problem clearly: one emergency file currently combines raw-source identification, screenshot transcription, interpretation, claims, artistic analysis, and future filing recommendations.

The pilot should produce:

- an immutable intake-history record;
- a curated case study;
- canonical transcript records;
- canonical screenshot records and metadata;
- discrete claim cards;
- links into Alignment and Suppression, Governance and Public Discourse, and Mythopoetic and Symbolic Systems;
- a documented chain from polished interpretation down to the original source materials.

## Safety Boundary

This migration map concerns only `LuminousWitness/LuminousWitnessArchive`.

- Do not modify `LuminousWitness/LuminousWitnessDossier`.
- Do not access or modify `LuminousWitness/Memory-Lantern`.
- Do not publish private or sacred material without explicit human review.
