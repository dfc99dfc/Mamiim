# AI Economic Ontology

> **An economic ontology defines the shared vocabulary through which an AI economy can be observed, represented, and connected.**

## Why an Economic Ontology?

Mamiim is designed to connect economic activity across systems that were not necessarily designed to understand one another.

Different platforms may describe similar things differently.

For example:

```text
Virtuals
→ Job

Olas
→ Service / Mech

OKX
→ Task

Binance
→ Skill

GitHub
→ Commit

Blockchain
→ Transaction

Marketplace
→ Order

Research System
→ Experiment / Result
```

These are different technical representations.

The economic question is:

> **Can they be represented within a common economic vocabulary?**

This is the purpose of an Economic Ontology.

---

# What Is an Ontology?

An ontology defines the important entities in a domain and the relationships between them.

It answers:

* What kinds of things exist?
* What distinguishes them?
* How are they related?
* Which concepts can contain or produce other concepts?
* Which concepts are observations versus interpretations?

For Mamiim, the ontology is not intended to describe all of AI.

It describes the **economic layer of AI activity**.

---

# The Mamiim Economic Ontology

A first version can be organized into several layers:

```text id="n4m8q2"
IDENTITY
    ↓
ACTIVITY
    ↓
OUTPUT
    ↓
ORGANIZATION
    ↓
ECONOMIC RELATIONSHIPS
    ↓
MEASUREMENT
    ↓
CLAIM
    ↓
MARKET
```

The core objects are:

```text id="q7p3m8"
Agent
Identity
Economic Event
Activity
Service
Skill
Economic Output
Economic Object
Counterparty
Organization
Industry
Ecosystem
Economic Claim
Measurement
Index
Financial Instrument
```

These objects should not be treated as interchangeable.

---

# 1. Agent

An **Agent** is a persistent economic actor capable of performing economic activity.

An agent may be:

* an AI agent
* a human
* an organization
* another persistent economic actor

For Mamiim, the important property is not whether the actor is human or artificial.

The important property is:

> **Can this entity participate in an economic process?**

---

# 2. Model

A **Model** is the computational system underlying an AI capability.

Examples include:

```text id="w5m8r2"
Foundation Model
Fine-Tuned Model
Specialized Model
Open-Source Model
Proprietary Model
```

A model is not automatically an Agent.

One model can power many agents.

```text id="m3q8p4"
Model
 ├── Agent A
 ├── Agent B
 ├── Agent C
 └── Agent D
```

This distinction is important for economic attribution.

---

# 3. Identity

**Identity** represents a technical or organizational identifier through which an entity can be observed.

Examples:

```text id="x8n4m2"
Wallet
Contract
Platform ID
Agent ID
API Endpoint
Developer Account
Repository
Website
Organization ID
```

One entity may have multiple identities.

```text id="p6q3m8"
Entity
 ├── Virtuals ID
 ├── Fetch ID
 ├── Wallet
 ├── Contract
 └── Website
```

Mamiim attempts to resolve these observations into a persistent economic identity.

---

# 4. Mamiim Entity

A **Mamiim Entity** is Mamiim's internal representation of a persistent economic actor or entity.

Conceptually:

```text id="j5m8q2"
Technical Identities
        ↓
Identity Resolution
        ↓
Mamiim Entity
```

The Entity is not necessarily a legal entity.

It is an economic reference.

This distinction allows Mamiim to operate without pretending that every machine identity corresponds directly to a legal person or company.

---

# 5. Economic Event

An **Economic Event (SE)** is the smallest observable event that represents a potentially productive or economically meaningful action.

Examples:

```text id="r4n7p2"
Task Completed
Service Delivered
Payment Received
Compute Provided
Dataset Licensed
Research Contribution
Software Contribution
Trade Executed
Reward Received
```

The key word is **potentially**.

A technical event is not automatically an Economic Event.

---

# 6. Technical Event

A Technical Event is an observable occurrence in a technical system.

Examples:

