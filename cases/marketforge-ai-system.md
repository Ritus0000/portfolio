# MarketForge / PRACA2 — AI Opportunity Discovery System

## One-Sentence Summary

MarketForge is an evidence-first AI system for discovering, reviewing and tracking professional opportunities by work-mechanics similarity, not just by job titles.

It is not a generic job-search scraper and not a chatbot wrapper. It is a closed-loop decision system: user intent becomes search strategy, sources become evidence, evidence is reviewed against candidate memory, human decisions are recorded, applications are prepared, and real responses feed the next search cycle.

## 30-Second Scan

- **Problem:** classic job search fails when the target profile is specific, interdisciplinary and not captured by simple role names.
- **Core idea:** compare opportunities to the actual mechanics of work: synthetic data, 3D simulation, computer vision datasets, rendering pipelines, spatial reasoning and product prototyping.
- **System type:** discovery engine + evidence pipeline + candidate memory + local semantic review + application tracker.
- **Design principle:** preserve raw evidence before interpretation.
- **Product loop:** intent -> evidence -> decision -> application -> response -> better next search.

## Product Flow

```text
User intent
↓
Search Brief Builder
↓
Search Generator
↓
DeepDiscovery
↓
Job Intake
↓
Raw Evidence Store
↓
Candidate Memory
↓
Local Semantic Review
↓
Human Decision
↓
Application Tracker
↓
Gmail / response feedback
↓
Better next search
```

## Why I Built It

My target profile is not well described by one clean label such as "AI engineer", "3D artist" or "data scientist".

A more accurate description is a work pattern:

```text
realistic 3D simulation
↓
synthetic visual data
↓
computer-vision-ready outputs
↓
spatial / visual reasoning
↓
practical AI product context
```

Normal job boards search titles. MarketForge searches for similarity between this work pattern and the real work described in opportunities.

## System Architecture

| Layer | Role in the system | Why it matters |
| --- | --- | --- |
| Search Brief Builder | Turns a vague user direction into structured search intent, query seeds, source preferences and constraints. | The user remains involved when the search direction changes. |
| Search Generator | Builds query strategies, source routes and retrieval plans. | The system does not depend on one fixed search phrase. |
| DeepDiscovery | Collects evidence from job boards, company pages, career pages, ATS systems and manual sources. | The system preserves the original source context. |
| Job Intake | Stores raw job text first, extracts factual metadata and creates semantic chunks. | Extraction failure is treated as a data-quality issue, not as low relevance. |
| Candidate Memory | Holds structured candidate context: experience, capabilities, evidence, tools, constraints and target domains. | Matching is candidate-aware instead of generic. |
| Semantic Review | Reviews opportunities against work mechanics and asks what needs manual checking. | The system avoids fake numeric certainty. |
| Application Tracker | Connects decision, application draft, status, Gmail events and follow-up history. | The loop continues after the application, not only until the Apply button. |

## Core Design Principles

- preserve raw source text before interpretation
- rank by work-mechanics similarity, not only title or industry
- keep uncertainty visible instead of inventing fake match percentages
- treat missing information as a manual-check flag
- use local models where possible
- ask the user before expanding into a new search direction
- connect search results with application outcomes

## Local-First AI Direction

The system is designed around local reasoning where possible:

| Component | Role |
| --- | --- |
| Local embedding model | Semantic retrieval and similarity search over candidate context and job evidence. |
| Local reasoning model | Candidate-aware review, explanation and manual-check generation. |
| Fallback local model | Lightweight review or backup reasoning when needed. |
| External providers | Optional and explicit; used only when the task justifies it. |

This matters because the product is dealing with personal career context, application drafts and private opportunity history. Local-first reasoning keeps the system closer to a personal intelligence tool than a generic cloud workflow.

## What The System Produces

For each opportunity, the goal is not just to say "good" or "bad".

A useful review should produce:

- what the role appears to actually involve
- which parts match the candidate's real work mechanics
- what evidence supports the match
- what is missing or needs manual checking
- what kind of application angle makes sense
- whether the opportunity should be applied to, saved, watched or rejected
- how the outcome should influence future search directions

## What This Proves

MarketForge shows how I think about AI products:

- not as a chatbot layer, but as a system with memory, evidence and decisions
- not as one prompt, but as a modular pipeline
- not as pure automation, but as human-in-the-loop intelligence
- not as generic ranking, but as context-aware semantic review
- not as a one-way search tool, but as a feedback system

## Transfer to AI Product Work

The transferable pattern is:

```text
vague real-world intent
↓
structured brief
↓
source discovery
↓
raw evidence
↓
semantic interpretation
↓
user decision
↓
feedback loop
```

This is relevant far beyond job search. The same product logic can be applied to architecture, real estate, retail layout, spatial planning, research discovery, digital twins and other domains where the system must preserve evidence, compare alternatives and support a practical decision.

## Public Scope

This public case study does not include private email data, real application logs, API keys, private candidate profile files or personal job-search records.

The final visual version of this case should use real sanitized product screenshots, not generated interface mockups.
