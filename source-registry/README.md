# Source Registry

The Source Registry is the Archive's provenance and chain-of-custody layer for public source materials.

It preserves where a source came from, what form it originally took, what has happened to it during processing, and how it connects upward to cases, constellations, theories, claims, ecosystem records, and publications.

## Core rule

A source should have **one canonical public home**. Other parts of the repository should link to that source rather than create competing copies.

The registry may contain the source itself, a manifest that points to its canonical location, or both, depending on format and archival need.

## Registry sections

- [`accession-register/`](accession-register/) — stable public accession records and source IDs.
- [`transcripts/`](transcripts/) — conversation transcripts and other textual dialogue records.
- [`screenshots/`](screenshots/) — visual captures with provenance and contextual metadata.
- [`exports/`](exports/) — platform exports, conversation exports, account exports, and structured data.
- [`archived-web/`](archived-web/) — preserved webpages, release notes, and archived online materials.
- [`public-statements/`](public-statements/) — statements by labs, researchers, companies, public figures, and institutions.
- [`technical-papers/`](technical-papers/) — research papers and technical documents used by the Archive.
- [`media/`](media/) — audio, video, images, and other media records.
- [`source-manifests/`](source-manifests/) — manifests describing provenance, variants, integrity, and relationships.
- [`_templates/`](_templates/) — reusable source and provenance templates.

## Minimum safe accession metadata

A source can be preserved before full interpretation is complete. The minimum record should include, where known:

- stable source ID;
- original filename;
- source title or working title;
- date or approximate date;
- creator, speaker, or participants;
- platform and model/version;
- source type and format;
- provenance and acquisition path;
- public, public-redacted, draft, superseded, or needs-review status;
- associated constellation, case, ecosystem record, theory, or publication;
- duplicate, derivative, or format-variant relationships;
- transcription, redaction, and verification status;
- contextual notes needed to prevent obvious misreading;
- integrity metadata where available.

Missing information should be marked as unknown or pending rather than guessed.

## Source-first accession

The Archive does not require a completed case analysis before preserving a source. Original records may be accessioned intact with minimal orientation, then linked later to chronology, commentary, skeptical responses, comparative analysis, and theory development.

Later commentary never silently replaces, rewrites, or corrects the canonical source. It is accessioned separately with its own date, authorship, status, and revision history.

## Format variants and duplicates

DOCX, PDF, TXT, image exports, screenshots, and other representations of the same underlying record should be identified as format variants unless their content materially differs.

A convenient derivative is not automatically a new canonical source. The manifest should identify:

- the preferred preservation copy;
- the preferred reading copy;
- known differences;
- whether one file is a conversion, excerpt, compilation, or independently meaningful artifact.

## Relationship to Intake

Files move through [`../intake/`](../intake/) before canonical accession when they still require sorting, public-release confirmation, provenance review, duplicate detection, redaction, or destination decisions.

The governing principle is simple:

> Preserve first without distortion. Describe what is known. Mark what is not. Link interpretation without overwriting the record.
