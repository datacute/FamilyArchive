# Roadmap

This is a living plan. Tackle phases sequentially but keep tasks small and reversible.

## Phase 0 — Repo hygiene (now)
- Store planning conversation in `NOTES/` (done).
- Establish repo structure and conventions (`METADATA/`).
- Draft vision, roadmap, contributing (done).

## Phase 1 — Conventions and scaffolding
- Decide ID scheme length and format for `P####` and `S####` (default: 4 digits).
- Finalize front matter fields for people and sources; add minimal JSON Schema/YAML examples.
- Create starter folders: `people/`, `sources/`, `narratives/`, `indexes/`.
- Add `METADATA/metadata-schema.md` and `METADATA/file-naming.md` (TBD).

## Phase 2 — Ingest and OCR
- Pick scanning defaults: 600dpi TIFF/PNG for documents, 300–600dpi for photos; store originals in OneDrive.
- Create OneDrive folder alignment and permalink approach.
- Add first 10 sources with `source.md`, `ocr.txt`, and optional `ocr-corrected.md`.

## Phase 3 — People pages
- Create first 10 person profiles with YAML front matter and short bios.
- Link each fact to `SID`s; add relationships by `UID`.
- Start curated indices in `indexes/` (surnames, people, timeline).

## Phase 4 — Presentation
- Choose a static site generator (MkDocs, Hugo, Eleventy) and a private hosting option.
- Generate person/source pages and listings; ensure stable, human-shareable URLs.
- Add basic client-side search across names, dates, places, and tags.

## Phase 5 — Search and enrichment
- Extend search to OCR and corrected transcriptions.
- Consider fuzzy search and tags (places, decades, events).
- Optional: embeddings for semantic search (private only).

## Phase 6 — Automation and QA
- Lint YAML front matter and check cross-links (UID/SID existence).
- Add CI to validate structure and generate indices.
- Add backup/export scripts (HTML/PDF snapshot + content ZIP).

## Phase 7 — Preservation
- Schedule periodic offline backups.
- Consider PDF/A for key documents and long-term storage options.
- Document a migration path out of current tools.

## Immediate next actions
- Confirm ID scheme and lock it in `METADATA/folder-structure.md`.
- Add first person (`P0001`) and first source (`S0001`) as exemplars.
- Decide the presentation tool to trial in Phase 4.

