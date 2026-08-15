# Steven Kyle Hensley — Independent Security Architecture Services

Status: Independent Research / Professional Services

Preferred Attribution:

Steven Kyle Hensley
QueBallSharken / Stevil

---

# Overview

I conduct independent security architecture analysis focused on
authorization boundaries, agentic execution, governance continuity,
trust evidence, provenance, and mutation-capable execution paths.

My work is informed by ongoing research into:

- Boundary-to-Boundary Invariant Survival (BBIS)
- Active Invariant Cloning (AIC)
- Deterministic Trust & Policy Evidence (DTPE)
- Boundary Evidence Analysis Framework (BEAF)
- Agent governance
- Authorization architecture
- Provenance and trust evidence
- Continuity-first architecture
- Execution and mutation boundaries

The objective is straightforward:

Identify where a system claims to enforce a security or governance
condition, determine what evidence actually demonstrates that enforcement,
and identify whether that condition remains effective through the execution
path.

---

# Core Principle

Claims are not evidence.

Evidence is not verification.

Verification is not truth.

Security architecture should therefore be evaluated by what can actually
be demonstrated at the enforcement boundary.

---

# Services

## 1. Architecture Review

### Typical Range

$250–$500

### Best For

- Small software projects
- Startups
- Developers
- Open-source projects
- Early-stage AI systems
- Authorization architecture questions

### Scope

A focused review of a supplied architecture, execution flow, or selected
code/configuration.

Typical areas:

- Authorization flow
- Authentication assumptions
- Enforcement boundaries
- State and version assumptions
- Evidence production
- Mutation paths
- Failure paths
- Commit/effect boundaries
- Governance gaps

### Deliverable

A concise written technical assessment containing:

- Architecture observations
- Boundary analysis
- Evidence gaps
- Identified failure modes
- Security implications
- Recommended next steps

---

# 2. Deep Authorization Assessment

### Typical Range

$750–$2,000

### Best For

- SaaS applications
- API platforms
- Authorization gateways
- Agent systems
- Multi-service architectures
- Systems with complex delegation

### Scope

A deeper adversarial analysis of authorization and execution architecture.

May include:

- Boundary decomposition
- Authorization-path analysis
- Identity binding
- Context binding
- State/version validity
- Authorization lineage
- Mutation identity
- Delegation analysis
- Retry and recovery paths
- Fallback paths
- Alternate execution routes
- Terminal commit/effect analysis
- Adversarial scenarios

### Deliverable

A formal technical assessment containing:

- Architecture model
- Boundary map
- Threat/failure analysis
- Evidence analysis
- Adversarial findings
- Severity/prioritization
- Remediation recommendations
- Questions requiring additional evidence

---

# 3. Agent Governance / Security Architecture Review

### Typical Range

$2,500–$7,500+

### Best For

Organizations developing:

- AI agents
- Multi-agent systems
- Tool-use systems
- Agent orchestration platforms
- Policy enforcement systems
- Authorization infrastructure
- High-impact automation
- Distributed execution systems

### Scope

A comprehensive examination of how authorization and governance
conditions propagate through an execution architecture.

Potential areas include:

- Agent-to-agent delegation
- Tool authorization
- Policy enforcement
- Authorization lineage
- Mutation-capable boundaries
- Governance continuity
- State transitions
- Execution tickets
- Trust evidence
- Provenance
- Retry/fallback behavior
- Asynchronous execution
- Recovery paths
- Human or machine overrides
- Irreversible effects
- Terminal mutation authority

### Deliverable

Depending on engagement scope:

- Architecture assessment
- Governance boundary map
- Authorization lineage analysis
- Adversarial threat model
- Evidence requirements
- Failure-mode analysis
- Recommended controls
- Validation/test plan
- Executive summary
- Technical appendix

---

# 4. Custom Research / Architecture Engagement

### Typical Range

$5,000–$15,000+

### Best For

Organizations facing a difficult security architecture question that does
not fit a standard review.

Potential engagements include:

- Independent architecture research
- Adversarial design review
- Authorization model analysis
- Agent governance research
- Provenance analysis
- Trust-evidence analysis
- Boundary enforcement research
- Security architecture experimentation
- Prototype validation
- Independent technical review

Scope and pricing are determined after reviewing the problem.

---

# 5. Research Collaboration

### Pricing

Negotiated.

Research collaborations may involve:

- Joint experiments
- Architecture analysis
- Adversarial testing
- Methodology development
- Independent review
- Reproducibility studies
- Open-source research
- Standards discussions

Collaborative work should clearly distinguish:

