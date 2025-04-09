# Git Strategy

This document outlines the Git strategy for working with the Cypress project in this repository.

## 1. Repository Initialization

- This is a **public repository** initialized to host a Cypress end-to-end testing project.
- A **Cypress project** has been initialized in the root directory.
- A `.gitignore` file has been configured to exclude files and directories specific to Cypress (e.g., `node_modules/`, `cypress/videos/`, `cypress/screenshots/`, etc.).

## 2. Git Workflow Strategy

To ensure smooth collaboration, maintainable code, and a clean Git history, the following Git workflow strategy is adopted.

### Branching Strategy

We use a **trunk-based development** model with the following branches:

- `main`: The stable production branch.
- `dev`: The integration branch for ongoing development.
- `feature/*`: Feature branches for individual tasks.
- `bugfix/*`: Bug fix branches.
- `hotfix/*`: Emergency fixes to be merged into `main`.

### Branch Naming Conventions

- Feature branches: `feature/<short-description>`
- Bugfix branches: `bugfix/<issue-id>-<short-description>`
- Hotfix branches: `hotfix/<short-description>`

Example:  
`feature/login-tests`  
`bugfix/123-fix-timeout-error`

### Rules and Best Practices

- All work should begin on a feature, bugfix, or hotfix branch.
- **Never commit directly to `main` or `dev`.**
- Create a **pull request (PR)** to merge changes into `dev` or `main`.
- All PRs must be reviewed and approved by at least one team member.
- Ensure all tests pass before merging a PR.
- Rebase frequently to keep branches up to date with `dev`.
- Squash commits before merging to keep the history clean.

### Merge Strategy

- Use **squash and merge** for PRs.
- Use **fast-forward merges** for hotfixes into `main`.

---

_This file is located at `/docs/git-strategy.md`._
