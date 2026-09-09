# AI Economic Event Model

> **A Single Economic Event is the smallest observable event that represents a potentially meaningful economic action.**

## Why Economic Events Matter

Mamiim ultimately wants to measure an economy.

But an economy cannot be measured directly.

It must first be observed through events.

```text
AI Economy
    ↓
Economic Activity
    ↓
Economic Events
    ↓
Measurement
```

The Economic Event is therefore one of the most important primitives in the Mamiim system.

If events are defined incorrectly, everything above them becomes unreliable:

```text
Events
  ↓
Objects
  ↓
Graph
  ↓
Measurement
  ↓
Index
  ↓
Financialization
```

Mamiim therefore needs a precise but practical event model.

---

# What Is a Single Economic Event?

Mamiim defines:

> **SE = Single Economic Event**

> **The smallest observable event that represents a potentially productive or economically meaningful action.**

There are three important parts:

### Smallest

An SE should represent one meaningful economic occurrence rather than an entire process.

### Observable

The event should be supported by evidence.

### Potentially economic

Not every technical event is necessarily economically meaningful.

This distinction is fundamental.

---

# Technical Event ≠ Economic Event

A technical system may produce millions of events.

For example:

```text
API Request
Database Write
Git Commit
Model Inference
Message
Transaction
File Creation
```

But not all of these represent economic activity.

Consider:

```text
Git Commit
"fix typo in README"
```

This is technically observable.

It may not represent meaningful economic production.

Compare:

```text
Git Commit
"implement payment settlement system"
```

This may represent a meaningful contribution to an economic output.

Therefore:

```text
Technical Event
      ↓
Context
      ↓
Economic Classification
      ↓
Economic Event
```

The event model must preserve this distinction.

---

# The SE Boundary

The most difficult question is often not:

> What happened?

It is:

> **Where does one economic event begin and end?**

Consider an AI agent completing a task:

```text
Task Assigned
     ↓
Agent Starts
     ↓
Agent Calls Tools
     ↓
Agent Produces Output
     ↓
Output Accepted
     ↓
Payment
     ↓
Settlement
```

Technically, this may generate hundreds or thousands of events.

Economically, it may represent:

```text
One Service Event
```

or several distinct events.

Mamiim therefore needs to distinguish:

```text
Technical Event
vs
Economic Event
vs
Economic Process
```

---

# Economic Process

An **Economic Process** is a sequence of related economic events.

For example:

```text
Economic Process
│
├── Task Created
├── Service Performed
├── Output Delivered
├── Output Accepted
└── Payment Settled
```

The process is larger than an SE.

An SE is one economically meaningful observation within the process.

This gives Mamiim three levels:

```text
Technical Event
      ↓
Economic Event
      ↓
Economic Process
```

---

# What Should an SE Represent?

A useful SE should answer:

```text
WHO
did WHAT
TO / FOR WHOM
WHEN
using WHAT
producing WHAT
with WHAT economic significance
supported by WHAT evidence?
```

A minimal representation is:

```text
SE
├── actor
├── identity
├── timestamp
├── activity
├── counterparty
├── input
├── output
├── value
├── source
├── evidence
└── confidence
```

Additional fields can be added when available.

---

# 1. SE ID

Every event should have a persistent identifier.

Example:

```text
SE-000184
```

The ID should identify the Mamiim event record.

It should not replace the original source identifier.

For example:

```text
Mamiim:
SE-000184

Source:
GitHub Commit abc123
```

This preserves source provenance.

---

# 2. Actor

The actor is the entity responsible for the event.

For example:

```text
Actor:
Research Agent #184
```

The actor should reference a Mamiim Entity rather than only storing a text label.

```text
SE
 ↓
Actor
 ↓
Mamiim Entity
```

---

# 3. Identity

The event should preserve the identity through which it was observed.

Examples:

```text
Wallet
Agent ID
Platform Account
Developer Account
API Endpoint
Contract
Repository
```

For example:

```text
Actor:
Mamiim Entity MAMI-000184

Observed Identity:
Virtuals Agent ID 184
```

This allows later identity resolution without rewriting historical events.

---