- Original contribution
- Collaboration
- Influence
- Implementation
- Independent verification

Attribution should be agreed upon before publication when appropriate.

---

# What I Actually Evaluate

A typical review asks questions such as:

    Where does authorization actually happen?

    What evidence proves that it happened?

    Can an authorized state become unauthorized before execution?

    Can downstream components inherit stale authority?

    Can two boundaries authorize different mutations?

    Does authorization remain bound to the mutation being executed?

    Can an alternate path bypass the intended enforcement boundary?

    What happens during retry?

    What happens during fallback?

    What happens during asynchronous execution?

    What happens during recovery?

    Where is the actual irreversible mutation authority?

    Can the system prove that the required governance condition
    remained enforceable until that point?

The objective is not to make an architecture look secure.

The objective is to determine what can actually be demonstrated.

---

# Research-Informed Methodology

My commercial architecture work is informed by independent research.

Current research areas include:

## BBIS

Boundary-to-Boundary Invariant Survival investigates whether a governing
invariant can remain a live refusal condition across mutation-capable
boundaries until the irreversible mutation authority.

## AIC

Active Invariant Cloning investigates whether governing authorization
semantics can be actively instantiated and compositionally preserved across
multiple enforcement boundaries.

## DTPE

Deterministic Trust & Policy Evidence investigates whether a system can
produce durable evidence that a decision actually followed the applicable
policy and authority state.

## BEAF

Boundary Evidence Analysis Framework is a private research methodology
currently undergoing empirical validation.

BEAF should not be represented as a validated industry standard or
universally established methodology.

Its current status is research.

---

# Important Research Disclaimer

The research described here is independent research.

It should not be interpreted as:

- Institutional endorsement
- OWASP endorsement
- Certification
- Formal accreditation
- A guarantee of security
- A guarantee of compliance
- A substitute for professional legal advice
- A substitute for organizational security testing

Research findings are evidence-based observations within the scope of the
review performed.

No security assessment can guarantee that an undiscovered vulnerability
does not exist.

---

# Pricing Philosophy

Pricing ranges are intentionally transparent.

The actual price of an engagement depends on:

- System complexity
- Scope
- Code volume
- Number of execution boundaries
- Number of services
- Number of environments
- Required testing
- Documentation quality
- Client availability
- Turnaround requirements
- Required deliverables

A quoted engagement may therefore fall above or below the published
ranges when scope materially differs.

The ranges are starting points, not automatic invoices.

---

# Initial Engagement Process

## Step 1 — Problem Definition

The client describes:

- System
- Architecture
- Security concern
- Desired outcome

## Step 2 — Scope

The review identifies:

- Boundaries
- Components
- Evidence available
- Execution paths
- Required deliverables

## Step 3 — Fixed Scope / Price

A written scope and price are agreed upon before work begins.

## Step 4 — Analysis

The architecture is examined using adversarial and evidence-oriented
analysis.

## Step 5 — Findings

Observations are documented with supporting evidence.

## Step 6 — Delivery

The client receives the agreed technical deliverable.

## Step 7 — Optional Follow-Up

Additional remediation review or validation may be performed separately.

---

# What Clients Should Provide

Depending on engagement scope:

- Architecture diagrams
- Relevant source code
- Authorization policies
- Configuration
- API definitions
- Execution traces
- Attestation formats
- Identity model
- State/version model
- Deployment information
- Known threat assumptions

Clients should never provide credentials, secrets, private keys, or
unnecessary sensitive information.

---

# First-Customer / Pilot Pricing

For initial engagements intended to establish real-world case studies,
the following reduced ranges may be available:

    Focused Architecture Review       $150–$300

    Authorization Assessment           $500–$1,000

    Agent Governance Review            $1,500–$3,500

Pilot pricing is limited and subject to scope.

The purpose of pilot engagements is to generate:

- Real-world evidence
- Reproducible findings
- Case studies
- Client feedback
- Methodology refinement

Client confidentiality takes priority over publication.

No client information should be publicly disclosed without permission.

---

# Long-Term Research-to-Product Direction

The current work is intentionally progressing in stages:

    PUBLIC RESEARCH
          |
          v
    TECHNICAL PORTFOLIO
          |
          v
    ARCHITECTURE REVIEWS
          |
          v
    REAL-WORLD CASE STUDIES
          |
          v
    REPEATABLE ASSESSMENT PROCESS
          |
          v
    EMPIRICAL VALIDATION
          |
          v
    PROFESSIONAL METHODOLOGY
          |
          v
    TRAINING / ASSESSMENT / TOOLING
          |
          v
    ENTERPRISE SERVICES / LICENSING
