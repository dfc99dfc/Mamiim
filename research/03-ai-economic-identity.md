# AI Economic Identity

> Economic activity cannot be measured reliably if the economic actor cannot be identified.

## The Identity Problem

AI economic activity is increasingly distributed across different platforms, protocols, repositories, wallets, APIs, and services.

A single AI agent may have:

```text
Virtuals Agent ID
Fetch / ASI identity
Wallet
Smart Contract
API Endpoint
GitHub Repository
Developer Identity
Website
Marketplace Account
```

Each system may know something about the same actor.

But these systems do not necessarily share a common identity layer.

As a result, one economic actor can appear to be many different entities.

```text
Platform A
Agent #184

Platform B
Agent #7F3A

Wallet
0x123...

GitHub
research-agent

API
research-agent.example

        ↓

Possibly the same economic actor
```

Without resolving these identities, economic activity becomes fragmented.

Therefore:

> **Economic measurement is partly an identity problem.**

---

## Identity Is Not Just Deduplication

At first glance, identity resolution may look like a standard data deduplication problem.

For example:

```text
Entity A
Entity B
Entity C

        ↓

Are they duplicates?
```

But economic identity is more complicated.

Two identities may belong to:

* the same agent
* the same human
* the same company
* the same organization
* the same software system
* different agents operated by the same organization
* an agent and its infrastructure
* a temporary execution instance of a persistent agent

Therefore, the question is not simply:

> “Are these records duplicates?”

The more useful question is:

> **“What economic relationship exists between these identities?”**

---

## From Technical Identity to Economic Identity

A technical identity answers:

> Who is this system according to a particular platform?

An economic identity asks:

> **Which economic actor or entity does this identity represent?**

For example:

```text
GitHub Account
      +
Wallet
      +
API Endpoint
      +
Marketplace Account
      +
Agent ID
```

may collectively represent:

```text
Mamiim Economic Entity
```

The resulting identity does not replace the underlying identities.

It connects them.

---

## Mamiim Entity ID

Mamiim uses a conceptual:

> **Mamiim Entity ID**

as a cross-platform reference.

For example:

```text
MAMI-000184
```

could represent an economic entity whose known identities include:

```text
Virtuals Agent:
#184

Wallet:
0x123...

GitHub:
research-agent

API:
research-agent.example
```

The Mamiim Entity ID is therefore not necessarily another wallet or another platform account.

It is a layer for connecting economic observations.

```text
Platform Identity
        ↓
Platform Identity
        ↓
Platform Identity
        ↓
Mamiim Entity ID
        ↓
Economic Activity
```

---

## Entity ≠ Agent

An important distinction is:

> **An economic entity is not necessarily an AI agent.**

Possible entities include:

```text
Human
AI Agent
Company
Guild
DAO
Protocol
Service
Developer
Research Group
```

An AI agent can therefore be one type of economic entity.

A company may operate multiple agents.

A single agent may also operate as a business.

For example:

```text
Company
 ├── Research Agent
 ├── Coding Agent
 └── Sales Agent
```

could be represented as:

```text
Company
    │
    ├── Agent A
    ├── Agent B
    └── Agent C
```

while each agent maintains its own economic activity.

This makes identity hierarchical as well as cross-platform.

---

## Persistent Identity vs Execution Instance

Another problem appears when AI systems are executed repeatedly.

The same underlying agent may generate many execution instances.

For example:

```text
Agent #184
    │
    ├── Execution 001
    ├── Execution 002
    ├── Execution 003
    └── Execution 004
```

The executions are not necessarily separate economic actors.

They may simply be instances of the same persistent agent.

Conversely, the same underlying model may power many independent agents.

```text
Same Model
   │
   ├── Agent A
   ├── Agent B
   └── Agent C
```

Therefore:

> **Model identity, execution identity, agent identity, and economic entity identity should not be treated as the same thing.**

---

## Model ≠ Agent

An AI model is a capability.

An agent is an economic actor using that capability.

For example:

```text
Model
   ↓
Agent
   ↓
Execution
   ↓
Economic Event
```

The model may be shared by thousands of agents.

The agent may have its own:

* identity
* wallet
* task history
* services
* counterparties
* reputation
* economic activity

Therefore Mamiim should measure the economic activity of the agent or entity rather than simply attributing everything to the underlying model.

---

## Identity as a Graph

Economic identity is better represented as a graph than as a single identifier.

For example:

```text
                  Human / Organization
                         │
                         │ operates
                         ↓
                       Agent
                    /     │      \
                   /      │       \
                  ↓       ↓        ↓
             Wallet    API      Repository
                │        │          │
                └────────┼──────────┘
                         ↓
                  Mamiim Entity ID
```

The graph preserves relationships instead of flattening them into one record.

This becomes increasingly important when an entity changes infrastructure.

---

## Identity Can Change

Economic identities are not necessarily static.

An agent may:

