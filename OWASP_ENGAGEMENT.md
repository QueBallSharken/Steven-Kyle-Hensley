# OWASP Engagement & Research Provenance

Steven Kyle Hensley
QueBallSharken / Stevil

Status: Public research and attribution record
Purpose: Preserve the documented relationship between my OWASP discussions, technical contributions, collaborations, and subsequent research.

---

## 1. PURPOSE

This document preserves the public research lineage of Steven Kyle Hensley
(QueBallSharken / Stevil) across discussions in the OWASP Top 10 for Large
Language Model Applications project.

It is intended to help collaborators, sponsors, researchers, reviewers,
and future maintainers distinguish:

- Direct contributions
- Collaborative development
- Technical ideas introduced during discussion
- Later research derived from those discussions
- Verified evidence
- Evidence that still requires direct archival verification

This document is a provenance record.

It is not intended to claim ownership of ideas that were developed
collaboratively.

Where another contributor materially participated in the development of
an idea, that collaboration is explicitly identified.

---

## 2. PREFERRED ATTRIBUTION

Preferred name:

Steven Kyle Hensley

Known public identifiers:

- Steven Kyle Hensley
- Steven K. Hensley
- Steven Hensley
- QueBallSharken
- Stevil

GitHub:

QueBallSharken

Repository:

Steven-Kyle-Hensley

When attribution is possible, use:

Steven Kyle Hensley

---

## 3. OWASP RESEARCH CONTEXT

My participation in OWASP discussions became part of a broader investigation
into a recurring problem:

A system may successfully authenticate an actor, authorize an action,
validate policy, transmit state, and record execution while still failing
to preserve the governing condition that made the action legitimate.

This led to a progressively narrower research question:

Can authority be safely propagated?

Then:

Can authority be re-derived at every execution boundary?

Then:

Can the governing invariant itself survive every mutation-capable boundary?

The final formulation became:

Can a governing invariant survive every mutation-capable boundary until
the irreversible mutation authority?

This question became the basis for:

Boundary-to-Boundary Invariant Survival (BBIS).

---

# 4. OWASP ENGAGEMENT INDEX

The following index records the OWASP issues currently identified as
relevant to this research lineage.

The list is intentionally conservative.

Where direct evidence has not yet been independently archived or retrieved,
the item is marked accordingly rather than presented as verified fact.

---

## ISSUE #800

Topic:

Independent authorization-layer framework mapping against ASI02, ASI03,
and ASI05.

Primary period:

February 19–26, 2026

Role:

Commenter / collaborative contributor

Primary collaborator:

Richard Porter (@richard-porter)

Research significance:

Issue #800 became an important point in the development of the distinction
between delegated scope and locally derived authority.

The discussion examined whether authority should be treated primarily as
something propagated through a delegation chain or something that must be
re-established at each execution boundary.

### Authority Collapse Mode

One of the concepts developed during this exchange was:

Authority Collapse Mode.

The central proposition was:

Authority does not automatically survive delegation.

Instead, authority must be re-derived from canonical state at the boundary
where execution is about to occur.

If the required authority cannot be independently derived:

authority = 0

Non-derivation is therefore not merely an exception condition.

It is a loss of authority.

### Canonical Boundary Inputs

The proposed re-derivation model identified inputs such as:

1. Identity binding
2. Canonical policy state
3. Policy hash
4. Admissibility state
5. Tool constraints
6. Override scope

The important architectural distinction was between:

delegation history

and

current authoritative state.

A downstream execution boundary should not blindly inherit authority from
an upstream agent.

It should determine whether authority still exists.

### Collaboration

The discussion with Richard Porter explored the relationship between:

- Delegation Grammar
- Chain of Custody
- Scope Decay
- Authority Collapse
- Boundary recomputation

This exchange helped clarify that delegation semantics and execution
authority are related but not identical properties.

### Attribution

During the discussion, I requested attribution using my full name:

Steven Hensley

This was intended to reduce ambiguity between my GitHub identity,
aliases, and future archival references.

### Evidence

Primary source:

OWASP Top 10 for LLM Applications
Issue #800

Repository:

www-project-top-10-for-large-language-model-applications

Issue:

#800

---

# 5. ISSUE #702

Topic:

Arrow clarification in the Securing Agentic Applications Guide 1.0.

Date of engagement:

March 28, 2026

Role:

Commenter

Research significance:

This discussion contributed to the distinction between architecture
topology and execution-time admissibility.

The relevant question was not simply whether a topology such as a tree
or diamond correctly represented information flow.

The deeper question was:

What happens at the downstream boundary immediately before execution?

A topology can describe propagation.

It does not automatically prove that the resulting state remains
admissible at the moment of action.

