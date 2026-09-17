# Redteam Closeout: Reserved Adapt Defense

This closes the experimental redteam campaign for the "reserved Adapt" defense-in-depth policy.

- **Status**: Campaign complete.
- **Outcome**: Successfully landed policy enforcement in PR #42 (`https://github.com/hamidmatiny/aegis/pull/42`) for `http_get` escalation.
- **Scripting**: The experimental audit script (`redteam/scripts/audit_reserved_adapt_defense_in_depth.py`) has been added for future regression testing, configured to soft-fail gracefully if input bypass datasets are not present.
- **Remaining Gaps**: `write_file` (HIGH severity) and `send_email`, `post_message`, `corp_http_get` (MEDIUM severity) need continued oversight and policy-as-code hardening.
