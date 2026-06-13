# Fibery

Fibery is a connected work management platform with a REST API and GraphQL API for managing entities, databases, automation rules, collaborative documents, and custom workflow views. It supports webhooks, file uploads, rich text operations, real-time change subscriptions, and a paginated change history log for building integrations and automating workflows.

## APIs

- **HTTP API** — Command-based REST API. All operations are POSTed to `/api/commands` as batched command arrays. Covers schema management, entity CRUD, views, files, webhooks, and history.
- **GraphQL API** — Full GraphQL interface with an interactive IDE, supporting queries, mutations, filtering, pagination, and nested entity operations.
- **MCP Server** — Model Context Protocol server (`fibery-mcp-server`) enabling AI assistants (including Claude) to explore workspace schema, query databases, and create/update entities.

## Authentication

Token-based authentication via `Authorization: Token YOUR_TOKEN` header. Tokens are generated per workspace user inside Fibery settings.

## Developer Resources

- Developer Docs: https://developers.fibery.com
- HTTP API Overview: https://developers.fibery.com/guides/http-api/overview
- GraphQL API: https://developers.fibery.com/guides/graphql-api/overview
- OpenAPI Spec: https://developers.fibery.com/api-reference/openapi.json
- GitHub Org: https://github.com/Fibery-inc
- Status Page: https://status.fibery.io
- Blog: https://fibery.com/blog/
- Pricing: https://fibery.com/pricing

## Pricing

| Plan       | Price (USD/user/month, annual) | Notes                                      |
|------------|--------------------------------|--------------------------------------------|
| Free       | $0                             | Up to 10 users, 10 databases, 1 GB storage |
| Standard   | $12                            | Unlimited databases, AI included           |
| Pro        | $20                            | JS automations, advanced permissions       |
| Enterprise | $40                            | Min 25 seats, SAML SSO, SCIM, unlimited automations |

Special discounts: 50% for non-profits/education, 100% for open-source, 6 months free (Pro) for startups.

## Catalog Files

- `apis.yml` — APIs.json 0.19 provider profile
- `plans/fibery-plans-pricing.yml` — Detailed pricing plan breakdown
- `rate-limits/fibery-rate-limits.yml` — API rate limit and pagination constraints
- `finops/fibery-finops.yml` — FinOps cost management guidance
