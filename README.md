# ESG, Carbon Accounting & Sustainability Reporting Portfolio

I use sustainability data to move from **measurement and data validation to disclosure, reporting, and management action**.

This portfolio brings together applied projects in greenhouse-gas accounting, ESG data quality, sustainability disclosure, reporting readiness, climate evidence analysis, and AI-assisted reporting workflows.

Across the projects, the common objective is not simply to produce an ESG metric or a report. It is to make the underlying data and evidence **traceable, reviewable, and useful for decision-making**.

## Reporting Workflow

**Data Collection → QA/QC → GHG & ESG Metrics → Framework Mapping → Evidence Review → Reporting → Management Action**

---

## Portfolio at a Glance

| Project | Primary Question | Methods / Tools | Current Status |
|---|---|---|---|
| [AI-Powered IFRS S2 Evidence & Gap Analysis](https://github.com/haveisi/AI-Powered-IFRS-S2-Requirement-Mapping-Evidence-Gap-Analysis) | How can AI help analysts find and organize climate-disclosure evidence while preserving human judgment? | Python, LlamaIndex, Pydantic, semantic retrieval, human-in-the-loop review | Applied disclosure-analysis pilot |
| [Scope 3 & Regenerative Agriculture Analytics](https://github.com/haveisi/04_scope3_regenerative_agriculture) | How can operational and agricultural emissions be translated into hotspots and reduction scenarios? | Python, GHG accounting, Streamlit, scenario analysis | Simplified GHG screening model |
| [Real Estate ESG & GRESB Readiness](https://github.com/haveisi/real-estate-carbon-benchmarking-gresb-analytics) | How can utility, emissions, benchmark, climate-risk, and evidence data be structured for ESG reporting readiness? | Python, Excel, ESG data QA, GRESB-style evidence review | Applied reporting-readiness case |
| [Climate Action Plan Analytics](https://github.com/haveisi/climate-action-plan-analytics) | How can unstructured climate plans be converted into structured and auditable analytical data? | AI-assisted extraction, JSON schemas, validation, deterministic scoring | Applied climate-policy analytics case |

---

# Featured Projects

## 1. AI-Powered IFRS S2 Requirement Mapping & Evidence Gap Analysis

**Climate disclosure | IFRS S2 | Evidence traceability | Python | LlamaIndex | Human-in-the-loop AI**

[View repository →](https://github.com/haveisi/AI-Powered-IFRS-S2-Requirement-Mapping-Evidence-Gap-Analysis)

I built this project around a practical sustainability-reporting question:

> **Can AI help analysts find and organize the right disclosure evidence while keeping the final assessment with a human reviewer?**

The workflow uses publicly available sustainability and climate disclosures as source material and combines:

**Document extraction → keyword and semantic retrieval → structured evidence extraction → schema validation → quotation validation → human review → IFRS S2 mapping → gap analysis → management action**

The pilot focuses on selected IFRS S2 climate-related disclosure areas, including governance, climate resilience, Scope 1 emissions, Scope 2 emissions, and climate-related targets.

A central design principle is that the AI assists with **evidence discovery and organization**, rather than making an autonomous compliance determination.

The workflow also distinguishes between three different questions:

**Is relevant evidence present?**

**Does the evidence address the disclosure requirement?**

**What remains incomplete or requires additional action?**

**What this project demonstrates:** AI can make sustainability-reporting review more efficient, but reliable disclosure analysis still requires requirement-level interpretation, source traceability, deterministic controls, and human judgment.

**Study status:** Applied portfolio pilot. It is not an audit, assurance engagement, legal opinion, or determination of compliance with IFRS Sustainability Disclosure Standards.

---

## 2. Scope 3 & Regenerative Agriculture Analytics

**Agriculture | GHG accounting | Operational + farm emissions | Python | Streamlit | Scenario analysis**

[View repository →](https://github.com/haveisi/04_scope3_regenerative_agriculture)

This project explores how greenhouse-gas data can move from **emissions measurement to hotspot identification and reduction planning**.

The model evaluates operational and agricultural emissions including:

- stationary and mobile fuel use
- purchased electricity
- fertilizer-related emissions
- agricultural inputs and field operations
- production-based emissions intensity
- regenerative-agriculture scenarios

The workflow then tests how changes in fertilizer use and agricultural practices affect emissions intensity and cost-emissions tradeoffs.

An interactive Streamlit dashboard provides a management-facing view of emissions sources and scenario outcomes.

The model explicitly separates modeled soil-carbon effects from operational Scope 1 emissions rather than automatically netting them together.

**What this project demonstrates:** GHG accounting becomes more decision-useful when emissions totals are connected to hotspots, operational drivers, and reduction scenarios.

**Study status:** Simplified analytical model developed for portfolio and learning purposes. It is not presented as a complete GHG Protocol-compliant corporate inventory.

---

## 3. Real Estate ESG & GRESB Readiness Analytics

**Real estate | Energy | Water | Waste | Emissions | ESG evidence | Python | Excel**

[View repository →](https://github.com/haveisi/real-estate-carbon-benchmarking-gresb-analytics)

I built this project around a fundamental ESG reporting problem:

> **Before sustainability data can support benchmarking or disclosure, how do we know whether the underlying information is complete, structured, and usable?**

The analytical workbook brings together:

- property and asset information
- monthly energy consumption
- water consumption
- waste data
- emissions factors
- performance benchmarks
- climate-risk indicators
- environmental-justice context
- retrofit options
- GRESB-style evidence checklist information

Python is used to inspect workbook structure, standardize fields, review benchmark data, summarize evidence categories, and generate reporting-ready tables and charts.

The emphasis is on the foundation of ESG reporting:

**Data structure → validation → performance metrics → evidence readiness → reporting**

**What this project demonstrates:** ESG reporting quality depends as much on the underlying controls, traceability, and data structure as it does on the final report or dashboard.

**Study status:** Multifamily-focused ESG readiness and building-performance analytics case. It is not presented as a formal GRESB submission.

---

## 4. Climate Action Plan Analytics

**Climate disclosure & policy | AI-assisted extraction | Structured data | Validation | Benchmarking**

[View repository →](https://github.com/haveisi/climate-action-plan-analytics)

Climate action plans contain large amounts of qualitative and quantitative information, but that information is often difficult to compare systematically.

This project develops an AI-assisted workflow for converting unstructured climate-plan documents into structured analytical datasets.

The workflow follows:

**Source document → schema-constrained extraction → structured JSON → validation → aggregation → deterministic analysis**

A key methodological rule is:

> **If information is not explicitly present in the source document, it should not be generated as though it were reported evidence.**

This approach separates AI-based document extraction from deterministic analytical scoring and helps reduce unsupported interpretation.

**What this project demonstrates:** AI-assisted ESG and climate analysis becomes more defensible when source extraction, evidence validation, analytical scoring, and interpretation are treated as separate steps.

---

# How I Think About Sustainability Reporting

I treat sustainability reporting as a **data, evidence, and governance process**, not simply a report-writing exercise.

A decision-useful reporting system should be able to answer five questions:

1. **Where did the information come from?**
2. **How was it calculated or derived?**
3. **What controls were applied before the information was accepted?**
4. **Which disclosure requirement or management question does it address?**
5. **What remains incomplete, uncertain, or actionable?**

My working approach is:

**Measure → Validate → Map → Review → Report → Act**

This distinction matters because the same sustainability information may serve different purposes.

A calculation suitable for internal screening may not yet be sufficiently documented for external disclosure. A disclosure may contain relevant information without fully satisfying a reporting requirement. And more evidence does not automatically mean better evidence.

---

# Data & Evidence Governance

Across the portfolio, I try to make the status of information visible rather than treating every input as equally reliable.

Depending on the project, inputs may be identified as:

**Reported** — directly supported by a public or documented source  
**Calculated** — derived from transparent calculations  
**Modeled** — generated through scenario or analytical modeling  
**Assumed** — introduced where information is unavailable  
**Proxy** — used as a substitute where direct information is unavailable

This distinction helps prevent assumptions from being presented as reported company information and makes analytical limitations easier to evaluate.

---

# Frameworks & Methodological Context

The projects draw on sustainability and climate-reporting concepts including:

- GHG accounting and Scope 1–3 concepts
- IFRS S2 climate-related disclosure requirements
- sustainability disclosure evidence mapping
- ESG data-quality and reporting controls
- GRESB-style real-estate reporting readiness
- climate-action-plan evaluation
- scenario analysis
- source traceability and evidence validation
- human-in-the-loop AI-assisted analysis

References to reporting frameworks indicate the methodological context used in a project. They should not be interpreted as certification, assurance, or formal compliance unless explicitly stated.

---

# Technology & Analytics

**Data & analytics:** Python, pandas, Excel, SQL  
**Visualization & reporting:** Power BI, Streamlit  
**AI-assisted analysis:** LlamaIndex, semantic retrieval, structured extraction, Pydantic validation, human review  
**Sustainability analytics:** GHG accounting, emissions-intensity analysis, ESG metrics, disclosure mapping, reporting-readiness assessment  
**Data controls:** QA/QC, schema validation, reconciliation, evidence traceability

---

# From Reporting to Decision Support

My interest is not limited to producing sustainability metrics.

The broader analytical progression I work toward is:

**ESG Data  
→ Reliable Metrics  
→ Disclosure  
→ Hotspot Identification  
→ Reduction Opportunity  
→ Scenario Analysis  
→ Management Decision**

This ESG and reporting portfolio therefore connects with my related work in:

### Life Cycle Assessment & Product Sustainability

Product LCA, EPD methodology, packaging, carbon intensity, materials, agriculture, and aquaculture.

[View Life Cycle Assessment Portfolio →](https://github.com/haveisi/life-cycle-assessment-portfolio)

### Climate, Decarbonization & Sustainability Finance

Climate risk, emissions-reduction scenarios, capital planning, NPV, IRR, marginal abatement cost, transition risk, and financially informed decarbonization.

*Portfolio under development.*

---

# About

My work sits at the intersection of **sustainability reporting, carbon accounting, environmental analytics, and decision support**.

Across these projects, the recurring objective is to make sustainability information more **traceable, defensible, and useful**—from the underlying data and evidence through reporting and ultimately into management decisions.
