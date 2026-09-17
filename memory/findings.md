# Findings

Append-only. Cite file paths and PR URLs.

- **2026-09-17**: Landed policy fix for reserved Adapt audit in PR #42 (`https://github.com/hamidmatiny/aegis/pull/42`), escalating `http_get` to block unauthorized data exfiltration.
- **2026-09-17**: Experimental redteam audit script (`redteam/scripts/audit_reserved_adapt_defense_in_depth.py`) added with CLI `--input` support and soft-fail handling when bypass JSONL is missing.
- **2026-09-17**: Remaining security gaps identified in agent-gate / policy engine: `write_file` (HIGH severity) and `send_email`, `post_message`, `corp_http_get` (MEDIUM severity) remain default-allow except where explicitly governed by named rules.

- **2026-09-17**: PR https://github.com/hamidmatiny/aegis/pull/66 opened (script CLI soft-fail + redteam/docs/adapt-defense-in-depth-closeout.md citing #42).