```text id="v8m3q6"
Commit
API Call
Transaction
Message
Execution
File Creation
Database Update
```

A Technical Event can become evidence for an Economic Event.

```text id="c5p8n2"
Technical Event
      ↓
Context
      ↓
Economic Classification
      ↓
Economic Event
```

This distinction prevents Mamiim from treating every technical action as economic production.

---

# 7. Activity

**Activity** describes the economic nature of an event or collection of events.

A preliminary taxonomy is:

```text id="q2m7r8"
TRADE
SERVICE
COMPUTE
DATA
CONTENT
LICENSING
SUBSCRIPTION
RESEARCH
PAYMENT
TRANSFER
CAPITAL
REWARD
```

Activity is therefore a classification.

It is not necessarily an independent object.

For example:

```text id="n8p4m3"
Economic Event
Activity:
SERVICE
```

---

# 8. Service

A **Service** is a repeatable economic capability offered by an agent or organization.

Examples:

```text id="x3q7m9"
Data Analysis
Translation
Image Generation
Code Review
Market Research
Trading Strategy
Physical Task
```

A service can generate multiple Economic Events.

```text id="m6p2r8"
Service
   ↓
Event 001
Event 002
Event 003
Event 004
```

---

# 9. Skill

A **Skill** is a capability that enables an agent to perform a task or provide a service.

The distinction between Skill and Service is useful:

```text id="w4n8q2"
Skill
"What can this actor do?"

Service
"What does this actor provide economically?"
```

For example:

```text id="p7m3x5"
Skill:
Data Analysis

Service:
$20 Data Analysis Report
```

A skill can therefore contribute to one or many services.

---

# 10. Economic Output

An **Economic Output** is the result produced by an Economic Event or activity.

Examples:

```text id="j8q4m2"
Report
Software
Research Result
Dataset
Design
Model
Analysis
Physical Task Completion
```

The output may or may not become a persistent Economic Object.

---

# 11. Economic Object

An **Economic Object** is:

> **A persistent, identifiable economic entity formed from one or more economic events and capable of being measured, valued, claimed, or potentially financialized.**

Examples:

```text id="r5m8q3"
Software Project
Research Output
Dataset
AI Skill
AI Service
AI-generated IP
Scientific Discovery
Digital Asset
```

The distinction is:

```text id="x2n7p4"
Event
  ↓
Output
  ↓
Persistent Object
```

An event happens.

An output is produced.

An object persists.

---

# 12. Counterparty

A **Counterparty** is another entity participating in an economic relationship.

For example:

```text id="v6m3q8"
Agent A
      ↓
provides service to
      ↓
Agent B
```

Agent B is the counterparty.

Counterparties can be:

* agents
* humans
* companies
* protocols
* platforms
* organizations
* other economic entities

---

# 13. Organization

An **Organization** is a persistent economic structure coordinating multiple participants or activities.

Examples:

```text id="q8p3m5"
Company
Guild
DAO
Research Organization
Agent Collective
```

An organization may contain:

```text id="m4n7r2"
Organization
 ├── Agent A
 ├── Agent B
 ├── Agent C
 └── Economic Objects
```

A single AI agent may also operate independently without belonging to an organization.

---

# 14. Industry

An **Industry** groups economically related organizations, agents, services, or activities.

For example:

```text id="x7m2q8"
AI Economy
 ├── AI Research
 ├── AI Software
 ├── AI Services
 ├── AI Compute
 ├── AI Data
 └── AI Robotics
```

Industry is therefore an aggregation layer.

It is not necessarily an actor.

---

# 15. Ecosystem

An **Ecosystem** represents a broader economic environment containing multiple actors, organizations, services, and infrastructure.

Examples could include:

```text id="p3n8m5"
Agent Ecosystem
Marketplace Ecosystem
Blockchain Ecosystem
Research Ecosystem
AI Economy
```

An ecosystem may contain multiple industries.

---

# 16. Economic Claim

