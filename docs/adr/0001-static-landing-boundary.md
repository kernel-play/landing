---
status: accepted
recorded: 2026-10-09
kind: retrospective
source_revision: 7c9ed55aa1b3cb2d7954f37306fa37f96b24fd47
---

# Keep the landing repository a static publishing surface

The checked-in landing is a standalone HTML page with local assets and a domain declaration, with no application service or package-managed runtime in this snapshot. Its architectural boundary is static publishing rather than ownership of authenticated platform behavior. That keeps the delivery surface small but means interactive domain operations require an external application; the original selection rationale is not present.

This records the implemented choice found in the inspected source; it does not introduce a new runtime change. The original decision discussion was not recovered; rationale and trade-offs are inferred from the implementation.

## Evidence

Inspected `origin/main` at `7c9ed55aa1b3cb2d7954f37306fa37f96b24fd47`. Source links are pinned to that revision.

- [index.html](https://github.com/kernel-play/landing/blob/7c9ed55aa1b3cb2d7954f37306fa37f96b24fd47/index.html)
- [CNAME](https://github.com/kernel-play/landing/blob/7c9ed55aa1b3cb2d7954f37306fa37f96b24fd47/CNAME)
