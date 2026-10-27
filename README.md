# Node.js + TypeScript Backend Template

The starting point I use for new Express services. Nothing app-specific, just the setup I'd otherwise redo every time: TypeScript, tests, linting, formatting, logging and error handling, wired together and working.

[auth-serv](https://github.com/shahruk-maharuj/auth-serv) was built on top of it.

## What's included

- **TypeScript + Express** with `ts-node` and `nodemon` for development
- **Central error handler** that turns `http-errors` into a consistent JSON error shape
- **Winston logging**: console plus `combined.log` and `error.log`, silenced during tests
- **Config** loaded from `.env` through one `Config` object
- **Jest + Supertest** set up with `ts-jest`, plus a first integration test
- **ESLint + Prettier**, with **Husky + lint-staged** so nothing unformatted gets committed

## Use it

```bash
git clone https://github.com/shahruk-maharuj/mern-backend-template my-service
cd my-service
npm install
npm run dev
```

| Script | What it does |
|---|---|
| `npm run dev` | Start with auto-reload |
| `npm test` | Run Jest in watch mode |
| `npm run lint` / `lint:fix` | Check / fix lint errors |
| `npm run format:check` / `format:fix` | Check / fix formatting |

## Stack

TypeScript · Node.js · Express · Jest · Supertest · Winston · ESLint · Prettier · Husky
