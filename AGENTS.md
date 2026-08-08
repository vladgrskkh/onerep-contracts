# onerep-contracts

OpenAPI specifications for OneRep services — the single source of truth for API contracts.

## Structure
```
auth/v1/openapi.yaml    # Auth service API
gym/v1/openapi.yaml     # Gym API service
```

## Usage
- Backend services implement against these specs
- Frontend client can be generated from these specs
- Use as reference for integration tests

## CI
OpenAPI spec validation on push/PR via swagger-cli.

## Adding new endpoints
1. Update the relevant openapi.yaml
2. Run validation: `npx @apidevtools/swagger-cli validate **/*.yaml`
3. PR review by both backend and frontend teams
