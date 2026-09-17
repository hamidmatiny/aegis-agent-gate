# Audit log

## 2026-09-17T16:46Z — hire-day seed audit

- Inventory: 19 files, 16 Go, **6** tests.
- README gaps: approval store in-memory (Postgres URL already in compose); gRPC unimplemented; credential detection regex-only; audit emit best-effort.
- **PRIMARY inherit:** `redteam/scripts/audit_reserved_adapt_defense_in_depth.py` — content-only Adapt bypasses are NOT stoppable by tool gate; tool-path bypasses depend on catalog tier + default.yaml. First real task: run/re-home that audit's conclusions into agent-gate + policy PRs (escalate tighten vs accept residual).
- Agent identity footgun: caller-declared `agent_id` vs `service_key_fingerprint` on TOOL_GATE receipts — verify docs/tests make this obvious.
