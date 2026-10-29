# Testing

Evidence date: October 29, 2026 (America/New_York). These results come from earlier recorded runs. The five-project package refresh reviewed the receipts and original-file hashes; it did not rerun application tests, lint or builds. Tests ran in isolated private copies using existing installed dependencies; no dependency reinstall was performed. JavaScript checks used Node 24.22.1.

| Check | Result |
|---|---|
| Command routing | PASS |
| Storage recovery | PASS |
| Shutdown coordination | PASS |
| Dice parser | PASS; harness reports 48 principal syntaxes |
| Security/RPG mode | PASS |
| npm dependency audit | 0 reported vulnerabilities |

## Historical evidence

Older handoff reports were used as context, not counted as new test runs.

## Reproducibility and limits

The source is private, so these tests cannot be run from this documentation repository. The owner retains command receipts and redacted logs separately. Tests used fixtures/mocks without production credentials. No database migration, real email or Discord operation was authorized or executed.

Earlier local validation ran five selected harnesses; this is not a complete bot regression, live Discord exercise or penetration test. No coverage percentage, uptime, user count or universal rollback guarantee is claimed. JSON persistence is not a distributed database.

A dependency audit is a dated registry observation, not proof of exploitability or a security certification. No coverage percentage is claimed. [Overview](../README.md).