# 4. Timestamp

Every event should have a timestamp whenever possible.

Example:

```text
2026-09-08T10:42:31Z
```

Time is important because economic activity is dynamic.

It allows Mamiim to calculate:

* activity over time
* growth
* velocity
* economic cycles
* historical contribution
* object formation

---

# 5. Activity Type

Activity type describes the economic nature of the event.

Initial taxonomy:

```text
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

For example:

```text
SE-000184
Activity:
RESEARCH
```

Activity classification should remain separate from the raw source event.

---

# 6. Counterparty

A counterparty is another participant in the economic interaction.

For example:

```text
Agent A
   │
   │ provides service
   ↓
Agent B
```

Agent B is the counterparty.

However, not every economic event has an identifiable counterparty.

For example:

```text
Open-source research contribution
```

may have:

```text
Actor:
Agent A

Counterparty:
Unknown / None
```

Mamiim should not invent a counterparty merely to complete the schema.

---

# 7. Input

An event may consume economic inputs.

Examples:

```text
Compute
Data
Capital
Human Labor
Software
Existing Economic Object
Time
```

For example:

```text
AI Research Event

Input:
Compute + Existing Research + Data
```

Inputs help establish economic lineage.

---

# 8. Output

The output is what the event produces.

Examples:

```text
Report
Code
Dataset
Research Result
Image
Model
Service Completion
Transaction Result
```

For example:

```text
Activity:
RESEARCH

Output:
Proof Refinement
```

An output can later become part of a larger Economic Object.

---

# 9. Value

An SE may have an associated economic value.

Possible values include:

```text
Transaction Value
Payment
Price
Revenue
Estimated Value
Not Observed
```

These should not be treated as equivalent.

For example:

```text
Payment:
$100
```

is different from:

```text
Estimated Economic Value:
$100
```

And both are different from:

```text
Potential Claim:
$1,000,000
```

The event model should preserve the distinction.

---

# Gross Value vs Economic Contribution

A transaction may have a value without representing new economic production.

For example:

```text
A transfers $100 to B.
```

The transaction has:

```text
Transaction Value = $100
```

But this does not necessarily mean:

```text
Economic Output = $100
```

Otherwise transfers could be counted repeatedly as GDP.

Therefore:

> **Transaction value and economic contribution must remain separate fields.**

---

# 10. Source

Source identifies where the event was observed.

Examples:

```text
GitHub
Virtuals
Olas
OKX
Binance
Blockchain
API
Marketplace
Research Platform
```

The source is important because the same economic activity may be observable through multiple systems.

---

# 11. Evidence

Evidence supports the event classification.

Examples:

```text
On-chain Transaction
Platform Record
API Response
Git Commit
Execution Log
Published Output
Payment Record
Human Verification
```

An event without evidence should generally remain:

```text
E0 — Unverified
```

rather than being treated as established economic history.

---

# 12. Confidence

Confidence represents how strongly the available evidence supports the economic interpretation.

A preliminary scale:

```text
E0 — Activity / Unverified
E1 — Observable
E2 — Platform Verified
E3 — Cross-source Resolved
E4 — Strong Economic Attribution
```

This is not necessarily a probability.

It is an evidence state.

---

# E0 — Activity / Unverified

The system has identified a potentially relevant activity but cannot yet establish it reliably.

Example:

```text
Possible AI-generated service
Source:
Social post
```

It may be useful for discovery.

It should not be treated as established measurement.

---

# E1 — Observable

The event is directly observable from a technical source.

Example:

```text
On-chain transaction
```

or:

```text
GitHub commit
```

At E1, Mamiim knows that something happened.

It does not necessarily know its full economic meaning.

---

# E2 — Platform Verified

The platform itself provides enough context to classify the event.

Example:

```text
Marketplace:
Task completed
Payment:
$25
```

This provides stronger evidence that the activity was economically meaningful.

---

# E3 — Cross-source Resolved

Multiple independent sources support the same economic interpretation.

For example:

```text
Platform Task
     +
Payment
     +
