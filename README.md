# Railway vs Vercel: Two Platforms, One Database Question That Decides It

Companion code for the Autonoma blog post 'Railway vs Vercel: Two Platforms, One Database Question That Decides It'.

> Companion code for the Autonoma blog post: **[Railway vs Vercel: Two Platforms, One Database Question That Decides It](https://getautonoma.com/blog/railway-vs-vercel)**

## Requirements

GitHub repository with Railway-deployed services; Railway CLI access (token); Autonoma account with an API key and at least one configured test suite.

## Quickstart

```bash
git clone https://github.com/Autonoma-Tools/railway-vs-vercel.git
cd railway-vs-vercel
Copy `.github/workflows/railway-e2e.yml` into your Railway-backed repository under the same path. Set three repository secrets: `RAILWAY_TOKEN` (from railway.app/account/tokens), `RAILWAY_SERVICE_ID` (your Railway service's ID), and `AUTONOMA_API_KEY` (from your Autonoma dashboard). Push a branch and open a PR to see the workflow run.
```

## Project structure

```
.
├── .github/
│   └── workflows/
│       └── railway-e2e.yml
├── .gitignore
├── LICENSE
└── README.md
```

- `.github/workflows/` — GitHub Actions workflow that ties Railway deployments to Autonoma E2E test runs.

## About

This repository is maintained by [Autonoma](https://getautonoma.com) as reference material for the linked blog post. Autonoma builds autonomous AI agents that plan, execute, and maintain end-to-end tests directly from your codebase.

If something here is wrong, out of date, or unclear, please [open an issue](https://github.com/Autonoma-Tools/railway-vs-vercel/issues/new).

## License

Released under the [MIT License](./LICENSE) © 2026 Autonoma Labs.
