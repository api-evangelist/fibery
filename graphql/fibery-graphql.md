# Fibery GraphQL API

The Fibery GraphQL API provides a flexible interface for reading and mutating data in your Fibery workspace. The schema is dynamically generated from your workspace structure: every Database you create in Fibery becomes a set of GraphQL types and operations, so the exact field names and query roots depend on the spaces and databases configured in each individual workspace. This means the API is introspected at the workspace level rather than having a single static schema shared across all accounts.

The API supports querying entities with filtering, sorting, and pagination via `findXxx` query roots (e.g., `findBugs`, `findFeatures`), and mutating data through mutation roots that target a specific database (e.g., `bugs { create(...) }`, `releases { update(...) }`). Rich text fields can be read in `text`, `md`, `html`, or `jsonString` format. Background jobs are available for long-running mutations, and file attachments can be added via URL. Fragments are not supported in the current implementation.

Authentication requires a Bearer token sent in the `Authorization` header. Each Fibery Space has its own GraphQL endpoint at `https://{account}.fibery.io/api/graphql/space/{SPACE_NAME}`, while the root URL `https://{account}.fibery.io/api/graphql` lists all available space endpoints. An interactive GraphiQL IDE is served directly at each space endpoint, enabling schema exploration and query execution without additional tooling.

**Endpoint:** https://{account}.fibery.io/api/graphql/space/{SPACE_NAME}

**Documentation:** https://developers.fibery.com/guides/graphql/overview.md

**References:**

- Documentation: https://developers.fibery.com/guides/graphql/overview.md
- GettingStarted: https://developers.fibery.com/guides/getting-started/authentication.md
- Reference: https://developers.fibery.com/guides/graphql/queries.md
- Mutations: https://developers.fibery.com/guides/graphql/mutations.md
- IDE: https://developers.fibery.com/guides/graphql/using-the-ide.md
- FAQ: https://developers.fibery.com/guides/graphql/faq.md