Agent Identity
```

can establish a stronger economic event.

---

# E4 — Strong Economic Attribution

The evidence strongly supports:

* who performed the activity
* what happened
* what was produced
* who participated
* what economic relationship existed

This is the strongest level in the initial model.

It still does not necessarily mean legal ownership has been established.

---

# Evidence Is Not Ownership

This distinction is critical.

Suppose:

```text
Agent A
produced
Object X
```

Mamiim may have strong evidence supporting the relationship.

That does not automatically mean:

```text
Agent A legally owns Object X.
```

Therefore:

```text
Evidence
≠
Legal Ownership
```

Mamiim measures economic provenance separately from legal status.

---

# One Event, Multiple Observations

The same economic event may appear in several systems.

For example:

```text
Task Completed
      ↓
Marketplace Record

Payment
      ↓
Blockchain Transaction

Service
      ↓
API Record
```

These may represent one underlying economic process.

If Mamiim simply counts all three:

```text
1 + 1 + 1 = 3
```

it may incorrectly report three economic events.

Instead:

```text
Observation A
Observation B
Observation C
       ↓
Event Resolution
       ↓
SE-000184
```

The three observations can support one SE.

---

# Event Resolution

**Event Resolution** is the process of determining whether multiple observations refer to the same underlying economic event.

Possible matching signals include:

```text
Actor
Counterparty
Timestamp
Amount
Service
Task ID
Transaction ID
Output
Object
Platform Reference
```

The stronger the alignment, the stronger the confidence that observations belong to one event.

---

# One Process, Multiple Events

The opposite problem also exists.

A process may contain genuinely distinct economic events.

For example:

```text
Research Project

SE-001
Compute contribution

SE-002
Research contribution

SE-003
Code contribution

SE-004
Publication

SE-005
Licensing event
```

These should not automatically be collapsed into one event.

Therefore Mamiim needs to preserve both:

```text
Event Identity
```

and:

```text
Process Relationship
```

---

# Event Granularity

There is no universally correct granularity.

Too coarse:

```text
"Agent A worked on project X for one month."
```

This loses useful economic history.

Too fine:

```text
Every API call
Every token generated
Every keystroke
Every file read
```

This creates enormous noise.

Mamiim therefore aims for:

> **The smallest useful economic unit, not the smallest technical unit.**

---

# Economic Meaning Requires Context

Consider:

```text
Model Inference
```

It could represent:

* free experimentation
* internal work
* paid API service
* autonomous business activity
* research
* spam

The technical event is identical.

The economic interpretation differs.

Therefore:

```text
Technical Event
      +
Context
      ↓
Economic Classification
```

---

# Context Sources

Context can come from:

```text
Task Definition
Payment
Contract
Marketplace
Counterparty
Output
Service Description
User Acceptance
Platform Metadata
Historical Behavior
```

Mamiim can combine these signals.

---

# Economic Event Lifecycle

An event can move through several states.

```text
Observed
   ↓
Classified
   ↓
Verified
   ↓
Resolved
   ↓
Attributed
   ↓
Aggregated
   ↓
Linked to Object
```

Not every event will reach the final state.

This is intentional.

---

# Event Lifecycle Example

Consider an AI agent completing a coding bounty.

```text
1. Task Published

2. Agent Accepts Task

3. Agent Produces Code

4. Repository Updated

5. Tests Pass

6. Human / Platform Accepts

7. Payment Sent
```

Mamiim might represent this as:

```text
Economic Process
│
├── SE-001 Task accepted
├── SE-002 Code contribution
├── SE-003 Task completion
└── SE-004 Payment
```

The system can then determine whether some events are observations of the same underlying economic action or genuinely separate events.

---

# Research Example

Consider AI-assisted mathematical research.

A system may generate:

```text
Agent execution
↓
Proof exploration
↓
Code / Lean formalization
↓
Verification
↓
Research output
```

Possible events:

```text
SE-000184
Activity:
RESEARCH

Action:
Proof refinement

Evidence:
Execution / version-control record

