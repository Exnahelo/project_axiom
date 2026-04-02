# Project Axiom — TODO

## How to Use This Document

Each task must result in a **concrete artifact**, not just a decision.

Every item should produce one or more of:

- a written spec block
- a diagram
- a schema
- a formal rule set

If a task does not produce an artifact, it is incomplete.

---

## Status: V0.5 Complete

`project_axiom_v_0_5.md` is the current reference architecture document. The following were delivered in V0.5 and do not need to be re-done:

- [x] Message schema (§8.4)
- [x] Escalation triggers and rules (§7.4, §8.3)
- [x] Authority matrix (§7.3)
- [x] Region input/output contracts and authority boundaries (§15)
- [x] Belief state transition model (§9.2)
- [x] Durable state rules (§9.4)
- [x] Threat model with response map (§12)
- [x] Validation service schemas for all 7 domains (§10.2)
- [x] Governance conflict resolution logic (§11.4)
- [x] Proposal–validation pattern (§16)
- [x] Routing policy examples (§14.4)
- [x] Execution walkthroughs — 3 flows (§13)
- [x] Minimal Viable Axiom definition (Appendix C)
- [x] Evaluation criteria (§22)
- [x] Implementation archetypes — 3 archetypes (§23)
- [x] Core vocabulary split into component / state / control (Appendix B)
- [x] Core invariants G1–I1 (§6)
- [x] Human Oversight Interface spec (§5.13, §11.5)
- [x] Contradiction object schema (Appendix B)

---

## Priority 1 — Schema and Protocol Specs

These unlock simulation, implementation, and publication.

- [ ] Belief object JSON schema
  - [ ] Write full schema (fields + types)
  - [ ] Define required vs optional fields
  - [ ] Provide 3–5 annotated examples
  - [ ] Define validation rules

- [ ] Contradiction object JSON schema
  - [ ] Formalize the schema defined in §13.2 into a typed spec
  - [ ] Provide 2–3 examples (type, severity, resolution status)

- [ ] Message schema JSON spec
  - [ ] Formalize the table in §8.4 into a typed JSON schema
  - [ ] Define lifecycle states (created / in-flight / acknowledged / failed)
  - [ ] Create 3–5 example messages (one per message type)

- [ ] Audit record schema
  - [ ] Define all required fields
  - [ ] Define event type taxonomy
  - [ ] Provide 3–5 examples

---

## Priority 2 — Governance and Arbitration Formalization

- [ ] Arbitration decision procedure
  - [ ] Write step-by-step logic (not just description)
  - [ ] Define inputs (conflict packet fields)
  - [ ] Define outputs (decision, confidence, trace)
  - [ ] Define authority boundaries (what it can/cannot override)
  - [ ] Define deadlock/fallback behavior
  - [ ] Produce arbitration flowchart diagram

- [ ] Governance arbitration protocol
  - [ ] Formalize the conflict resolution sequence from §11.4 into a rule set
  - [ ] Define all resolution outputs with preconditions
  - [ ] Define retry and timeout behavior

- [ ] Constitutional minimal set
  - [ ] Write the actual constitutional rules (not just categories)
  - [ ] Define what makes a rule constitutional vs policy-level
  - [ ] Define amendment procedure

- [ ] Deadlock resolution strategy
  - [ ] List concrete deadlock scenarios
  - [ ] Define resolution pathway for each
  - [ ] Define fallback to human oversight trigger conditions

---

## Priority 3 — Coordination and Routing

- [ ] Domain Coordinator interface contracts
  - [ ] Define coordinator responsibilities (formal)
  - [ ] Define allowed and forbidden actions
  - [ ] Define required methods (input/output signatures)
  - [ ] Define state structure
  - [ ] Create sequence diagram: region → coordinator → arbitration

- [ ] Routing specification
  - [ ] Formalize §14 routing policy examples into executable routing rules
  - [ ] Define routing decision algorithm
  - [ ] Define fallback routing behavior
  - [ ] Define routing audit requirements

- [ ] Cognitive cycle model
  - [ ] Choose cycle type: event-driven / phased / hybrid
  - [ ] Define full processing loop
  - [ ] Define triggers for each phase or event
  - [ ] Define timing and latency expectations
  - [ ] Create cycle diagram

---

## Priority 4 — Memory and Knowledge

- [ ] Consolidation algorithm
  - [ ] Define selection rules (what gets consolidated)
  - [ ] Define decay rules (what gets archived or pruned)
  - [ ] Define merge rules (how conflicting beliefs are handled)
  - [ ] Define consolidation cycle trigger conditions

- [ ] Snapshot isolation spec
  - [ ] Define read/write separation rules
  - [ ] Define snapshot creation triggers
  - [ ] Define rollback conditions

- [ ] Quarantine lifecycle spec
  - [ ] Define entry conditions (formal)
  - [ ] Define exit conditions (formal)
  - [ ] Define inspection rules (who can read, under what conditions)
  - [ ] Define maximum quarantine duration or review trigger

---

## Priority 5 — Diagrams and Visualization

- [ ] Unified architecture diagram
  - [ ] All 13 reference architecture components
  - [ ] All major data flows
  - [ ] Authority boundaries indicated

- [ ] Governance topology diagram
  - [ ] Constitutional layer, lens layer, preference layer
  - [ ] Interaction points with all subsystems

- [ ] Escalation flow diagram
  - [ ] Local → Domain → Global → Governance → Human
  - [ ] Trigger conditions at each level

- [ ] Belief lifecycle diagram
  - [ ] Hypothesis → Candidate → Supported / Quarantined / Rejected → Consolidated → Archived / Reopened

---

## Priority 6 — Research Extraction

- [ ] Domain-aware truth model paper outline
- [ ] Governance arbitration in modular AI paper outline
- [ ] Contradiction tolerance in cognitive architectures paper outline
- [ ] Provenance-weighted belief revision paper outline
- [ ] Layered memory consolidation for governed agents paper outline

---

## Strategic

- [x] Setup GitHub repo
- [ ] Update README for V0.5
- [x] Version documents (V0.1–V0.5 present)
- [ ] Decide IP strategy

---

## Meta

- [ ] Maintain glossary document (separate from Appendix B)
- [ ] Track open assumptions
- [ ] Track open risks
- [ ] Track version changes (changelog)

---

## Priority Focus

1. Belief object JSON schema
2. Message schema JSON spec
3. Arbitration decision procedure
4. Domain Coordinator interface contracts
5. Routing specification

These unlock:

- diagrams
- simulation
- implementation
- publication
