# Maily

Maily is a self-hosted, multi-user webmail application built as a TypeScript monorepo.

The project is currently in its foundation phase. The React frontend, NestJS API, background
worker, authentication and mail services will be introduced in separate, reviewable changes.

## Requirements

- Node.js 24.11.0
- pnpm 9.15.2 managed through Corepack

On Windows, use `pnpm.cmd` when PowerShell execution policy blocks the `pnpm.ps1` shim.

## Workspace

The workspace will contain applications under `apps/*` and shared packages under `packages/*`.
The root package controls common formatting, linting, type checking, tests and builds.

## Commands

- `pnpm install` installs all workspace dependencies.
- `pnpm run dev` starts development scripts exposed by workspace applications.
- `pnpm run build` builds all workspace applications.
- `pnpm run lint` checks source files with ESLint.
- `pnpm run typecheck` checks TypeScript project references and workspace packages.
- `pnpm run test` runs package test suites.
- `pnpm run test:e2e` runs end-to-end test suites.
- `pnpm run format:check` verifies formatting without changing files.
- `pnpm run format` formats supported files.

## Status

Maily is not ready for production use. The first milestone establishes a reproducible monorepo;
application features will be added incrementally.