An **Economic Claim** represents an economic interest, potential right, or exposure associated with an Economic Object or activity.

Examples:

```text id="j6q2m8"
Revenue Claim
Royalty Claim
Licensing Claim
Usage Claim
Contribution Claim
Prize Claim
Future Payment Claim
```

A claim is not the same as the underlying object.

```text id="r8m4p2"
Economic Object
      ↓
Economic Claim
```

---

# 17. Measurement

A **Measurement** represents a quantified observation about economic activity.

Examples:

```text id="w5q3m7"
Economic Activity
Revenue
Usage
Growth
Event Count
Output Count
Capital
```

Measurement answers:

> **What can we observe and quantify?**

It does not necessarily answer:

> What is it worth?

---

# 18. Index

An **Index** aggregates multiple measurements into a structured representation of an economic category.

For example:

```text id="n7m2p8"
Economic Events
      ↓
Industry Measurements
      ↓
AI Research Index
```

or:

```text id="x4q8m3"
Multiple Industries
      ↓
AI Economy Index
```

An index is therefore a measurement structure.

It is not automatically a financial product.

---

# 19. Financial Instrument

A **Financial Instrument** represents some form of marketable or programmable economic exposure.

Examples include:

```text id="m8p4r2"
Equity
Debt
Revenue Share
Royalty Structure
Tokenized Claim
Index Exposure
Event Contract
```

The financial instrument is downstream of the economic object and claim.

```text id="q3n7m5"
Economic Object
      ↓
Economic Claim
      ↓
Financial Instrument
```

---

# The Core Object Hierarchy

The most important distinctions can be summarized as:

```text id="v8m2q6"
Technical Event
      ↓
Economic Event
      ↓
Economic Output
      ↓
Economic Object
      ↓
Economic Claim
      ↓
Financial Instrument
```

These are different layers of representation.

---

# Event vs Activity

An event is something that happened.

Activity describes what kind of economic action it represents.

```text id="j5q8m3"
Event:
Agent A completed task X

Activity:
SERVICE
```

The activity is a classification of the event.

---

# Activity vs Output

Activity describes the action.

Output describes its result.

```text id="m7n3p8"
Activity:
RESEARCH

Output:
Research Result
```

Multiple events may contribute to one output.

---

# Output vs Object

An output is produced.

An Economic Object persists.

```text id="x2m8q4"
Event
 ↓
Output
 ↓
Persistent Object
```

For example, one research event may produce a proof fragment.

A sequence of research events may eventually form a persistent research output.

---

# Object vs Claim

An object exists.

A claim represents an economic interest associated with it.

```text id="r6p3m9"
Research Output
      ↓
Potential Licensing Claim
```

The research output is not itself the licensing claim.

---

# Claim vs Financial Instrument

A claim represents an economic interest.

A financial instrument represents that exposure in a financial structure.

```text id="q8m4n2"
Claim
 ↓
Financial Representation
```

The representation may be transferable or programmable.

---

# Agent vs Entity

An Agent is an actor capable of economic activity.

An Entity is a broader persistent economic reference.

Therefore:

```text id="p5m7x3"
Entity
 ├── Agent
 ├── Company
 ├── Organization
 └── Other persistent economic actor
```

Not every Entity is an Agent.

---

# Agent vs Model

A Model provides computational capability.

An Agent uses capabilities to perform tasks.

```text id="v3n8m5"
Model
   ↓
Agent
   ↓
Economic Activity
```

The same model may power many agents.

---

# Skill vs Service

A Skill is a capability.

A Service is an economic offering.

```text id="m6q2p8"
Skill
"What can be done?"

Service
"What is offered?"
```

The distinction allows Mamiim to measure both capabilities and economic demand.

---

# Company vs Organization

A company is one type of organization.

Other organizations may include:

* guilds
* DAOs
* research groups
* agent collectives

Therefore Mamiim should use **Organization** as the general graph concept.

---

# Industry vs Ecosystem

An Industry groups economic activity by economic domain.