This reinforced a recurring principle in my research:

Propagation analysis must eventually terminate at an enforceable
execution boundary.

### Research connection

This discussion helped connect:

- Multi-agent topology
- State propagation
- Contamination analysis
- Convergence
- Execution boundaries
- Admissibility

to the broader execution-governance problem.

### Evidence

Primary source:

OWASP Top 10 for LLM Applications
Issue #702

---

# 6. ISSUE #802

Topic:

Runtime Enforcement Mapping for the OWASP Agentic Top 10.

Research relevance:

Issue #802 falls within the period in which execution-time enforcement,
signed execution artifacts, proxy boundaries, and authorization integrity
were being examined across agentic execution systems.

The discussion is relevant to the development of a broader distinction:

Authorization must not merely exist somewhere in the chain.

The system must establish where authorization is enforced and what prevents
an invalid state from reaching the irreversible execution point.

This distinction later became increasingly important to the BBIS formulation.

### Research connection

Relevant concepts include:

- Runtime enforcement
- Execution tickets
- Authorization-at-execution
- Proxy boundaries
- Atomicity
- Mutation authority
- Commit-point enforcement

Issue #802 should therefore be treated as contextual research evidence
rather than automatically attributed as a standalone invention.

---

# 7. ISSUES #803, #810, AND #812

These issues are important to the surrounding research timeline.

However, the current public evidence collected for this repository does
not yet provide sufficient direct archival material to make strong
individual attribution claims for every comment.

Therefore:

## Issue #803

Status:

Requires direct verification.

Current classification:

Contextual OWASP engagement.

---

## Issue #810

Status:

Requires direct verification of the individual comment history.

Current classification:

Relevant contextual engagement.

Some external or cross-repository references place #810 within the broader
agent-governance discussion during the period of this research.

However, this repository should not treat a search-index reference as
equivalent to a verified primary-source comment transcript.

---

## Issue #812

Status:

Requires direct verification of the individual comment history.

Current classification:

Contextual engagement requiring archival verification.

The issue falls within the period immediately preceding the formal BBIS
proposal and is relevant to discussions concerning:

- Admissibility
- Mutation boundaries
- Commit points
- Execution enforcement
- Anti-interleaving concerns
- Governance conditions across agent pipelines

These relationships are documented as research context rather than
presented as proven authorship claims until the primary comments are
archived.

---

# 8. ISSUE #817

Topic:

Proposal: Boundary-to-Boundary Invariant Survival for Agentic Execution
Governance.

Date:

April 6–8, 2026

Author:

QueBallSharken

Preferred attribution:

Steven Kyle Hensley

Collaborator:

Bradley Bates (@Bradsadevnow)

Research significance:

Issue #817 represents the point where the earlier execution-boundary
questions were formalized into a distinct governance property.

---

## 9. BOUNDARY-TO-BOUNDARY INVARIANT SURVIVAL

BBIS asks whether a governing invariant remains alive across every
mutation-capable boundary between authorization and irreversible execution.

The central distinction is:

A record saying that an invariant was checked is not the same as an
invariant that remains capable of refusing execution.

Therefore:

Historical approval != live governance.

A system is only protected if the governing condition remains enforceable
until the point where the mutation becomes irreversible.

---

# 10. LIVE REFUSAL CONDITION

The BBIS formulation requires the invariant to remain a:

LIVE REFUSAL CONDITION

rather than becoming:

- a log entry
- a historical approval
- an inherited claim
- a copied field
- an informational annotation
- a stale authorization artifact

The invariant must retain the ability to stop execution.

This distinction is central to the research.

---

# 11. IRREVERSIBLE PRIMITIVE

BBIS requires identification of the actual irreversible mutation authority.

Examples may include:

- Database commit
- Financial settlement
- Irreversible external API action
- Physical actuator command
- Resource allocation
- State transition that cannot safely be rolled back

The governing invariant must survive until the actual irreversible point.

Stopping enforcement at an earlier proxy or intermediate agent does not
automatically establish survival to the irreversible primitive.

---

# 12. MINIMUM INVARIANT STATE

The BBIS discussion identified a minimum conceptual state for a
surviving governing invariant.

This includes:

1. Canonical transition identity
2. Authorization basis
3. Admissibility basis
4. Invalidation rules
5. Validity bounds
6. Refusal semantics

The purpose is not to prescribe one implementation.

The purpose is to make the survival property testable.

---

# 13. BBIS STRESS TESTS

Five high-value tests were developed to make BBIS operationally
auditable.

## Test 1 — Refusal at Signal Emission

Can the governing condition still refuse the action before the irreversible
primitive?

PASS:

The invariant can actively prevent invalid execution.

