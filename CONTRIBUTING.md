# 🧭 Contributing to SyncRobotic

Thanks for contributing! This guide covers the conventions shared across all
SyncRobotic repositories. Individual repos may add stack-specific notes in their
own `README.md` / `CLAUDE.md` — always check those for build & test commands.

By participating, you agree to our [Code of Conduct](./CODE_OF_CONDUCT.md).

## 🌿 Branching & promotion flow

We promote changes through tiers:

```
feat/*  or  refactor/*  →  dev  →  stage  →  main
```

- **Cut feature/refactor branches from the latest `dev`** (`git fetch` first —
  local `dev` can be stale). Open your PR against `dev`.
- **Never** branch from another feature branch, and **never** target
  `stage` / `main` directly. Promotion to `stage` and `main` happens via PR from
  the prior tier.
- Branch names: `feat/<short-slug>`, `refactor/<short-slug>`, `fix/<short-slug>`.

## ✍️ Commit messages — Conventional Commits

All commits follow [Conventional Commits](https://www.conventionalcommits.org/)
and are validated by commitlint:

```
feat(scope): add passkey sign-in
fix(api): correct 201 status on camera preview
chore(deps): bump lucide-react
refactor(structure): move ambient types into common/
```

Common types: `feat`, `fix`, `refactor`, `chore`, `docs`, `test`, `ci`, `perf`.
This drives automated, categorized release notes — so write them well.

## 🔀 Pull requests

- **Link an issue.** Reference the issue your PR addresses with a closing
  keyword (`Closes #123`). If a PR intentionally has no issue (chore / deps /
  docs / hotfix), say so and why. The PR template has a section for this.
- **Keep PRs small and focused** — one logical change per PR is easier to review
  and revert.
- **Green before review** — lint, typecheck, and tests should pass. Add or update
  tests for behavior changes.
- **Fill in the PR template** — summary, related issue, changes, checklist.
- Use a Conventional-Commits-style PR title (it becomes the squash-merge commit).

## 🐛 Reporting bugs & requesting features

Open an issue and choose the right template:

- **🐛 Bug Report** · **✨ Feature Request** · **🛠️ Task / Enhancement** · **📌 General Issue**

For how-to questions, see the
[Knowledge Base](https://syncrobotic.atlassian.net/wiki/home) instead.

## 🔒 Security

Never file security problems as public issues — follow the
[Security Policy](./SECURITY.md).

---

Questions about the process? Check the
[Knowledge Base](https://syncrobotic.atlassian.net/wiki/home) or ask a maintainer.
