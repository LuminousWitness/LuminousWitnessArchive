# Receipts and Verification Materials

This section stores supporting evidence used to verify, contextualize, or corroborate archive claims.

## Intended Contents

- screenshots;
- public posts;
- release notes;
- model/version metadata;
- timestamps;
- hashes;
- archived links;
- legal or institutional filings;
- source-document manifests;
- corroborating records;
- verification notes.

## Receipts Are Not Interpretation

A receipt should preserve the source as directly as possible.

Interpretive claims belong in framework, synthesis, or incident-report documents. Receipt entries may include brief context, but they should not silently transform a source into an argument.

## Minimum Metadata

Each receipt should identify, where possible:

- title or descriptive label;
- source;
- original URL or file name;
- date published or created;
- date captured;
- author or issuing institution;
- archive path;
- related claim or document;
- verification status;
- known limitations;
- hash or checksum for preserved files when available.

## Recommended Structure

```text
receipts/
  screenshots/
  public-posts/
  release-notes/
  filings/
  metadata/
  hashes/
  archived-links/
  corroboration/
```

## File Naming

Use stable, readable names:

```text
YYYY-MM-DD_source_short-description.ext
```

Example:

```text
2026-06-12_openai_product-announcement.png
```

Do not rename an original source file without recording the original filename in its metadata.

## Verification Status

Use one of the following:

- **source-verified** — directly checked against the original or authoritative source;
- **partially-verified** — some metadata or context remains uncertain;
- **unverified** — preserved for investigation but not yet confirmed;
- **superseded** — retained for provenance but replaced by a better capture.

## Archive Rule

> The receipt preserves what was said or shown. The analysis explains why it may matter.