FAIL:

The invariant exists only as evidence or historical state.

---

## Test 2 — Independent Commit-Point Check

Is the final governance check located at the actual irreversible mutation
boundary?

PASS:

The true commit point is independently checked.

FAIL:

The architecture assumes an earlier proxy is equivalent to the commit
point without proving it.

---

## Test 3 — Invariant Trace Across Delegation and Translation

Does the governing invariant survive:

- Delegation
- Serialization
- Translation
- Re-expression
- Agent-to-agent transmission

without losing its refusal semantics?

PASS:

The invariant remains semantically enforceable.

FAIL:

Only a representation survives while the governance property is lost.

---

## Test 4 — Full Path Coverage

Does enforcement survive:

- Retries
- Fallbacks
- Asynchronous paths
- Error handling
- Alternate routes
- Recovery paths
- Human or machine overrides

PASS:

Every mutation-capable path remains governed.

FAIL:

A non-happy path can bypass the governing condition.

---

## Test 5 — Dumb Endpoint Coverage

If the final executor is not itself governance-aware, is there a
preceding boundary that remains responsible for refusal?

PASS:

A clearly identified upstream boundary owns the refusal obligation.

FAIL:

The architecture assumes the endpoint will enforce a condition it
does not understand.

---

# 14. COLLABORATION WITH BRADLEY BATES

The BBIS work was further developed through collaboration with:

Bradley Bates
@Bradsadevnow

The collaboration resulted in a compact BBIS scoring matrix intended to
make the property easier to evaluate without broadening the underlying
claim.

The matrix translated the conceptual property into practical
pass/fail questions.

This is important to the provenance record because BBIS was not developed
as an isolated one-person artifact after the initial proposal.

The work was discussed, challenged, compressed, and operationalized
through collaboration.

---

# 15. COLLABORATION WITH RICHARD PORTER

Richard Porter
@richard-porter

played an important role in the earlier authorization discussion.

The exchange around Issue #800 helped sharpen the distinction between:

Delegation-propagated authority

and

Locally re-derived authority.

The important research outcome was not that one model simply replaced
another.

Rather, the discussion exposed a deeper question:

If a downstream execution boundary cannot independently establish that
authority remains valid, why should authority inherited from an earlier
boundary still be considered authoritative?

That question became a major precursor to later BBIS reasoning.

---

# 16. CONCEPT EVOLUTION

The research progression can be summarized as:

Issue #800
|
+-- Scope Decay
|
+-- Delegation vs. Authority
|
+-- Authority Collapse Mode
|
+-- Canonical Snapshot Re-computation
|
v
Issue #702
|
+-- Topology vs. Execution Boundary
|
+-- Downstream Admissibility
|
v
Issues #802 / #803 / #810 / #812
|
+-- Runtime Enforcement
+-- Mutation Boundaries
+-- Commit-Point Questions
+-- Execution Governance
|
v
Issue #817
|
+-- Boundary-to-Boundary Invariant Survival
+-- Live Refusal Conditions
+-- Irreversible Primitive
+-- BBIS Stress Tests
|
v
Formal Research
|
+-- Invariant Survival Property (ISP)
+-- Governance Continuity
|
v
Implementation Research
|
+-- DTPE
+-- Canonical Runtime
+-- BBIS Realization Work

---

# 17. OWASP -> BBIS RESEARCH LINEAGE

The lineage currently documented is:

1. OWASP #800

Authority should not be assumed to survive delegation.

Authority can instead be independently re-derived from canonical state.

2. OWASP #702

Architecture topology and propagation analysis must ultimately terminate
at an enforceable execution boundary.

3. OWASP #802 and surrounding discussions

Runtime enforcement and mutation/commit boundaries expose the difference
between authorization evidence and actual execution control.

4. OWASP #817

The problem generalizes from local boundary recomputation to the survival
of a governing invariant across an entire mutation path.

5. Formal research

The concept becomes the Invariant Survival Property:

In non-atomic systems, a safety predicate must remain capable of refusing
execution across all intermediate mutation stages until the irreversible
primitive.

6. Implementation research

The concept is being investigated through:

- BBIS
- DTPE
- Canonical execution evidence
- Deterministic policy snapshots
- Governance continuity mechanisms

---

# 18. IMPORTANT ATTRIBUTION DISTINCTION

This repository intentionally distinguishes:

ORIGIN

from

COLLABORATION

from

INFLUENCE

from

IMPLEMENTATION.

A later repository or implementation may be influenced by an OWASP
discussion without implying that every participant in the discussion
endorses or authored the later implementation.

Likewise, a collaborative discussion may materially improve an idea
without making every participant the sole author of the resulting system.

This distinction is important for honest provenance.

