# DocStable

**Know before you migrate.**

DocStable is a deterministic, offline analysis tool designed to assess the migration risks of Microsoft Office documents before transitioning to alternative office environments.

Instead of relying on cloud services or opaque AI systems, DocStable analyzes documents locally and produces clear, explainable findings and risk scores.

The goal is simple: **reduce uncertainty before large-scale Office migrations.**

---

## Why DocStable Exists

Office migrations rarely fail because of the migration tools themselves.

They fail because organizations do not fully understand the structure and complexity of their existing document landscape.

Hidden issues may include:

- macros and automation code
- external references
- unsupported document structures
- complex formatting constructs
- embedded objects

DocStable exposes these risks **before migration decisions are made**.

---

## Key Principles

DocStable follows a few strict design principles:

**Deterministic analysis**  
Given the same input and the same version of DocStable, the results are always identical.

**Fully offline operation**  
No cloud connection is required. All analysis happens locally.

**Transparent findings**  
Every finding can be explained and traced back to the document structure.

**Decision support, not automation magic**  
DocStable does not attempt to automatically "fix" documents.  
It provides the information needed to make informed decisions.

---

## What DocStable Analyzes

DocStable currently supports analysis of modern Microsoft Office formats:

- Word (`.docx`)
- Excel (`.xlsx`)
- PowerPoint (`.pptx`)

These formats are ZIP-based OpenXML containers and can be deterministically inspected without requiring Microsoft Office to be installed.

DocStable extracts structural information from the document packages and evaluates it using a set of deterministic rules.

---

## Findings and Risk Scoring

Each analyzed document produces a list of **Findings**.

Examples include:

- macro presence
- complex layout structures
- unsupported elements for alternative office suites
- external dependencies

Findings are aggregated into a **Risk Score**, which maps to a simple traffic-light system:

| Level | Meaning |
|------|--------|
| 🟢 Green | Low migration risk |
| 🟡 Yellow | Medium migration risk |
| 🔴 Red | High migration risk |

The goal is not perfect prediction, but **early visibility of potential migration blockers**.

---

## Reporting

DocStable generates structured reports that allow teams to:

- understand the overall document landscape
- identify migration-critical documents
- prioritize remediation work
- communicate risks to decision makers

Reports can be exported and integrated into migration planning workflows.

---

## Typical Use Cases

DocStable is designed for:

- Office migration projects
- digital sovereignty initiatives
- public sector IT modernization
- enterprise document landscape analysis
- migration planning and risk assessment

It is **not a document converter** and **not a document editor**.

It is a **decision support tool**.

---

## Architecture Overview

DocStable is intentionally simple:

- local desktop application
- deterministic analysis engine
- rule-based findings system
- transparent scoring model

No cloud services are involved.

This ensures:

- reproducibility
- privacy
- predictable behavior

---

## Status

DocStable is currently in **early access evaluation phase**.

The current version focuses on the core analysis engine and reporting capabilities.

Future versions may introduce additional analysis rules and visualization features.

---

## Licensing

DocStable is **commercial software**.

The source code is not open source.

Evaluation versions may be provided for testing and assessment purposes.

---

## Disclaimer

DocStable is an analysis and decision-support tool.

The software analyzes document structures and produces findings and risk scores based on deterministic rules.  
While the analysis is designed to highlight potential migration risks, the results do not constitute a guarantee of successful document conversion or migration.

Migration outcomes may depend on many external factors, including but not limited to:

- document complexity
- external dependencies
- macros and automation code
- software compatibility
- target office environments

DocStable provides transparency and guidance, but final decisions and actions remain the responsibility of the user.

The software is provided **"AS IS"**, without any warranty of any kind.

---

## Website

More information: https://www.doc-stable.com/

---

## Copyright
Copyright © 2026 DocStable & Ralph Dietrich.
