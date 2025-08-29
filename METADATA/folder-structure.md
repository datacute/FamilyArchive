# Folder structure and conventions

Version: 0.1 (draft)

## Top-level
- `people/` — one folder per person with stable `uid` and profile page.
- `sources/` — one folder per original record with stable `sid` and OCR.
- `narratives/` — essays and family stories.
- `indexes/` — curated/generated indices (surnames, people, places, timeline).
- `METADATA/` — conventions and schemas.
- `NOTES/` — working notes and conversations.

## People
Path: `people/<SURNAME>/<UID>-<slug>/index.md`
- `UID`: `P####` (e.g., `P0001`), never changes.
- `slug`: lowercase, hyphen-separated; include disambiguators like years.
- Front matter fields (minimum):
  - `uid`, `given`, `surname`
  - `birth.date`, `birth.place` (if known)
  - `death.date`, `death.place` (if known)
  - `parents`, `spouses`, `children` (arrays of `UID`s)
  - `sources` (array of `SID`s)
  - `privacy`: `public|restricted`

## Sources
Path: `sources/<SID>-<type>-<year>-<slug>/`
- Files: `source.md`, `ocr.txt` (raw), `ocr-corrected.md` (optional)
- `SID`: `S####` (e.g., `S0012`), never changes.
- Front matter fields (minimum in `source.md`):
  - `sid`, `type`, `date`, `place`
  - `people` (array of `UID`s)
  - `citation`
  - `external.onedrive` (URL), `archive_uri` (optional)
  - `tags` (optional)

## Narratives
Path: `narratives/<topic-or-person-uid>/index.md`
- Use front matter to link related `UID`s and `SID`s.

## Indexes
- Markdown lists the preferred UX until automated generation is added.

## Filenames and characters
- Use ASCII letters, digits, hyphens; avoid spaces and special characters.
- Dates in `YYYY-MM-DD` when known; otherwise year-only is acceptable.

## OneDrive and external storage
- Store originals in OneDrive with a mirrored logical structure if helpful.
- Link from `source.md` via `external.onedrive`.

## Changes to this spec
- Propose updates via PRs. Major changes get an ADR in `DECISIONS/`.
