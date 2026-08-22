# Fibery

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **Not from the company, and here with a question?** You are welcome here — we would rather be the
> front line and point you the right way than have a good report go nowhere. What this repository
> can answer is narrow, though, so it is worth knowing who you are actually looking for:
>
> - **A question about how the API works, an account, billing, or a bug in the service** — that is
>   the company's own support, not us. We profile this API; we do not operate it and cannot see
>   your account.
> - **A bug in an open-source project we only catalog** — file it on that project's own repository.
>   This has happened with a real and correct bug report that reached us instead of the people who
>   could fix it, which helped nobody.
> - **Anything about this listing itself** — the description, the tags, the rating, a missing or
>   wrong artifact — is ours. Open an issue here.
> - **Not sure, or something general about API Evangelist or APIs.io** — open an issue on the
>   [APIs.io Inbox](https://github.com/api-search/inbox) and we will route it.
>
> **This repository contains no software, and we will never ask you to download anything.** There is
> no build, release, installer, or binary here — only text and machine-readable API descriptions, so
> there is nothing here that can be "corrupt" or need "repairing". Any issue, comment, or email
> claiming otherwise and offering a download link is not from us and is hostile. Do not follow the
> link; it is a lure. Report it to GitHub and, if you like, tell us at
> [info@apievangelist.com](mailto:info@apievangelist.com) so we can take it down.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

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
