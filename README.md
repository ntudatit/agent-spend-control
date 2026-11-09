# Agent Spend Control

CKB-native spending permissions and payment reconciliation for AI agents purchasing APIs and data. The first proposed milestone validates a Budget Cell on local CKB; Fiber is a later, separately validated integration.

An agent proposes a purchase. A deterministic policy engine evaluates its task budget, approved vendor and approval requirements. A minimal PolicyVault enforces delegated spending limits on-chain. The system tracks settlement and service delivery independently, including payments that succeeded but did not deliver a result.

**Status:** design and implementation plan. Application code, deployed contracts, audits and measured performance are not yet included.

## Documentation


- [Architecture and product design](architecture-design.md): system architecture, sequence diagrams, invariants, threat model and business assumptions.

## Initial scope

- Local CKB, native-CKB Budget Cell validation and one deterministic demo vendor.
- Owner-controlled task allocations with per-call and remaining-budget limits; time-based limits are deferred.
- Separate agent identity, owner, policy signer, approver and gas relayer.
- Durable reservations, idempotency, canonical settlement reconciliation and delivery receipts.
- An operator console and deterministic agent demo; optional LLM integration.

Fiber, UDT assets, standard x402 support and testnet rollout require separate compatibility checks. The broader console and multi-tenant platform are later phases. The POC does not include arbitrary trading, bridges, lending or a project token.

## Development status

The repository currently contains the product architecture. Application implementation and reproducible setup instructions will be added as development progresses.



