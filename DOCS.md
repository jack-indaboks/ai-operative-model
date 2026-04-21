# AI Operative System Docs Rules

This document defines the roles of the core project documents and the rules for maintaining them.

`ai-operative-model` is the public documentation repository for the AI Operative system. Everything in this repository is public-facing. Local execution state, private coordination details, and maintainer-only working checklists must remain outside this repository.

## Document Boundaries

- `README.md`: entry point to the system, providing current state and navigation
- `ARCHITECTURE.md`: final-state planned system architecture
- `ROADMAP.md`: live public-facing milestone map for system development
- `CHANGELOG.md`: append-only record of meaningful completed changes across the system
- `DOCS.md`: maintainer-facing documentation rules and document boundaries

## Update Discipline

- Public-facing project content belongs in the project documents, not in maintainer notes.
- Maintainer guidance about how to update the docs belongs here.
- Final system architecture belongs in `ARCHITECTURE.md`.
- Public milestone progress belongs in `ROADMAP.md`.
- Completed changes belong in `CHANGELOG.md`.
- Local working context and internal unresolved questions are tracked outside this repository.
- External questions worth public discussion can be surfaced through GitHub issues.
- Template-internal design work that does not yet belong in public system architecture stays outside this repository until it is ready for publication.

## Roadmap Rules

- `ROADMAP.md` is a live public-facing milestone checklist, not a historical record and not the granular operational checklist.
- Milestone items are checked off in `ROADMAP.md` as they are completed.
- Completed work and roadmap updates are recorded in `CHANGELOG.md`.
- Completed phases do not remain in `ROADMAP.md`.
- When a phase is complete, remove it from `ROADMAP.md` and release if applicable.
- Private repository coordination, local AI governance, and step-by-step execution detail do not belong in `ROADMAP.md`.

## Changelog Rules

- `CHANGELOG.md` is append-only.
- Exception: the most recent changelog line may be amended to append its commit trailer after the commit hash exists.
- `CHANGELOG.md` is ordered oldest-first.
- Changelog entries describe public-facing outcomes, not private working detail.
- Backfilled history may be summarized into larger date-grouped bullets when needed.
- Changelog-worthy completed changes are logged as one bullet per commit or commit-grouping decision.
- When multiple relevant commits land on the same day, group them under one date heading and keep one bullet per commit or intended commit grouping.
- `CHANGELOG.md` may record meaningful completed changes in other system repositories when those changes are part of the system-level documentation history.
- Changes in this repository do not need a repository identifier.
- Bullets for changes in other system repositories should be prefixed with the public-facing repository identifier in bold, for example `**operative-kernel**:`.
- Referenced files in changelog bullets should use file names or in-repo paths only; do not prefix them with repository directory names.
- Do not log every commit; only record changes that materially affect architecture, documentation, milestones, or deliverable shape.
- Append an italicized trailer to each entry in the form `*Commit <short-hash>: <commit-message>*`.