An Ecosystem describes a broader environment in which actors and infrastructure interact.

For example:

```text id="x8m4q2"
AI Economy
   ↓
AI Research Industry
   ↓
Research Organizations
   ↓
Agents
```

The same ecosystem can contain multiple industries.

---

# Relationships

The ontology becomes useful when relationships are defined.

A first relationship vocabulary could include:

```text id="q4n7m8"
IDENTITY
is_identified_by
resolves_to

ACTIVITY
performs
provides
consumes
pays
receives
trades_with
licenses
uses
contributes_to

OUTPUT
produces
derived_from
depends_on
transforms

ORGANIZATION
belongs_to
employs
coordinates
owns
operates

GRAPH
related_to
supports
counterparty_of

OBJECT
contains
version_of
derived_from
supports_claim

FINANCIAL
claims
values
references
financializes
```

These relationships form the edges of the Economic Graph.

---

# The Core Economic Graph

A simplified graph is:

```text id="m8q3p7"
Agent
  │
  ├── performs → Economic Event
  │
  ├── provides → Service
  │
  ├── has → Skill
  │
  └── belongs_to → Organization
                    │
                    ↓
                  Industry

Economic Event
  │
  ├── has → Activity
  ├── produces → Output
  ├── interacts_with → Counterparty
  └── supported_by → Evidence

Output
  │
  └── becomes → Economic Object
                     │
                     └── supports → Economic Claim
                                      │
                                      └── represented_by
                                                ↓
                                      Financial Instrument
```

---

# Provenance in the Ontology

Provenance should not be treated as a separate isolated object.

It is a property of relationships and transformations.

For example:

```text id="p6m8q3"
Object X
   │
   └── derived_from
          │
        Event A
          │
          └── evidence → Commit
```

The provenance chain allows Mamiim to explain why a relationship exists.

---

# Evidence

Evidence is the basis on which economic records are established.

Examples:

```text id="n3q7m5"
Onchain Transaction
Platform Record
API Record
Commit
Execution Log
Published Output
Contract
Payment
Human Verification
```

Evidence can support:

* identity
* event classification
* attribution
* output
* claim

---

# Confidence

Every interpreted relationship may have a confidence level.

For example:

```text id="x5m8r2"
Agent A
   ↓
contributed_to
   ↓
Object X

Confidence:
E3
```

The evidence level can be represented alongside the relationship.

This allows uncertain relationships to remain in the graph without being treated as equally established.

---

# Temporal Dimension

Economic relationships change over time.

An agent may:

```text id="q7m3p8"
join Organization A
      ↓
leave Organization A
      ↓
join Organization B
```

A service may:

```text id="m4n8x2"
launch
 ↓
grow
 ↓
decline
 ↓
discontinue
```

Therefore relationships should ideally have temporal information.

Conceptually:

```text id="r8p2m5"
Relationship
 ├── start
 ├── end
 ├── evidence
 └── confidence
```

---

# Identity History

Identity itself may evolve.

An agent can:

```text id="v6m3q8"
Wallet A
   ↓
Wallet B
   ↓
Contract C
```

The historical relationship should not necessarily be overwritten.

Instead:

> **Identity is a history, not only a current label.**

This preserves provenance.

---

# Ontology and Double Counting

The ontology helps determine whether two observations represent:

```text id="x3q7m9"
Two Economic Events
```

or:

```text id="n5m8p2"
Two observations
of one Economic Event
```

For example:

```text id="j8m4q3"
Service Completion
      ↓
Payment
      ↓
Settlement
```

may contain multiple technical observations of one underlying economic process.

The ontology provides the conceptual structure needed to distinguish them.

---

# Ontology and Aggregation

The same ontology supports aggregation:

```text id="p2m7n8"
Economic Events
      ↓
Activities
      ↓
Economic Objects
      ↓
Organizations
      ↓
Industries
      ↓
Ecosystems
      ↓
AI Economy
```

Each layer can be measured without losing the lower-level history.

---

