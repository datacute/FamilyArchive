# Vision

FamilyArchive preserves, organizes, and shares our family’s history in durable, open formats so future generations can discover people, places, and stories with clarity and care.

## Scope
- Preserve high-quality scans and trustworthy transcriptions of original sources.
- Maintain structured person pages with relationships and citations.
- Provide simple, permanent links for non-technical relatives through a publishable site.
- Keep the content portable: plain text/Markdown, YAML front matter, open file formats.

## Principles
- Source-first: every claim cites a source. Distinguish facts, transcriptions, and interpretations.
- Stable identifiers: people (UID: P####) and sources (SID: S####) never change.
- Separation of concerns: preservation (scans + text) vs presentation (browse/search UI).
- Privacy by default for living people and sensitive material.
- Incremental improvement: accept rough OCR now, refine over time with clear diffs.

## Content layers
- Preservation: originals in OneDrive (or similar), plus raw OCR and corrected transcriptions in the repo.
- Structure: Markdown with YAML front matter for people, sources, and narratives.
- Presentation: a static site generator (added later) that renders people, sources, and stories with search.

## Success criteria
- Families can find a person, see relationships, and open cited sources in 3 clicks or fewer.
- Every fact on person pages links to at least one source (SID).
- All content is cloneable, readable, and editable offline using standard tools.
- Regular backups and export paths exist to migrate elsewhere if needed.