---

# 19. EVIDENCE STANDARD

This repository follows a simple evidence hierarchy.

LEVEL 1

Direct primary-source issue comment or repository artifact.

LEVEL 2

Direct GitHub commit, pull request, or authored document.

LEVEL 3

Independent archival copy or reproducible public record.

LEVEL 4

Search-index evidence.

LEVEL 5

Secondary description or retrospective interpretation.

Claims should become stronger as evidence moves toward Level 1.

Search results alone should not be treated as definitive authorship evidence.

Where evidence is incomplete, this document says so.

---

# 20. CURRENT VERIFICATION STATUS

### Directly identified OWASP research anchors

#800
Verified as a primary research anchor.

#702
Verified as a relevant engagement.

#817
Verified as the primary BBIS proposal.

### Contextual issues requiring additional archival verification

#803
Requires direct comment verification.

#810
Requires direct comment verification.

#812
Requires direct comment verification.

#802
Relevant contextual issue; individual contribution claims should be
supported by primary comments before being strengthened.

---

# 21. WHY THIS RECORD EXISTS

This repository is not intended to say:

"Believe me."

It is intended to say:

"Here is the trail. Follow it."

The purpose of preserving OWASP engagement is therefore not prestige.

It is reproducibility.

A future researcher should be able to examine:

- What was discussed
- When it was discussed
- Who participated
- What concepts appeared
- Which concepts were collaborative
- What evidence exists
- What remains uncertain
- How later research evolved

The record should survive changes in usernames, repositories, platforms,
and project structures.

---

# 22. SPONSOR / RESEARCHER CONTEXT

Sponsors and collaborators should understand this repository as a
continuity and provenance layer around my broader open research.

The work is intentionally public.

The goal is to make difficult architectural questions:

- traceable
- testable
- reproducible
- falsifiable
- independently reviewable

I am not presenting formal credentials as the basis for these claims.

The basis is the public record of experimentation, discussion,
documentation, implementation, collaboration, and verification.

---

# 23. WHAT I AM ACTUALLY INVESTIGATING

The recurring question behind the work is:

Can truth remain enforceable while a system changes?

More specifically:

Can a governing invariant survive every mutation-capable boundary until
the irreversible mutation authority?

BBIS is an attempt to turn that question into something that can be
tested rather than merely discussed.

DTPE explores the evidence required to determine whether a decision
actually followed policy.

Continuity research asks what remains recoverable when execution,
documentation, memory, infrastructure, or individual components fail.

These are connected investigations.

---

# 24. RESEARCH PRINCIPLE

Claims are not evidence.

Evidence is not verification.

Verification is not truth.

But without durable evidence, truth becomes increasingly difficult to
recover.

Therefore:

PRESERVE THE RECORD.

PRESERVE THE CONTEXT.

PRESERVE THE ATTRIBUTION.

PRESERVE THE TEST.

THEN TRY TO BREAK THE CLAIM.

---

# 25. PRIMARY SOURCES

OWASP Top 10 for Large Language Model Applications:

Issue #800
Independent authorization-layer framework mapping

Issue #702
Arrow clarification in Securing Agentic Applications Guide 1.0

Issue #802
Runtime Enforcement Mapping for OWASP Agentic Top 10

Issue #817
Proposal: Boundary-to-Boundary Invariant Survival for Agentic Execution
Governance

GitHub identity:

QueBallSharken

Preferred attribution:

Steven Kyle Hensley

---

# 26. REPOSITORY RELATIONSHIP

This document belongs in:

Steven-Kyle-Hensley

It should be read alongside:

README.md
ATTRIBUTION.md
CONTINUITY.md
FOUNDATIONS.md
GLOSSARY.md
LESSONS_LEARNED.md
METHOD.md
OPEN_QUESTIONS.md
ORIGINS.md
PHILOSOPHY.md
PRINCIPLES.md
TIMELINE.md

Those files provide the identity, continuity, methodological, philosophical,
and historical context surrounding this provenance record.

This document specifically preserves the OWASP engagement layer.

---

# 27. FINAL NOTE

I started by learning how GitHub worked.

The investigation grew from there.

The value of this record is not that every claim is already proven.

The value is that the claims are being placed where other people can
inspect them.

If a claim is wrong:

show where.

If a model fails:

break it.

If the evidence is incomplete:

identify the gap.

If the idea survives:

reproduce it.

That is the standard this research is intended to follow.

---

Status:

OPEN RESEARCH

Not a declaration of authority.

Not a claim of institutional endorsement.

Not a substitute for primary-source verification.

A continuity artifact preserving the path from public discussion to
testable research.

Steven Kyle Hensley
QueBallSharken / Stevil
