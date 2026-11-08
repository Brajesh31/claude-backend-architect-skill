# claude-backend-architect-skill

A Claude Code skill for designing scalable, secure, resilient, and maintainable backend systems and APIs.

## Overview

This skill supports backend architecture decisions across service boundaries, API contracts, data ownership, distributed communication, resilience, and operations. It is intended for system design and architecture work rather than isolated code fixes.

## Main Capabilities

- Define service boundaries and responsibilities.
- Design REST and other API contracts.
- Select synchronous and asynchronous communication patterns.
- Model data ownership and persistence.
- Plan scaling and capacity.
- Apply resilience patterns.
- Design authentication and authorization boundaries.
- Improve observability and operational readiness.
- Plan safe deployment and migration strategies.

## Architecture Areas

### Service Boundaries

Define cohesive services around business responsibilities. Avoid splitting a system into services when the deployment and ownership overhead outweighs the benefit.

### API Contracts

Specify request and response schemas, error formats, pagination, versioning, and compatibility expectations.

### Distributed Systems

Consider timeouts, retries, idempotency, message delivery, consistency, and partial failures.

### Data Architecture

Define ownership, transaction boundaries, query patterns, indexing, and migration requirements.

### Resilience and Operations

Plan health checks, metrics, logs, tracing, alerting, capacity, backups, and recovery.

## Installation

```bash
git clone https://github.com/Brajesh31/claude-backend-architect-skill.git ~/.claude/skills/backend-architect
```

## Usage

Invoke the skill for backend architecture planning or review:

```text
/backend-architect
```

Provide the product domain, expected traffic, data model, deployment environment, security requirements, and current architecture constraints.

## Recommended Workflow

1. Capture functional and non-functional requirements.
2. Map users, system boundaries, and external dependencies.
3. Define data ownership and API contracts.
4. Select architecture and communication patterns.
5. Identify failure modes and security boundaries.
6. Plan observability and operational support.
7. Design rollout, migration, and rollback steps.
8. Validate the design against representative workloads.

## Design Checklist

- Service responsibilities are clear.
- APIs have stable contracts.
- Data ownership is explicit.
- Authentication and authorization are enforced.
- Timeouts and retries are bounded.
- Operations are observable.
- Capacity and cost assumptions are documented.
- Deployments can be rolled back safely.
- Complexity is justified by the requirements.

## Repository Contents

- `SKILL.md`: Main backend architecture instructions.
- `README.md`: Architecture workflow and review checklist.

## Practical Guidance

A modular monolith is often a better starting point than microservices. Split services only when independent scaling, deployment, team ownership, or failure isolation provide a concrete advantage.