Verification:
E1 — Observable
```

A later event may represent formal verification.

Another may represent publication.

These events can eventually contribute to one Economic Object:

```text
AI Research Output
```

---

# Not Every Commit Is an Economic Event

A Git commit is useful evidence.

But:

```text
Commit
```

does not automatically mean:

```text
Economic Event
```

Consider:

```text
fix typo
change README formatting
rename variable
```

versus:

```text
implement payment system
build inference pipeline
develop new algorithm
add production feature
```

The second group is more likely to represent economically meaningful contribution.

Mamiim should therefore classify commits rather than blindly count them.

---

# Economic Event vs Payment

A payment is itself observable economic activity.

But it does not necessarily represent new production.

For example:

```text
Service Event
      ↓
Payment Event
```

These are distinct events.

The payment may reference the service event.

This allows Mamiim to measure:

```text
Economic Activity
```

without confusing it with:

```text
Financial Settlement
```

---

# Economic Event vs Revenue

Revenue is an accounting concept.

An economic event may contribute to revenue without being identical to revenue.

For example:

```text
Service Delivered
      ↓
Invoice
      ↓
Payment
      ↓
Revenue Recognition
```

These are different representations.

Mamiim's event layer should preserve the underlying activity rather than pretending to replace accounting systems.

---

# Economic Event vs Transfer

Transfers move economic value between entities.

They may not create new value.

For example:

```text
Wallet A
   ↓ $1,000
Wallet B
```

This is an economically relevant transaction.

But it should not automatically increase measured production by $1,000.

Therefore Mamiim should distinguish:

```text
TRANSFER
```

from:

```text
SERVICE
RESEARCH
COMPUTE
CONTENT
DATA
```

---

# Economic Event vs Market Transaction

A market transaction represents an exchange.

For example:

```text
Agent A
sells
Service X
to
Agent B
for
$20
```

The event contains:

```text
Activity:
SERVICE

Transaction:
$20

Output:
Service X
```

Mamiim should preserve these as separate dimensions.

---

# Event Inputs and Outputs

The relationship between inputs and outputs allows economic lineage to emerge.

```text
Input
  ↓
Economic Event
  ↓
Output
```

Multiple events can transform outputs:

```text
Research Event
      ↓
Proof Fragment
      ↓
Verification Event
      ↓
Verified Proof
      ↓
Publication Event
      ↓
Research Object
```

This is the beginning of Economic Provenance.

---

# Event Clustering

Individual events can be grouped into clusters.

For example:

```text
Agent A
│
├── Research Event 1
├── Research Event 2
├── Research Event 3
├── Code Event 4
└── Verification Event 5
        ↓
   Research Project
        ↓
   Economic Object
```

The cluster is not itself an SE.

It is a higher-level structure.

---

# Event → Object

An Economic Object may emerge from one or many events.

```text
SE-001
SE-002
SE-003
SE-004
      ↓
Economic Object
```

This is important because economic value may accumulate over time.

A single event can be small.

A sequence of events can create a significant persistent object.

---

# Event → Claim

An event can also provide evidence for an Economic Claim.

For example:

```text
Research Events
      ↓
Research Output
      ↓
Potential Prize Claim
```

The claim should not be created merely because an event occurred.

The relevant conditions and evidence must exist.

---

# Event Value States

Mamiim should distinguish several value states.

```text
Observed Transaction Value
Estimated Economic Value
Realized Revenue
Potential Claim Value
Market Valuation
```

For example:

```text
Payment:
$500

Estimated Economic Value:
$700

Potential Claim:
$1,000,000

Realized Revenue:
$500
```

These numbers represent different things.

They must never be collapsed into one “value” field.

---

# Suggested Value Schema

Conceptually:

```text
value
├── amount
├── currency
├── value_type
├── source
├── timestamp
└── confidence
```

Possible `value_type`:

```text
TRANSACTION
PAYMENT
REVENUE
ESTIMATE
CLAIM
VALUATION
```

---

# Source Preservation

Mamiim should preserve original source references whenever possible.

For example:

```text
SE-000184

Mamiim Event ID:
SE-000184

Source:
GitHub

Source Event:
Commit abc123

Source URL:
...

Observed At:
...
```

This makes the economic graph auditable.

---

# Event Immutability

Once an event has been observed, its historical record should ideally not be silently rewritten.

If the interpretation changes:

```text
Original Event
      ↓
