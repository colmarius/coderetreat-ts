# Scope

Keep this repository a minimal TypeScript + Vitest Coderetreat starter using npm
and its committed lockfile. Exercise code and tests belong in `src/`.
Do not add an exercise solution, framework, UI, coverage tooling, lint stack,
or release automation unless explicitly requested.

# Verification

- `npm ci` installs the locked dependencies.
- `npm run test:run` runs tests once; `npm test` starts watch mode.
- `npm run typecheck` checks all TypeScript code and tests in strict mode.
- When changing the test setup, temporarily break a smoke-test expectation,
  confirm the test command exits nonzero, restore it, and rerun verification.