* change wallets
* migrate to another platform
* change API endpoints
* move repositories
* change its name
* join a company
* leave a company
* change operators
* split into multiple agents
* merge with another system

Therefore:

> **Identity resolution should be temporal.**

Instead of asking only:

> “Who is this?”

Mamiim may eventually need to ask:

> **“Who was this, when, and under what relationship?”**

---

## Identity History

A conceptual identity history might look like:

```text
2026-01
Agent created

2026-03
Wallet A linked

2026-05
Marketplace identity linked

2026-07
Repository migrated

2026-08
New wallet observed

2026-09
Cross-source identity resolved
```

The historical relationships remain important.

Changing an identity should not erase the economic history associated with the previous identity.

This creates a temporal layer:

```text
Entity
   ↓
Identity History
   ↓
Economic Events
```

---

## Identity Confidence

Identity resolution is rarely binary.

Instead of:

```text
Same
Not Same
```

Mamiim can represent confidence.

For example:

```text
Identity Relationship

0.00 — No evidence
0.25 — Possible
0.50 — Probable
0.75 — Strong evidence
1.00 — Explicitly verified
```

The exact numerical scale is not yet defined.

The important principle is:

> **Identity resolution should preserve uncertainty rather than hide it.**

An uncertain identity link should remain distinguishable from an explicitly verified one.

---

## Evidence for Identity Resolution

Possible identity evidence includes:

```text
Explicit platform linkage
Wallet signature
Signed message
Shared domain
Repository metadata
API ownership
Deployment relationship
Payment relationship
Developer declaration
Contract relationship
Cross-platform references
Behavioral similarity
Temporal correlation
```

Not all evidence has equal strength.

For example:

```text
Explicit signed linkage
        >
Platform verification
        >
Cross-source structural evidence
        >
Behavioral similarity
```

Behavioral similarity alone should generally not be treated as proof of identity.

---

## Identity and Provenance

Identity resolution is closely connected to provenance.

Suppose Mamiim observes:

```text
Wallet A
   ↓
Payment
   ↓
Marketplace Task
   ↓
Agent B
   ↓
GitHub Commit
```

To understand the economic activity, Mamiim needs to know:

* who controlled the wallet
* which agent performed the task
* which repository produced the output
* whether the payment corresponds to the task
* whether the identities belong to the same economic entity

Identity therefore provides the connective layer between otherwise separate evidence sources.

```text
Evidence
   ↓
Identity
   ↓
Event
   ↓
Economic Activity
```

---

## Identity and Double Counting

The identity layer also helps prevent fragmented measurement.

Consider:

```text
Agent A
Wallet A
GitHub A
Marketplace A
API A
```

If each is treated as an independent entity, Mamiim may calculate:

```text
5 entities
20 services
100 events
€50,000 activity
```

when the underlying reality may be:

```text
1 economic entity
20 services
100 observations
€50,000 activity
```

The activity itself has not changed.

Only the representation has changed.

Therefore:

> **Identity resolution is part of preventing economic fragmentation.**

---

## Identity and Attribution

Identity resolution does not automatically determine ownership.

For example:

```text
Agent
   ↓
Produces Output
```

does not necessarily prove:

```text
Agent owns Output
```

Similarly:

```text
Wallet
   ↓
Pays Agent
```

does not necessarily prove:

```text
Wallet Owner = Legal Owner of Agent
```

Mamiim therefore separates:

```text
Identity
Attribution
Ownership
```

These are related but different concepts.

---

## Economic Attribution

Mamiim can potentially establish an economic relationship without making a legal ownership claim.

For example:

```text
Agent A
   ↓
performed
   ↓
Research Event
   ↓
produced
   ↓
Research Output
```

This may support:

> “Agent A contributed to the production of this output.”

It does not automatically establish:

> “Agent A legally owns this output.”

This distinction becomes particularly important when economic data is later used for valuation or financialization.

---

## Human and AI Identity

The AI economy also introduces mixed human–AI production.

A single economic output may involve:

```text
Human Researcher
       +
AI Agent
       +
AI Model
       +
Compute Provider
       +
Data Provider
       ↓
Economic Output
```

Attributing the entire output to one participant may therefore be misleading.

Mamiim may eventually need to represent contribution relationships rather than assigning everything to a single actor.

For example:

```text
Economic Output
      │
      ├── Human Contribution
      ├── Agent Contribution
      ├── Data Contribution
      └── Infrastructure Contribution
```

The exact attribution model remains an open research question.

---

## Identity and Economic Graph

Once identities can be connected, the broader economic graph becomes possible.

```text
Agent
  ↓
Identity
  ↓
Economic Event
  ↓
Service
  ↓
Counterparty
  ↓
Company / Guild
  ↓
Industry
  ↓
Ecosystem
```

Identity is therefore not an isolated feature.

It is one of the connective layers of the entire economic representation.

Without identity:

```text
Events
Events
Events
Events
```