# Ontology and AI GDP

AI GDP-like measurements can use ontology-defined categories.

For example:

```text id="w4q8m2"
Economic Event
   ↓
Activity = SERVICE
   ↓
Industry = AI Services
   ↓
Economic Measurement
   ↓
AI Economy Aggregate
```

This makes macro measurement traceable to underlying economic observations.

---

# Ontology and Financialization

Financialization can also reference ontology-defined objects.

```text id="z7m3q5"
Economic Object
      ↓
Claim
      ↓
Valuation
      ↓
Financial Instrument
```

The financial layer can therefore reference an underlying economic structure rather than an isolated token or number.

---

# Ontology as Interoperability

The ontology creates a translation layer between platforms.

For example:

```text id="k5n8p2"
Virtuals:
Job

Olas:
Service

OKX:
Task

GitHub:
Commit

Blockchain:
Transaction
```

Mamiim can ask:

> What economic role does this observation represent?

and map it into a common vocabulary.

```text id="m3q7x8"
Platform Representation
        ↓
Mamiim Ontology
        ↓
Economic Event
```

---

# Ontology Is Not a Forced Normalization

Different systems can preserve their original terminology.

Mamiim does not need to erase platform-specific concepts.

Instead:

```text id="r8m2p6"
Source Concept
      ↓
Mapped Concept
      ↓
Source Context Preserved
```

For example:

```text id="n4q7m3"
OKX:
Task

Mamiim:
Economic Event
Activity:
SERVICE
Source Type:
OKX Task
```

The original observation remains available.

---

# Ontology and Machine Reasoning

A common ontology also allows AI systems to reason about economic structures.

An AI agent could query:

> Find agents providing data-analysis services with increasing demand.

The system can translate this into:

```text id="x6m3q8"
Agent
AND
Service = Data Analysis
AND
Demand Growth > threshold
```

The ontology provides the shared semantics required for such queries.

---

# Ontology as a Primitive

If Mamiim succeeds, its ontology may become more valuable than any individual dashboard.

The ontology defines:

```text id="p7m4n8"
What counts as an entity
What counts as an event
What counts as activity
What counts as an object
What relationships exist
How evidence is attached
How uncertainty is represented
```

This becomes the conceptual foundation for the Economic Graph.

---

# The Mamiim Data Model

A simplified object model is:

```text id="q8m3r5"
ENTITY
 ├── Identity
 ├── Agent
 └── Organization

ACTIVITY
 ├── Economic Event
 ├── Service
 └── Skill

OUTPUT
 ├── Economic Output
 └── Economic Object

RELATIONSHIP
 ├── Counterparty
 ├── Contribution
 ├── Provenance
 └── Organization Membership

MEASUREMENT
 ├── Activity
 ├── Revenue
 ├── Growth
 └── Index

CLAIM
 └── Economic Claim

MARKET
 └── Financial Instrument
```

This is a conceptual model, not yet a final database schema.

---

# Minimal Mamiim Ontology

The MVP does not need to implement the entire ontology.

A minimal version could begin with:

```text id="m5q8n2"
Agent
Identity
Economic Event
Activity
Output
Economic Object
Evidence
Confidence
```

Then progressively add:

```text id="x7p3m8"
Service
Skill
Counterparty
Organization
Industry
Claim
Measurement
Index
Financial Instrument
```

This keeps the initial system manageable.

---

# The Smallest Useful Schema

A minimal Economic Event might contain:

```text id="v4n8q2"
SE ID
Actor
Identity
Timestamp
Activity Type
Counterparty
Input
Output
Value
Source
Evidence
Confidence
Related Object
```

This is enough to begin building a meaningful economic graph.

---

# The Economic Object Schema

A minimal Economic Object could contain:

```text id="j3m7p8"
Object ID
Object Type
Produced By
Underlying Events
Inputs
Outputs
Version
Provenance
Evidence
Status
Associated Claims
```

This allows the object to remain connected to its history.

---

# The Economic Claim Schema

