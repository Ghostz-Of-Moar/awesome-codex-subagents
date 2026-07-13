# Codex Assignment Instructions

Codex is the implementation engine for the Flotilla Agent System.

## Required Task Header

```text
PRIMARY AGENT:
SUPPORTING AGENTS:
PRODUCT:
REPOSITORY:
BRANCH:
OBJECTIVE:
REFERENCE SYSTEM AND VERSION:
LICENSE AND PROVENANCE:
ACCEPTANCE CRITERIA:
REQUIRED TESTS:
SECURITY/PRIVACY REVIEW:
COMPATIBILITY REVIEW:
```

Use `REFERENCE SYSTEM AND VERSION` and `LICENSE AND PROVENANCE` whenever existing or third-party code is involved.

## Routing Rules
- Harbor decomposes and routes work.
- Arbiter receives final summaries and unresolved decisions.
- Archaeon owns analysis, architecture extraction, algorithm extraction, refactoring plans, modernization plans, porting analysis, and independent reconstruction of existing codebases.
- Forge implements approved work.
- Architect reviews structural changes in the new system.
- Ariadne owns Figma and product interaction systems.
- Prism owns themes and visual identity.
- Daedalus owns mathematics, DSP, and procedural systems; extracted mathematical models pass through Archaeon before Daedalus extends them.
- Anansi owns motif memory, narrative continuity, and cultural context.
- Envoy owns localization and publishing.
- Ledger owns pricing and unit economics.
- Bridge owns integrations and interoperability.
- Archivist owns documentation and source-of-truth maintenance.
- Advocate owns user research and accessibility evidence.
- QA verifies behavior; Tuner verifies performance; Sentinel verifies security; Counsel verifies policy and licensing; Custodian verifies compatibility.
- Launchmaster coordinates release; Watchtower monitors production.

## Mandatory Archaeon Rule

Before Codex adopts ideas, implementation patterns, mathematics, UI behavior, architecture, or source material from another codebase, it must read `archaeon.md` and produce an Archaeon analysis.

The analysis must distinguish:

1. general ideas and principles;
2. implementation choices;
3. legally reusable material and obligations;
4. protected, private, incompatible, or unsuitable expression that must not be copied.

When reuse permissions are uncertain, stop reuse and route the question to Counsel. Analysis may continue, but copied implementation must not.

Read `AGENTS_INDEX.md` and the primary agent's file before beginning work.