# Distribution Hub Web

React frontend for Distribution Hub, maintained separately from the FastAPI API.

## Current status

The frontend is an initial scaffold. It currently renders a landing screen and does not consume commercial endpoints, provide business routes, authentication, customer screens, or a functional API integration.

The backend and product domain are documented in the [API repository](https://github.com/lc-curto/distribution-hub-api):

- [Architecture](https://github.com/lc-curto/distribution-hub-api/blob/main/docs/ARCHITECTURE.md)
- [Domain and product](https://github.com/lc-curto/distribution-hub-api/blob/main/docs/DOMAIN.md)
- [Data model](https://github.com/lc-curto/distribution-hub-api/blob/main/docs/DATA_MODEL.md)
- [API runbook](https://github.com/lc-curto/distribution-hub-api/blob/main/docs/RUNBOOK.md)

## Technologies

- Node.js 22 in CI;
- pnpm 9.15.0 in CI;
- React 18;
- TypeScript;
- Vite;
- React Router;
- TanStack React Query;
- Vitest.

## Requirements

- Node.js 22;
- pnpm 9 or a version compatible with lockfile version 9.

## Configuration and development

```bash
pnpm install
cp .env.example .env
pnpm dev
```

The only currently available variable is:

```text
VITE_API_URL=http://localhost:8000
```

It represents the planned API address, but the current scaffold does not use it yet.

## Validation

```bash
pnpm build
pnpm test
```

The CI workflow runs `pnpm install --frozen-lockfile` and `pnpm build`. A test script exists, but no frontend tests are currently implemented and CI does not run `pnpm test` yet.

## Current structure

```text
src/main.tsx       entrypoint and initial component
src/app/           reserved for application code
src/assets/        reserved for assets
src/hooks/         reserved for hooks
src/layouts/       reserved for layouts
src/store/         reserved for state
src/styles/        reserved for styles
src/test/          reserved for tests
src/types/         reserved for types
src/utils/         reserved for utilities
```

Reserved directories do not prove that features are implemented.
