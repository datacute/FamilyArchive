# Contributing

Thanks for helping preserve our family history. Small, incremental contributions are welcome.

## Ways to contribute
- Share stories or corrections in plain text/Markdown.
- Add person pages (`people/`) or source records (`sources/`).
- Improve OCR: edit `ocr-corrected.md` while keeping `ocr.txt` unchanged.
- Add dates/places/citations to existing pages.

## For non-technical contributors
- You can write content in a document and send it to a maintainer to add.
- Or edit Markdown files directly in the GitHub web UI if you have access.
- Keep personal/sensitive details about living people minimal; mark privacy as `restricted` when unsure.

## For technical contributors
- Follow the folder and ID conventions in `METADATA/folder-structure.md`.
- People live under `people/<SURNAME>/<UID>-<slug>/index.md` with YAML front matter.
- Sources live under `sources/<SID>-<type>-<year>-<slug>/` with `source.md`, `ocr.txt`, and optional `ocr-corrected.md`.
- Link people ↔ sources using `uid`/`sid`, not filenames.

## Naming and IDs
- People IDs: `P####` (e.g., `P0001`); Source IDs: `S####` (e.g., `S0012`). IDs are permanent.
- Slugs: lowercase, hyphenated, include disambiguators like years (e.g., `john-smith-1856-1932`).

## Front matter templates
See examples in `NOTES/2025-08-30-initial-conversation.md` and align with `METADATA/metadata-schema.md` (to be added).

## Privacy
- Living persons: set `privacy: restricted` and avoid publishing exact birthdates/addresses.
- Remove or redact sensitive info on request.
- If unsure, ask a maintainer before committing.

## Review flow
1. Open a pull request summarizing the change.
2. Ensure links to `UID`/`SID` resolve.
3. A maintainer reviews for structure, privacy, and citations.
4. Merge when checks pass.

