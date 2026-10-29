# Architecture

Discord events enter a shared composition layer and are routed to domain modules. Storage helpers maintain recoverable JSON state. The local Control Center observes and manages the runtime through restricted local interfaces. The main entrypoint still contains substantial legacy composition; modularization is incremental.

```text
Discord events → routing and authorization → domain modules → recoverable JSON state
Local Control Center → restricted operations → runtime observation and recovery
```

## Design rationale

Recoverable file writes and controlled shutdown address interrupted operations. Explicit permissions separate a visible UI action from authority to perform it. A parser evaluates bounded dice expressions instead of executing user-supplied JavaScript.

## Boundaries

Earlier local validation ran five selected harnesses; this is not a complete bot regression, live Discord exercise or penetration test. No coverage percentage, uptime, user count or universal rollback guarantee is claimed. JSON persistence is not a distributed database.

The diagram is an explanatory abstraction of inspected source, not a deployment topology or operational runbook. [Overview](../README.md).
