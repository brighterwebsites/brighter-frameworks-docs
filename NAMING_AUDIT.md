# Naming Inconsistencies Found

## Issue 1: Content vs Post
- **Found in:** CAR discussions, ALTC Framework
- **Problem:** "Content Architecture Record" but "per post"
- **Resolution:** TBD
- **Affects:** CAR schema, documentation

## Issue 2: SCOS vs Site Essentials
- **Found in:** Business context, refactor plan
- **Problem:** SCOS = category, Site Essentials = product name?
- **Resolution:** TBD
- **Affects:** All marketing materials, code namespace

## Issue 3: [List others as you find them]**Day 3: Create GLOSSARY.md**

This becomes your **canonical terminology reference**:

# Framework Glossary

## Canonical Terms

### SCOS (Strategic Content Operating System)
- **Definition:** Category of software that operationalizes content strategy frameworks
- **Type:** Software category (like "CMS" or "CRM")
- **Not:** A brand name
- **Related:** Site Essentials (the actual product implementation)

### Site Essentials
- **Definition:** The WordPress MU plugin that implements SCOS principles
- **Type:** Product name
- **Namespace:** `SiteEssentials\`
- **Status:** Working name (marketing brand TBD)

### ALTC Framework
- **Full Name:** Authority-Led Topic Clusters Framework
- **Definition:** Content strategy methodology prioritizing positioning over keywords
- **Type:** Strategic framework
- **Status:** Proprietary, trademark pending

### WFB (Website-First Blueprint)
- **Full Name:** Website-First Blueprint
- **Definition:** Digital marketing philosophy positioning website as core asset
- **Type:** Methodology (less defined than ALTC)
- **Status:** Implied methodology, needs formalization

### CAR (Content Architecture Record)
- **Full Name:** Content Architecture Record
- **Definition:** Machine-readable metadata stored per post declaring strategic purpose
- **Storage:** Post meta (per post/page)
- **Format:** JSON
- **Status:** Needs specification

### CAM (Content Authority Map)
- **Full Name:** Content Authority Map
- **Definition:** Site-wide intelligence layer tracking authority signals over time
- **Storage:** Custom table or wp_options
- **Format:** TBD
- **Status:** Needs specification

### Proof Library
- **Definition:** Centralized repository of atomic, verifiable claims with temporal tracking
- **Storage:** Custom table
- **Format:** Structured data (claims + evidence + timestamps)
- **Status:** Needs specification ⭐ START HERE

### Authority Anchors
- **Definition:** The 8 mechanisms that prove expertise (Trust & Proof, Process & Education, etc.)
- **Count:** 8 anchors
- **Type:** Content classification framework
- **Part of:** ALTC Framework

### LLM.txt
- **Definition:** Site-level file declaring authority and providing AI context
- **Location:** `/llm.txt` (site root)
- **Standard:** Emerging (like robots.txt)
- **Status:** Needs format specification

## Naming Conventions

### Code
- PHP Namespace: `SiteEssentials\`
- Class names: `PascalCase`
- Functions: `snake_case`
- Constants: `SCREAMING_SNAKE_CASE`

### Documentation
- Framework names: Title Case (ALTC Framework)
- Acronyms: ALL CAPS (CAR, CAM, SCOS)
- File names: kebab-case with extension (.md)

### Database
- Tables: `wp_prefix_se_` (e.g., `wp_se_proof_library`)
- Options: `site_essentials_` prefix
- Post meta: `_se_` prefix
- Transients: `se_` prefix

## Decision Log

### [Date] - SCOS vs Site Essentials
**Decision:** SCOS = category, Site Essentials = product
**Reason:** Allows for category creation separate from brand
**Updated:** Business context docs, README files

### [Date] - CAR naming
**Decision:** Content Architecture Record (not "Post Architecture Record")
**Reason:** Can apply to pages, CPTs, not just posts
**Updated:** TBD---

## Why Start with Proof Library

**Your instinct is correct. Here's why:**

### Dependency Chain
