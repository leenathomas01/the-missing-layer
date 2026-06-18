# Waypoint: The Missing Layer Between Requirements and Implementation

## Status

Exploration waypoint only.

This is not a proposal, architecture, framework, or product design.

It is a record of an observed gap and several candidate directions.

---

## Origin

Investigation began while discussing:

* Agentic system bottlenecks
* Memory architectures
* State management
* Governance and verification

Unexpected conclusion:

The most interesting bottleneck may not be agent intelligence.

It may be the lack of a formal, reviewable, machine-comprehensible layer between business intent and implementation.

---

## Core Observation #1

Software engineering currently formalizes:

Requirements (partially)
↓
Implementation (strongly)

But relies heavily on humans for:

Requirements
↓
[ Human Interpretation ]
↓
Implementation

This interpretation layer is often carried by:

* Business Analysts
* Product Managers
* Architects
* Senior Developers
* QA
* Meetings
* Documentation
* Tribal knowledge

The layer exists.

It is simply not formally represented.

---

## Core Observation #2

Historically:

Code Generation Speed ≈ Code Review Speed

AI-assisted development changes this relationship:

Code Generation Speed >> Human Review Speed

Result:

Human attention becomes the scarce resource.

The bottleneck shifts from implementation generation to implementation review and verification.

---

## Core Observation #3

Many "hallucinations" may actually be:

Goal Drift
Constraint Failure
Scope Expansion
Over-engineering

rather than purely model intelligence failures.

This suggests that improving alignment to requirements may be as important as improving reasoning capability.

---

## Pivotal Question

How does a system continuously know what it is supposed to remain aligned to?

Or more generally:

How do we create a reviewable, traceable representation between intent and implementation?

---

## Candidate Missing Layer

Current:

Business Intent
↓
???
↓
Implementation

Hypothesis:

A missing abstraction layer may exist.

We do not know its final form.

Possible manifestations:

* Requirements Graphs
* Constraint Models
* Logic Blocks
* Semantic Change Representations
* Behavioral Diff Layers
* Traceability Graphs
* Something not yet invented

---

## Logic Block Hypothesis

One candidate implementation explored.

Goal:

Provide a review abstraction between requirements and raw code.

Concept:

Requirements
↓
Risk Classification
↓
Logic Blocks
↓
Code

Potential benefit:

Humans review:

* Intent
* State mutations
* Risk concentrations
* Critical assumptions

instead of reviewing thousands of generated lines.

Status:

Interesting hypothesis.

Unproven.

---

## Assumption-Centric Review

Key insight inspired by historical QA experience:

Elite reviewers often inspect assumptions rather than syntax.

Review focus becomes:

* What assumptions were introduced?
* What assumptions changed?
* What assumptions were removed?

Possible future artifact:

Assumption Diff

rather than only:

Code Diff

---

## Risk Classification Direction

Potential review model:

Risk =
Requirement Risk
+
Implementation Risk
+
Uncertainty Risk

Purpose:

Focus limited human attention on areas where judgment matters most.

---

## What Survives If AI Disappears?

Important sanity check.

The idea remains valuable even if:

* LLMs disappear
* Agents disappear
* New architectures replace current systems

Therefore the concept appears to be a software engineering problem rather than an AI-specific problem.

---

## Strongest Current Thesis

AI did not create this gap.

AI exposed it.

The software industry may have spent decades compensating for a missing abstraction layer using human interpretation and organizational process.

As generation velocity increases, that compensation becomes increasingly difficult to sustain.

---

## Open Research Questions

1. Is there truly a missing abstraction layer, or are we rediscovering existing requirements-engineering concepts?

2. What is the smallest useful representation between requirements and implementation?

3. Can requirements become continuously verifiable rather than static documents?

4. Can assumption tracking become a first-class engineering artifact?

5. How should human attention be allocated when generation becomes effectively unlimited?

6. What survives across:

   * Human developers
   * LLMs
   * Future synthesis systems

7. Is the future repository structure:

   Requirements
   ↓
   Semantic Layer
   ↓
   Code

or something fundamentally different?

---

## Guiding Principle

Do not become attached to any specific implementation.

Protect the question.

The question appears more durable than any current answer.
