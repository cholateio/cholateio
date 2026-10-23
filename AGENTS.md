<!-- Tool-neutral project memory. Never put local paths, costs or personal data here. -->
# cholateio

## Project goal

The GitHub profile README for the `cholateio` account: a hub page that introduces each public project with a one-line description and a link.

## Stack

- Language / framework: Markdown + inline HTML, rendered by GitHub on the profile page
- Services: none
- Test: none (no code); preview the rendered README on GitHub, and check that every relative image path in `README.md` and `README.zh-TW.md` exists under `assets/`

## File layout

- `README.md` — the profile page in English (featured project, then tables grouped by kind)
- `README.zh-TW.md` — Traditional Chinese (Taiwan) translation of `README.md`
- `assets/` — images referenced by `README.md` and `README.zh-TW.md` (webp)

## Constraints

- Link only to public repositories and public sites; never link a private repository (a private project may appear only through its public site).
- Keep images small (webp) and give every `<img>` an `alt` text that describes it.
- Path-type constraints are mirrored in `kit.toml [protected]`; keep the two in sync (one glob per line).

## Conventions

- Commit messages: `docs: ...` (for example `docs: add <project> to the tools table`).
- Table rows: project link, one sentence on what it does, month and year started.
- `README.md` (English, default) and `README.zh-TW.md` (Traditional Chinese) mirror each other; this profile repo stays English-first, unlike the other repos; update both in the same commit.

## Where to look

- `README.md` and `README.zh-TW.md` — the only content files (English and Traditional Chinese)
