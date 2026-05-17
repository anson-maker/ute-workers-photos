# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Repository contents

This is an asset-only repository. It contains JPG photos at the root and nothing else (no source code, no package manifests, no build system, no tests, no linters, no CI). The `README.md` is a single line with the project name.

File naming convention at the repo root:
- `F##.jpg` — `F01.jpg` through `F45.jpg`
- `FM##.jpg` — `FM01.jpg`, `FM02.jpg`
- `S##.jpg` — `S02.jpg`, `S03.jpg`
- `angmoh.jpg` — one-off image

Numbering is sparse/non-contiguous in some series (e.g. `S` starts at `02`). Preserve the existing prefix + zero-padded number scheme when adding new files.

## Working in this repo

Because there is no code, the usual "build / lint / test" workflows do not apply. Typical tasks here are:
- Adding, removing, renaming, or replacing image files.
- Editing `README.md`.

When adding binary assets, commit them directly with `git add <file>` (avoid `git add -A` / `git add .` so unrelated files aren't swept in). There is no asset pipeline — files are served as-is from the repo.

## Branch policy

Per the session instructions, develop on the branch named in the task brief (e.g. `claude/add-claude-documentation-kePO0`) and push only to that branch. Do not push to `main` without explicit permission.

## When to expand this file

If code, a build system, or tooling is later added to this repo, replace the "Repository contents" section above with real architecture and command documentation. Until then, do not invent commands or workflows that don't exist here.
