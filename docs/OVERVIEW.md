# Repository Overview: St-John-Software/.github

## Purpose

This is the GitHub organization profile repository for **St John Software**. It serves as the public-facing identity for the organization on GitHub — the `profile/README.md` file is automatically displayed on the organization's GitHub profile page. The root `README.md` provides a minimal label for the repository itself.

## Architecture

```
.github/
├── README.md           # Repository label ("# .github / St John Software")
├── profile/
│   └── README.md       # GitHub org profile page (rendered at github.com/St-John-Software)
└── docs/
    └── OVERVIEW.md     # This file
```

**Key files:**

- `profile/README.md` — The only content rendered publicly. GitHub automatically displays this on the organization's profile page. Currently contains the default GitHub template with commented-out placeholder suggestions but no visible content.
- `README.md` — Minimal root README, not rendered on the org profile.

## Key Patterns

- **GitHub special repo**: The `.github` repository name is reserved by GitHub for organization-level defaults (issue templates, workflow templates, etc.). The `profile/` subdirectory is specifically for the org profile page.
- **Markdown only**: All content is Markdown. No code, build system, or dependencies.
- **Profile content**: The `profile/README.md` supports full GitHub-flavored Markdown including badges, images, and HTML.

## Configuration

No environment variables or configuration values. This repository has no CI/CD workflows, no actions, and no branch protection rules currently defined.

## Extending This Repo

Common additions to a `.github` org repository:
- `.github/ISSUE_TEMPLATE/` — Default issue templates applied to all repos in the org that don't define their own.
- `.github/PULL_REQUEST_TEMPLATE.md` — Default PR template for org repos.
- `.github/workflows/` — Reusable workflows (called via `workflow_call`).
- `profile/README.md` — Fill in the org profile with description, links, and badges.