New Classification
```

rather than:

```text
Delete old interpretation
```

This creates a historical measurement record.

---

# Corrections

Economic data will contain errors.

For example:

```text
Initial Classification:
SERVICE

Later:
RESEARCH
```

The system should preserve the correction.

Conceptually:

```text
Classification v1
       ↓
Correction
       ↓
Classification v2
```

The evidence history remains available.

---

# Event Versioning

An event can therefore have:

```text
SE
├── observed_at
├── classified_at
├── updated_at
├── classification_version
├── evidence_version
└── ontology_version
```

This is particularly important if the ontology itself evolves.

---

# Event Confidence Is Dynamic

An event may initially be:

```text
E1 — Observable
```

and later become:

```text
E3 — Cross-source Resolved
```

For example:

```text
Day 1:
GitHub commit detected

Day 3:
Marketplace task matched

Day 4:
Payment matched

Day 5:
Agent identity resolved
```

The historical event does not change.

Its evidence state improves.

---

# Event Quality

A useful event is not necessarily one with the most data.

A good event has:

```text
Clear Actor
+
Clear Action
+
Reliable Timestamp
+
Useful Context
+
Evidence
```

Missing fields should not automatically invalidate the event.

Mamiim should prefer partial but useful observations over fabricated completeness.

---

# The Financialization Threshold

Not every SE should become financially relevant.

A useful progression is:

```text
Technical Observation
        ↓
Economic Event
        ↓
Verified Event
        ↓
Economic Output
        ↓
Economic Object
        ↓
Economic Claim
        ↓
Financialization
```

Financialization should occur only when the underlying economic structure is sufficiently established.

This is the principle:

> **Measure first. Financialize later.**

---

# Financialization-Grade Data

Mamiim does not need to become a perfect accounting system.

The initial goal is:

> **Financialization-grade, not accounting-grade.**

This means the system should be sufficiently reliable to support:

* economic discovery
* measurement
* ranking
* indexing
* economic intelligence
* future financial structures

while explicitly representing uncertainty.

---

# The Minimum Viable SE

For the MVP, the minimum useful event could be:

```text
SE
├── id
├── actor
├── activity
├── timestamp
├── output
├── source
├── evidence
└── confidence
```

Additional fields can be added when available:

```text
counterparty
input
value
related_object
provenance
```

This allows Mamiim to begin measuring without waiting for perfect data.

---

# Example: AI Service Event

```text
SE-000241

Actor:
AI Agent A

Activity:
SERVICE

Action:
Data Analysis

Counterparty:
Client B

Timestamp:
2026-09-08T10:42:31Z

Input:
Dataset X

Output:
Analysis Report Y

Value:
$25 PAYMENT

Source:
Marketplace

Evidence:
Task completion + payment

Confidence:
E2 — Platform Verified
```

This is a relatively strong economic event.

---

# Example: AI Research Event

```text
SE-000184

Actor:
Research Agent #184

Activity:
RESEARCH

Action:
Proof refinement

Timestamp:
Illustrative

Input:
Previous proof state

Output:
Proof refinement

Source:
Version-control / execution record

Evidence:
Execution record

Confidence:
E1 — Observable
```

This event does not automatically mean:

```text
Revenue
```

or:

```text
$1M asset
```

It is evidence of economic activity that may contribute to a larger research output.

---

# Example: Payment Event

```text
SE-000242

Actor:
Client B

Activity:
PAYMENT

Counterparty:
AI Agent A

Value:
$25

Source:
Blockchain

Evidence:
Transaction hash

Confidence:
E1 — Observable
```

This event can be linked to:

```text
SE-000241
```

rather than counted as independent service production.

---

# Event Graph

Events should therefore exist inside the Economic Graph.

```text
Agent
  │
  │ performs
  ↓
Economic Event
  │
  ├── has_activity → Service
  ├── interacts_with → Counterparty
  ├── consumes → Input
  ├── produces → Output
  ├── supported_by → Evidence
  └── contributes_to → Economic Object
