# Contributing

Team members: everything about how we work lives in the [engineering handbook](https://github.com/Syncrobotic/SyncAI-Docs-Handbook). It takes ten minutes to read. This page is the short version, and if the two ever disagree, the handbook wins.

## The short version

**Branch from `dev`, PR back into `dev`.** Name the branch `<type>/<short-slug>`, for example `feat/123-camera-preview`. Changes reach `stage` and `main` only through promotion PRs, which repo owners open. Never target `stage` or `main` with a feature.

**Write commits and PR titles in English, as [Conventional Commits](https://www.conventionalcommits.org/).** `feat(api): add camera preview`, `fix(docker): run migrations in the server only`. They become the changelog. Descriptions and issue bodies can be in any language.

**Squash or merge, your call. Promotions are never squashed.** Squash suits a small PR. If you merge, every commit lands on `dev`, so tidy them first. Promotions always use a merge commit, so `dev`, `stage` and `main` keep one shared history.

**One PR, one change.** Link the issue with `Closes #123`, or say why there isn't one. Keep it under about 400 lines. CI must be green and a code owner must approve. Nobody approves their own PR.

**Anything with a screen uses the [design system](https://design-system.syncrobotic.me).** Internal tools included.

**Secrets never go into git.** Use `.env` locally and keep a `.env.example` with names only.

## Issues

Pick a template. Write the title in English as `[Area] what should happen`. Give one deliverable and acceptance criteria someone can check. Repo owners triage weekly and set the priority label (`P0` to `P3`).

Product questions and how-to guides live in [Confluence](https://syncrobotic.atlassian.net/wiki/home). Security problems go through the [security policy](SECURITY.md), never a public issue.

By taking part you agree to our [Code of Conduct](CODE_OF_CONDUCT.md).
