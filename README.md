# Project Axiom

**A governance-first modular cognitive architecture for advanced AI systems.**

---

## What It Is

Project Axiom is a reference architecture that separates user interaction, domain reasoning, validation, memory mutation, and policy enforcement into distinct components with constrained write pathways. Its core claim is that advanced AI systems should be organized as governed distributed cognition rather than as a monolithic model with loosely attached tools and memory.

Governance is treated as a system control plane — not an ethics overlay or post hoc review mechanism. Epistemic state is represented as typed structured objects with provenance and lifecycle management. Memory mutation follows a proposal-validated-commit pattern rather than unconstrained writes.

---

## Key Properties

- **Governance as control plane** — enforces permissions, validation policy, escalation, and fault containment
- **Typed epistemic state** — belief objects with provenance, confidence, uncertainty type, and validation status
- **Proposal-validated-commit writes** — no unconstrained durable state mutation
- **Domain-sensitive validation** — 7 epistemic domains with distinct evidentiary standards and validator services
- **Fault containment** — subsystem isolation, quarantine, rollback, and degraded operation modes
- **Auditable by design** — immutable audit records for all durable state mutations and high-risk actions
- **Modular specialization** — domain-specialized Cognitive Regions with defined authority limits

---

## Current Version

**V0.5** — Structural rewrite with reference architecture, authority matrix, execution walkthroughs, evaluation criteria, and formal invariants.

See [`project_axiom_v_0_5.md`](project_axiom_v_0_5.md) for the full specification.

---

## Document History

| Version | Description |
|---|---|
| V0.1 | Initial architecture sketch |
| V0.2 | Expanded modular cognition framing |
| V0.3 | Domain model, generator-governor pattern, memory architecture |
| V0.4 | Correction pass: distributed coordination, domain-scoped uncertainty, threat model |
| V0.5 | Structural rewrite: reference architecture, authority matrix, invariants, walkthroughs, evaluation criteria |

---

## V0.5 Contents at a Glance

1. Executive Summary
2. Mission and Design Scope
3. System Model at a Glance
4. Document Scope
5. Reference Architecture (13 components with Role / Inputs / Outputs / Authority limits)
6. Core Invariants (G1–I1)
7. Authority and Permissions (Authority Matrix)
8. Coordination Model (3-level routing + message schema)
9. Knowledge and Memory Model (belief lifecycle, 8 memory layers, durable state rules)
10. Domain Validation Model (7 domains, validator service schemas)
11. Governance and Control Plane (constitution, lenses, preferences, human oversight)
12. Threat Model, Fault Containment, and Recovery
13. Execution Walkthroughs (standard query, contradiction, mutation proposal)
14. Routing Policy: Region × Domain × Priority
15. Cognitive Region Architecture (10 regions with standard schema)
16. Proposal–Validation Pattern
17. Trust and Reliability Model
18. Inter-Module Communication Model
19. Controlled Adaptation and Learning
20. Design Horizon and Scope Boundaries
21. Open Research Questions
22. Evaluation Criteria
23. Implementation Archetypes (3 archetypes)
24. Roadmap
25. Conclusion
- Appendix A: Design Rationale
- Appendix B: Core Vocabulary (component / state / control)
- Appendix C: Minimal Viable Axiom
- Appendix D: Version History

---

## Status

This is a reference architecture specification, not a production system. Some subsystems can be prototyped with current technology; others require advances in distributed inference and coordination infrastructure. The document distinguishes these cases explicitly.

---

## Next Steps

See [`todo.md`](todo.md) for the current work plan. Priority items:

1. Belief object JSON schema
2. Message schema JSON spec
3. Arbitration decision procedure
4. Domain Coordinator interface contracts
5. Routing specification

---

## License

See [`LICENSE`](LICENSE).
