# ACID (acid)

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
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

ACID (Atomicity, Consistency, Isolation, Durability) is a set of properties that guarantee database transactions are processed reliably even in the face of errors, power failures, or system crashes. These four properties ensure that data remains accurate and consistent, making ACID compliance a fundamental requirement for relational databases, distributed systems, and financial APIs.

**URL:** [Visit APIs.json](https://raw.githubusercontent.com/api-evangelist/acid/refs/heads/main/apis.yml)

**Run:** [Capabilities Using Naftiko](https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=company-api-evangelist&utm_content=repo)

## Tags:

 - ACID, Database, Transactions, Atomicity, Consistency, Isolation, Durability, Distributed Systems

## Timestamps

- **Created:** 2025-01-01
- **Modified:** 2026-04-19

## APIs

### PostgreSQL Transaction API
PostgreSQL provides full ACID compliance through its transaction management system including BEGIN, COMMIT, ROLLBACK, SAVEPOINT, and isolation level controls. PostgreSQL uses Multi-Version Concurrency Control (MVCC) to provide high concurrency while maintaining strong data consistency guarantees.

**Human URL:** [https://www.postgresql.org/docs/current/transaction-iso.html](https://www.postgresql.org/docs/current/transaction-iso.html)

#### Tags:

 - PostgreSQL, RDBMS, MVCC, ACID, SQL

#### Properties

- [Documentation](https://www.postgresql.org/docs/current/transaction-iso.html)
- [PostgreSQL BEGIN Transaction](https://www.postgresql.org/docs/current/sql-begin.html)
- [GitHubRepository](https://github.com/postgres/postgres)

### CockroachDB Distributed SQL API
CockroachDB is a distributed SQL database providing serializable ACID transactions across multiple nodes and regions. It uses the Raft consensus algorithm and supports the PostgreSQL wire protocol.

**Human URL:** [https://www.cockroachlabs.com/docs/stable/](https://www.cockroachlabs.com/docs/stable/)

#### Tags:

 - CockroachDB, Distributed SQL, ACID, Serializable, Cloud Native

#### Properties

- [Documentation](https://www.cockroachlabs.com/docs/stable/)
- [CockroachDB Transactions](https://www.cockroachlabs.com/docs/stable/transactions.html)
- [GitHubRepository](https://github.com/cockroachdb/cockroach)

### Google Spanner API
Google Spanner is a globally distributed, externally consistent database providing ACID transactions at global scale using TrueTime clock synchronization. The Cloud Spanner API offers both read-write and read-only transactions via REST and gRPC.

**Human URL:** [https://cloud.google.com/spanner/docs/transactions](https://cloud.google.com/spanner/docs/transactions)

#### Tags:

 - Google Spanner, Distributed Database, Global Scale, ACID, TrueTime

#### Properties

- [Documentation](https://cloud.google.com/spanner/docs/transactions)
- [APIReference](https://cloud.google.com/spanner/docs/reference/rest)
- [OpenAPI](https://raw.githubusercontent.com/APIs-guru/openapi-directory/main/APIs/googleapis.com/spanner/v1/openapi.yaml)

### Amazon Aurora Transactions API
Amazon Aurora provides ACID-compliant transactions for MySQL and PostgreSQL-compatible editions with distributed storage across 3 AZs with 6-way replication. The Aurora Data API enables HTTP-based serverless SQL transactions.

**Human URL:** [https://docs.aws.amazon.com/AmazonRDS/latest/AuroraUserGuide/Aurora.Overview.html](https://docs.aws.amazon.com/AmazonRDS/latest/AuroraUserGuide/Aurora.Overview.html)

#### Tags:

 - AWS Aurora, MySQL, PostgreSQL, ACID, Serverless

#### Properties

- [Documentation](https://docs.aws.amazon.com/AmazonRDS/latest/AuroraUserGuide/Aurora.Overview.html)
- [Aurora Data API Reference](https://docs.aws.amazon.com/rdsdataservice/latest/APIReference/)

### Atomikos Transaction API
Atomikos provides ACID transaction management middleware for distributed microservices, supporting XA transactions across REST services using the Try-Confirm/Cancel (TCC) pattern.

**Human URL:** [https://www.atomikos.com/](https://www.atomikos.com/)

#### Tags:

 - Atomikos, Distributed Transactions, TCC Pattern, Microservices, XA

#### Properties

- [Documentation](https://www.atomikos.com/)
- [ACID Transactions Across Microservices](https://www.atomikos.com/Blog/ACIDTransactionsAcrossMicroservices)

## Common Properties

- [ACID Wikipedia Reference](https://en.wikipedia.org/wiki/ACID)
- [CockroachDB Open Source Repository](https://github.com/cockroachdb/cockroach)
- [ACID JSON-LD Context](json-ld/acid-context.jsonld)
- [ACID Vocabulary](vocabulary/acid-vocabulary.yaml)

## Features

| Name | Description |
|------|-------------|
| Atomicity | Transactions are all-or-nothing: either all operations in a transaction succeed and are committed, or none are applied and the database is rolled back to its prior state. |
| Consistency | A transaction brings the database from one valid, consistent state to another, enforcing all defined constraints, triggers, and cascades. |
| Isolation | Concurrent transactions execute as if they were serialized, preventing interference. Isolation levels control the degree of visibility between concurrent transactions. |
| Durability | Once a transaction is committed, it remains committed even in the event of system crashes, power failures, or other errors. |
| Distributed ACID | Modern distributed databases extend ACID guarantees across multiple nodes, regions, and data centers using consensus algorithms (Raft, Paxos) and synchronized clocks. |
| REST API Transaction Patterns | Design patterns for ACID-like guarantees in REST APIs include Two-Phase Commit (2PC), Try-Confirm/Cancel (TCC), and Saga patterns for managing distributed transactions. |

## Use Cases

| Name | Description |
|------|-------------|
| Financial Transactions | Banking and payment systems require ACID compliance to ensure monetary transfers are atomic and durable across system failures. |
| Inventory Management | E-commerce systems use ACID transactions to prevent overselling by ensuring inventory decrements and order creation are atomic. |
| Distributed Microservices Coordination | Microservices architectures use Saga and TCC patterns to achieve eventual consistency with compensating transactions. |
| Multi-Region Database Replication | Global applications use databases like Google Spanner and CockroachDB to maintain ACID consistency across geographic regions. |
| Idempotent API Design | REST APIs use database transactions to implement idempotency keys, ensuring duplicate requests produce the same result. |

## Integrations

| Name | Description |
|------|-------------|
| PostgreSQL | The most widely deployed open-source RDBMS with full ACID compliance via MVCC and configurable transaction isolation levels. |
| MySQL / MariaDB | Popular open-source databases providing ACID compliance through the InnoDB storage engine with row-level locking and MVCC. |
| MongoDB Multi-Document Transactions | MongoDB added multi-document ACID transactions in version 4.0, extending its document model with ACID guarantees. |
| Apache Kafka Transactions | Kafka's transactional API enables exactly-once semantics with atomic writes to multiple partitions. |
| Saga Pattern / Orchestration | The Saga pattern decomposes long-running transactions into local transactions with compensating actions for distributed consistency. |

## Artifacts

Machine-readable API specifications organized by format.

### JSON Schema

- [ACID Transaction Schema](json-schema/acid-transaction-schema.json)
- [ACID Saga Step Schema](json-schema/acid-saga-step-schema.json)

### JSON Structure

- [ACID Transaction Structure](json-structure/acid-transaction-structure.json)
- [ACID Saga Step Structure](json-structure/acid-saga-step-structure.json)

### JSON-LD

- [ACID Context](json-ld/acid-context.jsonld)

### Examples

- [ACID Transaction Example](examples/acid-transaction-example.json)
- [ACID Saga Step Example](examples/acid-saga-step-example.json)

## Vocabulary

- [ACID Vocabulary](vocabulary/acid-vocabulary.yaml) — Unified taxonomy mapping 6 resources, 7 actions, 2 workflows, and 5 personas across the ACID database transaction landscape

## Maintainers

**FN:** Kin Lane

**Email:** kin@apievangelist.com
