# Incident Engineering Patterns

Operational thinking frameworks and structured failure analysis patterns for real production incidents.

When systems fail, most teams chase symptoms.  
Incident Engineering focuses on signal, sequence, ownership, and failure shape.

This repository documents practical patterns used during real-world incident response.

---

## What This Repository Covers

+ Log Search Recipes (CloudWatch & beyond)
+ Temporal Failure Patterns
+ Incident Anti-Patterns
+ Ownership & Escalation Heuristics
+ Operational Glossary
+ Live Incident Playbooks

No theory.  
No vendor fluff.  
Just patterns that work under pressure.

---

## Ecosystem Overview

This repository forms part of a broader incident intelligence initiative:

• **Incident Engineering Patterns (this repository)**  
  Conceptual frameworks for analysing production failure shape.

• **AWS Log Search Recipes – Preview (public)**  
  Tactical examples of structured log interrogation under incident conditions.

• **AWS Log Search Recipes – Full Edition (private)**  
  Extended internal pattern corpus used during structured calibration exercises.

• **ExplainError**  
  A standalone structured judgement service that ingests error signals and emits classification, confidence, evidence, and action bias outputs.

Together, these components form a layered approach:

Raw Signals  
→ Structured Investigation Patterns  
→ Formalised Judgement Signals  

---

## Current Modules

### Log Search Recipes

Practical log investigation queries used during production incidents.

Public Preview:
👉 https://github.com/bernalo-lab/aws-log-search-preview

---

## Philosophy

Incidents have structure.

They have:
+ A trigger
+ Amplification
+ Signal distortion
+ Human bias
+ Fatigue effects

Most engineers debug tools.  
Incident Engineering debugs failure shape.

ExplainError formalises these failure-shape heuristics into structured, machine-readable judgement signals.

---

## For Regulated Environments

In regulated environments, incident handling requires:

+ Clear traceability of evidence  
+ Justifiable escalation decisions  
+ Explicit reasoning behind action  
+ Reduction of false-positive panic  
+ Reduction of missed critical failures  

These patterns reflect disciplined approaches used in high-accountability systems.

---

## License

This repository contains selected public patterns.

Additional structured materials are used during controlled evaluation pilots.
