# SHARIAGUARD

Scholar-Led, AI-Screened, and Blockchain-Enforced Shariah Compliance for Every Akad in Islamic Fintech.

## Prototype

This repository currently contains a single-file browser prototype in `index.html`.

### Interactive flow

1. **Overview** — 3-layer SHARIAGUARD architecture.
2. **Akad Screening** — edit an akad draft and run deterministic local screening rules.
3. **DPS Review** — approve or reject flagged clauses.
4. **Smart Contract** — generate a SHA-256 contract hash and simulate permissioned-ledger commit.
5. **Audit Dashboard** — inspect the local audit event log and search events.
6. **Fatwa Knowledge** — inspect the prototype's structured DSN-MUI references.

### Local browser data

The prototype is intentionally designed to run without an external backend or API key. Application state is held in the browser runtime and can be extended to `localStorage`/IndexedDB for persistence.

> **Important:** the screening engine and ledger are prototype simulations. They are not a production Shariah ruling engine or a live Hyperledger deployment. Final Shariah authority remains with qualified scholars/DPS.

## Run

Open `index.html` directly in a modern browser, or serve the repository with any static HTTP server.

## Competition demo

Recommended demonstration:

`Overview → Akad Screening → DPS Review → Smart Contract → Audit Dashboard`

Use the demo Mudharabah contract to show a flagged late-payment-income clause, DPS approval, hash generation, ledger commit, and resulting audit trail.
