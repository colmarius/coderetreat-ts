# Coderetreat TypeScript starter

A minimal playground for short practice rounds. No exercise implementation is included.

## Prerequisites

- Node.js 24.22.2 (pinned in `.nvmrc`). With nvm, run `nvm install` and `nvm use`.
- npm (included with Node.js).

## Install and verify

```sh
npm ci
npm test          # watch mode; press q to quit
npm run test:run  # run once
npm run typecheck
```

Put TypeScript code and tests in `src/`. Vitest discovers `*.test.ts` files.

## Start fresh each round

Commit the starter once before your first round. Keep that commit as `HEAD` while
practicing; do not commit round work to it. Stop watch mode before resetting.

The following commands **discard all tracked and untracked round work in `src/`**,
restoring the starter smoke test. Copy anything you want to keep elsewhere first.
Dependencies and files outside `src/` are left alone.

```sh
git restore --source=HEAD --staged --worktree -- src
git clean -fd -- src
npm test
```