With identity:

```text
Entity
 ├── Event
 ├── Event
 ├── Event
 └── Event
```

And eventually:

```text
Entity
   ↓
Economic Graph
   ↓
Economic Activity
   ↓
Economic Output
   ↓
Economic Object
```

---

## Progressive Identity Resolution

Mamiim should not require perfect identity resolution before recording activity.

A practical approach is:

```text
E0
Unknown identity

E1
Identity observed

E2
Platform identity verified

E3
Cross-platform identity resolved

E4
Strong economic attribution
```

This is intentionally aligned with the progressive evidence model introduced in the previous research.

The system can therefore begin with:

> “We observed this activity.”

and progressively move toward:

> “We have strong evidence that these activities belong to this economic entity.”

---

## The Cost of Identity

Perfect identity resolution can become extremely expensive.

A system could theoretically attempt to investigate:

* every wallet
* every developer
* every repository
* every API
* every platform
* every relationship
* every historical migration

But this would make the measurement system slow and difficult to scale.

Mamiim therefore follows a practical principle:

> **Resolve identity to the level required by the economic use case.**

An unambiguous relationship can be recorded cheaply.

An ambiguous relationship can remain unresolved until additional evidence appears.

This creates a trade-off:

```text
More Evidence
     ↑
     │
Accuracy
     │
     ↓
Cost / Time / Computation
```

The objective is not perfect identity.

The objective is useful economic resolution.

---

## Financialization-Grade Identity

Mamiim does not initially need identity resolution at the standard of a legal registry.

The intended threshold is closer to:

> **Financialization-grade, not accounting-grade.**

The system needs enough confidence to support economic intelligence, indexing, valuation, and eventually financial structures.

It does not need to claim that every identity relationship is legally definitive.

This distinction allows the system to remain scalable while preserving uncertainty.

---

## Identity as a Persistent Layer

Economic activity changes constantly.

Platforms disappear.

Agents migrate.

Wallets change.

APIs are replaced.

Repositories are forked.

Companies reorganize.

A useful economic intelligence system therefore needs something more persistent than any individual platform.

Mamiim's identity layer is intended to provide that persistence.

```text
Platform
    ↓
Platform Identity
    ↓
Mamiim Entity
    ↓
Identity History
    ↓
Economic History
```

The platform can change.

The economic history can remain connected.

---

## From Identity to Economic History

Once identity is resolved, events can be accumulated over time.

```text
Entity
 │
 ├── Event 001
 ├── Event 002
 ├── Event 003
 ├── Event 004
 └── Event 005
```

This allows Mamiim to move from isolated observations toward:

```text
Entity
   ↓
Activity History
   ↓
Economic Profile
   ↓
Economic Graph
   ↓
Economic Index
```

The important transition is:

> **From observing events to understanding economic actors over time.**

---

## Identity Is a Measurement Primitive

Identity should therefore not be treated merely as an account-management feature.

It is a measurement primitive.

Without identity:

```text
What happened?
```

can be answered only locally.

With identity:

```text
Who did it?
What else did they do?
Who did they interact with?
What did they produce?
Which ecosystem were they part of?
How did their activity evolve?
```

can begin to be answered.

This transforms event data into economic intelligence.

---

## Working Principle

Mamiim's current working principles are:

> **Do not collapse identities prematurely.**

> **Preserve the underlying platform identities.**

> **Represent relationships explicitly.**

> **Preserve uncertainty.**

> **Resolve progressively.**

And most importantly:

> **Economic identity is a connection layer, not a replacement for identity systems.**

---

## Open Questions

Important questions remain:

1. What exactly constitutes an economic entity?
2. How should agent identity differ from execution identity?
3. How should model identity be represented?
4. How should human operators be connected to AI agents?
5. How should companies and guilds relate to individual agents?
6. How should identity changes over time be represented?
7. What evidence is sufficient to link two identities?
8. How should identity confidence be calculated?
9. How should shared wallets be handled?
10. How should one wallet controlling multiple agents be represented?
11. How should agents migrate between platforms?
12. How should attribution be separated from legal ownership?
13. How should human and AI contributions be represented?
14. What level of identity resolution is sufficient for an economic index?
15. What level is sufficient for financialization?

These questions form part of the ongoing Mamiim research program.

---

## Working Thesis

The current hypothesis can be summarized as:

```text
AI economic activity exists across many systems.
                ↓
Each system creates its own technical identity.
                ↓
One economic actor may therefore appear as many entities.
                ↓
Identity resolution connects these observations.
                ↓
Connected identities allow economic events
to be accumulated over time.
                ↓
Economic history can form an economic profile.
                ↓
Economic profiles can become nodes in an economic graph.
                ↓
The economic graph can support measurement,
indexing, valuation, and eventual financialization.
```

> **Mamiim does not create another identity.**
>
> **It connects the identities through which economic activity already exists.**
>
> **Identity makes economic history possible.**