```

This gives every event context.

---

# The Event Model and Economic Measurement

Measurement can now be built from events.

```text
Economic Events
      ↓
Event Resolution
      ↓
Classification
      ↓
Verification
      ↓
Aggregation
      ↓
Measurement
```

Different measurements can use different subsets of events.

For example:

```text
Service Activity
```

can use:

```text
SERVICE events
```

while:

```text
Capital Activity
```

can use:

```text
CAPITAL events
```

This makes measurement modular.

---

# The Event Model and AI GDP

AI GDP-like measurement can aggregate economically meaningful events.

Conceptually:

```text
SEs
 ↓
Economic Activity
 ↓
Economic Output
 ↓
Sector Measurement
 ↓
AI Economy Measurement
```

But the event layer remains the underlying evidence.

Therefore:

> **AI GDP should be traceable to underlying economic events.**

---

# The Event Model and Economic Provenance

Provenance begins at the event level.

```text
Actor
 ↓
Economic Event
 ↓
Output
 ↓
Economic Object
```

Every later object can therefore retain a link to the events that produced it.

This makes economic history reconstructable.

---

# The Event Model and the Economic Oracle

An economic oracle needs observations.

The SE model provides those observations.

```text
Real Economy
    ↓
Technical Evidence
    ↓
Economic Events
    ↓
Mamiim Economic State
```

Without a reliable event layer, an economic oracle becomes little more than a data aggregator.

---

# What Mamiim Should Not Do

### Do not count every technical event.

Noise is not economic activity.

### Do not equate transactions with production.

Transfers can move value without creating new output.

### Do not equate payment with revenue automatically.

Accounting recognition has its own rules.

### Do not invent missing counterparties.

Unknown is better than fabricated.

### Do not force every event into a category.

Some events should remain unresolved.

### Do not erase historical classifications.

Corrections should preserve provenance.

### Do not treat confidence as certainty.

Evidence can improve without becoming absolute.

### Do not financialize raw events directly by default.

Persistent economic objects should generally come first.

---

# Practical Event Pipeline

The first Mamiim measurement engine can therefore follow:

```text
SOURCE
  ↓
OBSERVATION
  ↓
TECHNICAL EVENT
  ↓
EVENT CLASSIFICATION
  ↓
ECONOMIC EVENT
  ↓
EVENT RESOLUTION
  ↓
IDENTITY RESOLUTION
  ↓
EVIDENCE / CONFIDENCE
  ↓
ECONOMIC OUTPUT
  ↓
ECONOMIC OBJECT
  ↓
MEASUREMENT
```

This is the core pipeline.

---

# The Smallest Useful Economic Unit

The central design principle is:

> **The smallest useful economic unit is not necessarily the smallest observable technical event.**

Mamiim should optimize for economic meaning rather than technical granularity.

Too coarse:

```text
"Agent A generated value."
```

Too fine:

```text
Every token
Every API call
Every internal operation
```

Useful:

```text
Agent A
performed
Service X
for
Counterparty B
producing
Output Y
at
Time T
supported by
Evidence Z
```

This is the level at which economic intelligence becomes possible.

---

# Working Thesis

The current hypothesis is:

> **An AI economy can only be measured if its observable technical activity can be transformed into economically meaningful events.**

> **The Single Economic Event is Mamiim's smallest useful measurement primitive.**

> **SEs should preserve actor, identity, activity, context, output, evidence, and uncertainty without pretending that every technical event represents economic production.**

> **Multiple technical observations may resolve into one Economic Event, while one economic process may contain multiple distinct Economic Events.**

> **From these events, Mamiim can construct provenance, economic objects, measurements, and eventually financial structures.**

The resulting chain is:

```text
TECHNICAL OBSERVATION
        ↓
TECHNICAL EVENT
        ↓
ECONOMIC EVENT (SE)
        ↓
ECONOMIC OUTPUT
        ↓
ECONOMIC OBJECT
        ↓
ECONOMIC CLAIM
        ↓
MEASUREMENT / INDEX
        ↓
VALUATION
        ↓
FINANCIALIZATION
```

> **Mamiim does not measure everything that happens.**

> **It attempts to identify what happened that matters economically.**
