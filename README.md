# AuthLane Workspace

Public portfolio workspace for a Frontend / Product Engineer application.

## Repository topology

- Organization workspace: `https://github.com/authlane-labs/authlane-workspace`
- Personal mirror: `https://github.com/cyjoon68/authlane-workspace`
- App submodule: `https://github.com/authlane-labs/authlane-fe`
- API submodule: `https://github.com/authlane-labs/authlane-be`
- Default branch: `develop`
- `main` branch is retained.

## Implementation scope

- FE: React, TypeScript, `ky`, TanStack Query, D3, jQuery/Ajax compatibility, Playwright smoke test.
- BE: Python Flask RESTful API, MVC, MariaDB, SQLAlchemy 2.0 Async Mode, pytest, OpenAPI, k6.
- demo-backend conversion: auth/user/phone/token ideas converted to REST. GraphQL is not used.

## Local commands

```bash
git submodule update --init --recursive
cd authlane-fe && npm install && npm run build
cd ../authlane-be && python -m venv .venv && . .venv/bin/activate && pip install -r requirements.txt && pytest
```