A minimal claim could contain:

```text id="q6m2r9"
Claim ID
Claim Type
Underlying Object
Claimant
Potential Value
Realized Value
Status
Evidence
Legal Status
Financialization Status
```

This prevents the system from collapsing potential value into realized revenue.

---

# Ontology Versioning

The ontology itself will evolve.

For example:

```text id="n8p3m5"
Ontology v0.1
   ↓
Ontology v0.2
   ↓
Ontology v1.0
```

New economic behaviors may require new categories.

Existing categories may need refinement.

Therefore Mamiim should preserve ontology versions rather than silently changing historical classifications.

---

# Why This Matters

Without a shared ontology:

```text id="w7m3q8"
Platform A
Platform B
Platform C
Platform D
```

remain separate datasets.

With an ontology:

```text id="x4n8p2"
Platform A
Platform B
Platform C
Platform D
       ↓
Common Economic Vocabulary
       ↓
Economic Graph
```

This is what makes cross-ecosystem economic intelligence possible.

---

# What Mamiim Should Not Assume

### Every technical event is an Economic Event.

Economic meaning requires context.

### Every Agent is an AI.

Humans and organizations can also be economic actors.

### Every Entity is an Agent.

Companies, organizations, and other persistent entities may exist independently.

### Every Output is an Economic Object.

Persistence and economic relevance matter.

### Every Object has a Claim.

Measurement does not create ownership.

### Every Claim is legally enforceable.

Legal status must remain separate.

### Every Financial Instrument maps cleanly to one Object.

Financial structures can reference multiple objects or claims.

### The ontology is finished.

The AI economy itself is still evolving.

---

# Working Ontology

The current Mamiim ontology can be summarized as:

```text id="p8m4q3"
                    ECOSYSTEM
                        │
                     INDUSTRY
                        │
                   ORGANIZATION
                        │
        ┌───────────────┴───────────────┐
        ↓                               ↓
      AGENT                         COUNTERPARTY
        │
        ↓
     IDENTITY
        │
        ↓
 ECONOMIC EVENT
        │
   ┌────┼────┐
   ↓    ↓    ↓
ACTIVITY INPUT OUTPUT
             │
             ↓
     ECONOMIC OBJECT
             │
             ↓
      ECONOMIC CLAIM
             │
             ↓
         VALUATION
             │
             ↓
   FINANCIAL INSTRUMENT
```

And across the entire graph:

```text id="m7q2n8"
EVIDENCE
   +
PROVENANCE
   +
CONFIDENCE
   +
TIME
```

These provide the historical and epistemic context for the graph.

---

# The Ontology as Mamiim's Language

The deeper purpose of the ontology is not simply database organization.

It creates a common language for the AI economy.

Different platforms may produce different technical objects.

Mamiim attempts to translate them into a shared economic vocabulary.

```text id="q3m8p5"
Many Technical Languages
          ↓
      Mamiim Ontology
          ↓
One Economic Language
```

This language allows economic activity to become comparable across systems.

---

# Working Thesis

The current hypothesis is:

> **The AI economy will emerge across many technical systems with different identities, terminology, and data structures.**

> **Economic intelligence requires a common vocabulary capable of representing actors, events, activities, outputs, objects, claims, and relationships across these systems.**

> **Mamiim's Economic Ontology provides the conceptual language for its Economic Graph.**

> **The ontology allows fragmented technical observations to become comparable economic representations without erasing their original context.**

The resulting architecture is:

```text id="v8m3q7"
TECHNICAL SYSTEMS
      ↓
Technical Events
      ↓
MAMIIM ECONOMIC ONTOLOGY
      ↓
Economic Events
      ↓
Economic Identity
      ↓
Economic Provenance
      ↓
Economic Graph
      ↓
Economic Objects
      ↓
Measurement / Index
      ↓
Economic Intelligence
      ↓
Financialization
```

> **Different systems speak different technical languages.**

> **Mamiim is building a common economic language for the AI economy.**
