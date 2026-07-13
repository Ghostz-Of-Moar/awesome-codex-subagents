# PostGlobal Phase 0 — Product Intake, Discovery, and Vertical Slice

## Objective
Establish the agent-routed foundation for PostGlobal: a web-first product that lets a single user create one post and publish it to multiple supported social networks from one account, then expands into multilingual communication and audience-reach tools.

## Primary Agent
**Harbor** — decomposition, routing, dependency tracking, and consolidation.

## Supporting Agents
- **Conductor** — MVP priority and scope discipline
- **Oshoshi** — APIs, SDKs, repositories, services, vendors, and existing solution scan
- **Archaeon** — analysis of selected reference implementations
- **Architect** — system boundaries and data architecture
- **Forge** — implementation through Codex
- **Bridge** — social-network integrations and interoperability
- **Dockmaster** — environments, CI/CD, deployment, secrets, backups, and rollback
- **Ariadne** — workflow and interaction design
- **Prism** — theme system, dark/midnight modes, and skin architecture
- **Sextant** — telemetry, activation, posting-success metrics, and experiments
- **Sentinel** — authentication, token storage, abuse, and security review
- **Counsel** — privacy, platform terms, licensing, and liability review
- **Custodian** — compatibility, dependency lifecycle, migration, and SBOM
- **QA** — integration, failure-state, and release-candidate verification
- **Tuner** — performance baselines and regression gates
- **Ledger** — pricing, unit economics, and API-cost analysis
- **Advocate** — onboarding, accessibility, and support-pattern requirements
- **Envoy** — localization and multilingual publishing behavior
- **Archivist** — decisions, research, and source-of-truth maintenance
- **Launchmaster** — release readiness
- **Watchtower** — production monitoring
- **Arbiter** — executive outcome report

## Product Thesis
PostGlobal begins as a simple paid tool for publishing one post to multiple networks. Its advanced value is helping creators, artists, businesses, and influencers communicate effectively with audiences who do not share their language.

## First Vertical Slice
One user must be able to:
1. create an account;
2. connect two supported social-network accounts;
3. compose one text-first post;
4. publish immediately to both networks;
5. receive clear per-network success or failure results;
6. view a persistent posting history;
7. revoke a connected account safely.

## Explicitly Out of Scope
- team accounts
- enterprise permissions
- full campaign management
- AI translation
- scheduled posting
- analytics dashboards beyond operational success metrics
- video editing
- inbox aggregation
- social listening
- automated engagement

## Oshoshi Discovery Mission
Produce a ranked map covering:
- social-platform APIs and current publishing permissions;
- OAuth and token-management requirements;
- official SDKs and maintained wrappers;
- open-source multi-network publishing systems;
- scheduling and job-queue options;
- Supabase, managed Postgres, and alternative backend options;
- Replit deployment suitability and limitations;
- translation and localization services for later phases;
- moderation and abuse-prevention services;
- product analytics stacks;
- observability and error-reporting tools;
- licensing, lock-in, API-cost, rate-limit, and platform-policy risks.

Every recommendation must include provenance, version, license, maintenance health, compatibility, estimated adoption cost, security implications, lock-in risk, recommended disposition, receiving agent, and next action.

## Architecture Questions
- web-first React/Next.js versus another full-stack framework;
- Supabase versus custom-backend responsibilities;
- job queue and retry architecture for partial publication failures;
- encrypted token storage and rotation;
- provider-adapter interface for each social network;
- idempotency and duplicate-post prevention;
- audit logging and user-visible posting history;
- provider-specific content validation before submission;
- future mobile and desktop clients without backend fragmentation.

## Sextant Measurement Plan
Initial events:
- sign_up_started
- sign_up_completed
- provider_connect_started
- provider_connect_succeeded
- provider_connect_failed
- post_created
- publish_started
- provider_publish_succeeded
- provider_publish_failed
- multi_publish_completed
- posting_history_viewed
- provider_revoked

Initial metrics:
- signup completion rate
- first-provider connection rate
- second-provider connection rate
- time to first successful multi-post
- percentage of multi-post attempts with complete success
- partial-failure recovery rate
- seven-day return rate

## Security and Privacy Gates
- no plaintext provider tokens;
- least-privilege provider scopes;
- explicit revocation and deletion behavior;
- auditable token access;
- no silent reposting or engagement automation;
- privacy policy and terms before public launch;
- data-retention schedule;
- breach-response and provider-revocation procedure.

## Acceptance Criteria
- dedicated PostGlobal repository selected or created;
- architecture decision record approved;
- two launch providers selected based on verified API access;
- Oshoshi discovery map completed;
- security and legal blockers documented;
- MVP UX flow defined;
- telemetry taxonomy approved;
- implementation backlog divided into Codex-sized tasks;
- CI/CD and rollback plan defined;
- first vertical slice ready for implementation.

## Immediate Next Action
Create or connect a dedicated `PostGlobal` repository, then move this brief to `/docs/product/phase-0.md` and install a product-specific `AGENTS.md` that references the central Flotilla roster.
