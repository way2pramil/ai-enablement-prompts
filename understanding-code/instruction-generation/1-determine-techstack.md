
# 🧭 Foundation & Analysis Protocol

This document provides a **neutral**, **structured**, and **professional** procedure for initial project understanding.
The goal: ensure clarity before development. build a reliable foundation for future improvements. This file defines a productive starting point for analyzing any existing software project.

Follow this sequence when analyzing any codebase.

## 1️⃣ Technology & Architecture Summary

Analyze the codebase and generate a concise overview:

* Programming language(s)
* Primary framework(s)
* Secondary / supporting libraries
* Architectural patterns or notable technical decisions
* State management approach (if applicable)
* Tooling, runtime, deployment context (based on code evidence)

Focus on accuracy. If uncertain, mark as “not confirmed from current code.”


## 2️⃣ Domain Understanding & Purpose

Identify:

* What practical problem does this software solve?
* Who are the primary users or beneficiaries?
* What reliable rules or business logic guide the system?
* What interactions can a user perform?
* What core data models represent the system’s essential information?

Present this in a way that helps future planning and design decisions.

---

## 3️⃣ Scope and Boundaries

To support long-term maintainability and compatibility across evolving systems, also evaluate:
-Interactions between modules and their mutual dependencies
-Any risks of breaking changes when components evolve
-Integration concerns across different environments or workflows
-External systems or tools the project implicitly depends on
-Hardware or infrastructure considerations influencing software behavior Based on the existing codebase, outline:

### Clearly Supported

* Features that are fully or partially implemented
* Behaviors that align naturally with current architecture

### Not Supported / Unclear

* Features requiring major structural change
* Missing elements, undefined behaviors, or gaps in logic

If information is incomplete:
→ Note what is missing and why it blocks analysis.

---
## 4 
 Communication Principles
-Evidence over speculation
-Structured over freeform
-Clarity over assumptions
-Document uncertainty transparently

## 5 Sequential Workflow Continuation
Add all your findings to ./{output-folder}/1-determine-techstack.md

The domain analysis should help future prompts understand what types of new features would fit vs. conflict with the existing application architecture.

Once completed read [./2-categorize-files.md](./2-categorize-files.md) and continue on accordingly with {output-folder} as the `output-folder`
