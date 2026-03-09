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

## Incident Investigation Toolkit

  Start here if you are responding to a production incident.
  These resources summarise investigation patterns used by experienced engineers when analysing system failures

• **2AM Incident Investigation Cheat Sheet**  
  A rapid decision framework for investigating production incidents under pressure.
  Instead of reading thousands of log lines, engineers follow a structured sequence of focused searches to quickly identify the earliest failure signal and narrow the investigation scope.

  Designed to reduce hesitation during on-call situations and accelerate the first critical minutes of incident response.

• **AWS Incident Nightmares (Failure Patterns)**  
  A collection of recurring failure scenarios frequently observed in AWS production systems.
  These patterns highlight incidents that are commonly misdiagnosed, such as retry amplification loops, dependency outages, and  partial deployments.

  Recognising these failure shapes early helps engineers avoid chasing symptoms and focus on the underlying cause.

  Designed to reduce hesitation during on-call situations and accelerate the first critical minutes of incident response.

• **Practical Incident Investigation Playbook**  
  A step-by-step walkthrough of how engineers investigate a real production incident using structured log searches.
The playbook demonstrates how a small number of targeted queries can quickly reveal the origin, scope, and likely cause of a system failure.

Designed to bridge the gap between theory and real operational practice.

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
