# Starting backlog — day one

- PRIMARY inherit: redteam/scripts/audit_reserved_adapt_defense_in_depth.py — classify which Adapt bypasses would be stopped by agent-gate risk tiers vs content-only (no tool). Produce actionable gate/policy tightening proposals as PRs (not merges).
- Known gaps from README: approval store still in-memory (Postgres DATABASE_URL already in compose); gRPC unimplemented; credential detection regex-only.
- Agent identity: caller-declared agent_id vs service_key_fingerprint — audit whether receipts + docs make this footgun impossible to miss.
