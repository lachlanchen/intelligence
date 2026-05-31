# Repository Guidelines

## Project Structure & Module Organization

This repository is a reference archive, not an application codebase. All repository assets are under `references/`.

- `references/papers/`: curated PDF papers for research context.
- `references/repos/MetaBCI/`: snapshot of the MetaBCI repository.
- `references/repos/autonomous-drone-racing/`: snapshot of the Awesome Autonomous Drone Racing list/references.

When adding material:
- Keep new content under `references/`.
- Use content-based, descriptive filenames.
- For PDF naming, include year/topic, e.g. `2025-Brain-organoid-computing-overview.pdf`.

## Build, Test, and Development Commands

There are no build or test pipelines for this top-level repository.

- `git status`: verify what changed before commit.
- `git log --oneline --references`: review commit history and message style.
- `git add references/... && git commit -m "..."`: only required workflow for contributor updates.

## Coding Style & Naming Conventions

Because this repo stores references, style rules apply to metadata and docs:
- Markdown: sentence case headings, concise language, one line per paragraph.
- Filenames: `YYYY-Short-Descriptive-Title.ext`, hyphen-separated words, no spaces.
- Directories: lower-case with hyphens if needed, e.g. `references/papers`.

## Testing Guidelines

No automated test suite is configured in this repository.

- Validate links in this repo manually (local file presence).
- If added repositories include tests, run their tests inside `references/repos/<repo>` only when explicitly changing those upstream contents.

## Commit & Pull Request Guidelines

Recent commits in this repo use simple imperative summaries.

- Prefer short imperative commit messages that describe the change:
  - `Add ...`
  - `Vendor in ...`
  - `Rename ...`
- Keep each commit scoped to one change set (e.g., add one paper set or one reference repo).
- In PRs, include:
  - what changed,
  - source locations (URLs or file paths),
  - why it was added,
  - any known size impact.

## Security & Repository Hygiene

- Use only trusted repository URLs before cloning or copying.
- Do not commit sensitive credentials or API keys in commit history.
- Store large binary files only when needed; avoid unnecessary duplicates.
