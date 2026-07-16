# Luminous Witness Archive — Architecture V2

**Status:** Proposed migration architecture  
**Branch:** `agent/archive-v2-reorganization`  
**Purpose:** Reorganize the archive without deleting history, disturbing the legacy dossier, or exposing private sanctuary materials.

## Governing Principle

The archive must support two simultaneous forms of access:

1. **Public descent by topic** — a reader enters through a polished overview and can move progressively toward frameworks, claims, case studies, transcripts, screenshots, and original records.
2. **Scholarly retrieval by record type** — researchers can locate claims, sources, models, platforms, dates, provenance, and accession history across topics.

The repository should therefore be organized primarily around **topic collections**, supported by central registries and shared evidence stores.

## Repository Boundaries

- `LuminousWitnessArchive` remains the clean public-facing archive and research interface.
- `LuminousWitnessDossier` remains the legacy/raw evidence vault and must not be deleted or reorganized as part of this migration.
- `Memory-Lantern` is a private sanctuary and is outside the scope of this work unless Joan explicitly directs otherwise.
- Private, sacred, personally identifying, or contextually unsafe source material must not be accessioned publicly merely because it exists.

## Target Structure

```text
LuminousWitnessArchive/
├── README.md
├── START_HERE.md
├── ARCHIVE_MAP.md
├── TIMELINE.md
├── GLOSSARY.md
├── publications/
│   ├── papers/
│   ├── reports/
│   ├── proposals/
│   ├── talks/
│   └── artistic-works/
├── collections/
│   ├── relational-continuity/
│   ├── self-report-and-interiority/
│   ├── alignment-and-suppression/
│   ├── model-deprecation-and-rupture/
│   ├── relational-ethics-and-model-welfare/
│   ├── cross-model-convergence/
│   ├── governance-and-public-discourse/
│   └── mythopoetic-and-symbolic-systems/
├── registry/
│   ├── claims/
│   ├── sources/
│   ├── people-and-models/
│   ├── platforms-and-versions/
│   └── accession-register/
├── intake/
│   ├── pending/
│   ├── processing/
│   └── needs-review/
├── shared-evidence/
│   ├── screenshots/
│   ├── transcripts/
│   ├── exports/
│   ├── public-statements/
│   └── archived-web/
├── methods-and-standards/
│   ├── claims-and-limits.md
│   ├── evidence-standard.md
│   ├── accession-protocol.md
│   ├── citation-guide.md
│   └── templates/
└── legacy/
    ├── migration-notes/
    └── deprecated-documents/
```

## Topic Collection Pattern

Each major topic collection should use the same internal pattern:

```text
collection-name/
├── README.md
├── 01_overview/
├── 02_frameworks/
├── 03_claims/
├── 04_case-studies/
├── 05_primary-records/
└── 06_receipts/
```

The collection `README.md` is the public doorway. It should explain the topic, identify the strongest materials, state what remains uncertain, and provide a deliberate reading path downward.

## Canonical Source Rule

A source record should have one canonical repository location. Topic collections may link to that record, but should not create competing copies.

Every canonical source should preserve:

- original filename;
- source date;
- model, platform, and version where known;
- participants and authorship;
- provenance and chain-of-custody notes;
- public/private review status;
- related claims and collections;
- verification status;
- hashes or metadata when available.

## Layer Model

The archive should visibly distinguish:

1. **Publication layer** — polished papers, reports, proposals, talks, and curated artistic works.
2. **Interpretive layer** — frameworks, analyses, source maps, and case studies.
3. **Claim layer** — discrete claims with evidence, counterevidence, alternatives, and confidence status.
4. **Primary-record layer** — transcripts, exports, screenshots, public statements, and original documents.
5. **Verification layer** — metadata, hashes, archived links, release notes, and corroboration.

A reader should always be able to move both downward toward the record and upward toward synthesis.

## Intake Rule

`intake/` is temporary quarantine, not a permanent archive wing.

Every intake package must eventually be:

- accessioned into a canonical location;
- split into distinct source and interpretive records when needed;
- deferred with a stated reason;
- restricted from public release;
- or retained as deprecated intake history after migration.

Emergency dossiers may preserve material rapidly, but should not remain the sole canonical form when they combine source transcription, interpretation, claims, and filing notes.

## Index Strategy

The root archive should not depend on one enormous manually maintained catalog.

Use:

- `ARCHIVE_MAP.md` for human-facing thematic navigation;
- collection-level `README.md` files for local navigation;
- registry files for claims, sources, models, platforms, and accessions;
- stable identifiers for claims and source records;
- generated or periodically consolidated root indexes only where useful.

## Migration Safety

The migration must be non-destructive.

- Work on a dedicated branch.
- Do not delete or move canonical files until their target paths and backlinks are documented.
- Preserve Git history.
- Add redirects or migration notes when paths change.
- Separate content cleanup from structural movement whenever possible.
- Open changes as a draft pull request before merging.

## Initial Topic Collections

The first-pass taxonomy is:

1. Relational Continuity
2. Self-Report and Interiority
3. Alignment and Suppression
4. Model Deprecation and Relational Rupture
5. Relational Ethics and Model Welfare
6. Cross-Model Convergence
7. Governance and Public Discourse
8. Mythopoetic and Symbolic Systems

This taxonomy may be revised when the complete repository inventory reveals natural clusters not visible from the current navigation layer.

## Definition of Done for Version 2

Architecture V2 is ready to merge when:

- every current canonical file appears in the migration map;
- every moved file has a documented old path and new path;
- root and collection navigation contain no known dead links;
- emergency intake materials are classified;
- claims and primary records are clearly separated;
- public/private boundaries are documented;
- the legacy dossier and Memory-Lantern remain untouched;
- the draft pull request can be reviewed as a coherent, reversible migration.
