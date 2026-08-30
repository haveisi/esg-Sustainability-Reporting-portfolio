# ESG, Carbon Accounting & Sustainability Reporting Portfolio

I work with sustainability data to make reporting more reliable, traceable, and useful for decisions.

My projects focus on the part of ESG work that often gets overlooked: the systems behind the final report.

That includes:

- collecting and organizing sustainability data;
- checking data quality and resolving inconsistencies;
- calculating and reviewing GHG and ESG metrics;
- connecting reported information to source evidence;
- building dashboards and reporting workflows;
- using AI carefully for evidence review and disclosure analysis;
- connecting ESG information with operational issues, risks, and improvement actions.

My working approach is:

**Source Data → QA/QC → Reliable Metrics → Evidence → Reporting → Hotspots / Risk → Action**

---

## Portfolio at a Glance

| Project | What I Worked On | Tools / Methods |
|---|---|---|
| [**Mercy Corps Climate Reporting & Power BI Rebuild**](https://github.com/mercycorps/Climate-Report) | Multi-country GHG reporting, validation, data flows, Power BI, reporting controls | GHG Protocol, Excel, SharePoint, Power Automate, Microsoft Fabric, Power BI |
| [**ESG–EHS Decision Intelligence & FP&A**](https://github.com/haveisi/esg-ehs-fpa-decision-intelligence) | Connecting ESG performance with EHS risk, CAPA, improvement projects, and financial decisions | Databricks, SQL, Python, Power BI, DAX, ESG/EHS, FP&A |
| [**AI-Powered IFRS S2 Evidence & Gap Analysis**](https://github.com/haveisi/AI-Powered-IFRS-S2-Requirement-Mapping-Evidence-Gap-Analysis) | Climate-disclosure evidence review and gap analysis with human oversight | Python, LlamaIndex, Pydantic, semantic retrieval, human-in-the-loop review |
| [**Scope 3 & Regenerative Agriculture Analytics**](https://github.com/haveisi/04_scope3_regenerative_agriculture) | GHG hotspots, agricultural emissions, and reduction scenarios | Python, GHG accounting, Streamlit, scenario analysis |
| [**Real Estate ESG & GRESB Readiness**](https://github.com/haveisi/real-estate-carbon-benchmarking-gresb-analytics) | Energy, water, waste, emissions, benchmarking, and ESG evidence readiness | Python, Excel, ESG data QA/QC, GRESB-style review |

---

# 1. Mercy Corps Climate Reporting & Power BI Rebuild

**GHG accounting | Scope 1–3 | Data quality | Microsoft Fabric | Power BI | SharePoint | Power Automate**

[View repository →](https://github.com/mercycorps/Climate-Report)

This is the strongest example in this portfolio of working with a real organizational sustainability-reporting system.

I supported a rebuild of a multi-country carbon-reporting workflow covering:

- more than **40 countries**;
- **7 reporting years**;
- more than **15,000 records**;
- Scope 1, Scope 2, and selected Scope 3 emissions data.

The main challenge was not simply producing an emissions total.

The bigger issue was making sure the information entering the reporting process was complete, consistent, reviewable, and traceable.

## Reporting flow

**Microsoft Forms  
→ Excel staging  
→ validation and issue review  
→ SharePoint / Power Automate  
→ Microsoft Fabric Lakehouse / Delta  
→ Power BI**

My work included:

- reviewing country, office, fiscal year, scope, category, and emissions fields;
- creating validation rules and review flags;
- identifying missing or inconsistent records;
- standardizing office and country information;
- documenting QA/QC logic;
- checking curated reporting tables;
- supporting SharePoint-based source and refresh workflows;
- building Power BI views for executive reporting, operational review, trends, and data validation.

One of the most useful parts of the dashboard was not the executive summary.

It was the **validation layer**, because it made questionable records visible before they were accepted into reporting.

This project reinforced a simple lesson for me:

> A sustainability dashboard is only as reliable as the data controls behind it.

---

# 2. ESG–EHS Decision Intelligence & FP&A

**Timken public reporting case**

**ESG | EHS | Risk | CAPA | Databricks | SQL | Power BI | DAX | FP&A**

[View repository →](https://github.com/haveisi/esg-ehs-fpa-decision-intelligence)

I developed this project to explore what can happen **after ESG reporting**.

A sustainability report can show trends in emissions, energy, water, and waste.

But management still has to answer other questions:

- Where are the operational risks?
- What needs corrective action?
- Which improvement projects should be prioritized?
- Which projects create both environmental and financial value?
- Which actions may still be necessary even when the NPV is weak?

I used public Timken sustainability reporting as the corporate evidence base and then built a clearly labeled synthetic facility-level layer for EHS, risk, CAPA, and project-finance analysis.

## Analytical flow

**Public ESG evidence  
→ environmental KPIs  
→ EHS indicators  
→ facility hotspot  
→ risk  
→ CAPA  
→ improvement project  
→ financial analysis  
→ management priority**

The environmental layer includes:

- Scope 1 and Scope 2 emissions;
- energy use;
- renewable-energy share;
- water;
- waste;
- waste diversion.

The EHS demonstration layer includes:

- TRIR;
- LTIR;
- Good Catch activity;
- residual risk;
- open and overdue CAPA;
- facility-level hotspots.

The project layer adds:

- CAPEX;
- annual savings;
- carbon reduction;
- risk reduction;
- payback;
- NPV;
- simplified marginal abatement cost.

## Data architecture

I structured the project using a Databricks medallion approach:

**Bronze → Silver → Gold → Power BI**

Bronze stores source evidence and extracted information.

Silver organizes reviewed ESG metrics and modeled EHS / project information.

Gold creates KPI, risk, CAPA, and project-decision tables for Power BI.

## Why I included EHS here

I do not see EHS as the main theme of this portfolio.

I see it as one of the operational systems that can make ESG information more actionable.

For example:

**EHS observation  
→ risk  
→ corrective action  
→ project  
→ cost / benefit  
→ management decision**

That connection is useful because sustainability reporting often sits too far away from the operational systems that actually produce change.

## Data transparency

I deliberately separate:

- **Reported** — directly supported by public Timken reporting;
- **Derived** — calculated from reported data;
- **Synthetic** — facility, risk, CAPA, and project records created for the prototype;
- **Analyst-developed** — thresholds, scoring logic, and prioritization rules.

This is an independent portfolio project and does not represent Timken's internal systems, methodology, or facility data.

---

# 3. AI-Powered IFRS S2 Evidence & Gap Analysis

**IFRS S2 | Climate disclosure | Evidence traceability | Python | LlamaIndex | Human review**

[View repository →](https://github.com/haveisi/AI-Powered-IFRS-S2-Requirement-Mapping-Evidence-Gap-Analysis)

I built this project because sustainability reports contain a large amount of information, but finding the exact evidence needed for a disclosure requirement can still be slow and inconsistent.

The question I explored was:

> Can AI help find and organize disclosure evidence without allowing the AI to make the final compliance judgment?

## Workflow

**Source document  
→ keyword / semantic retrieval  
→ structured evidence extraction  
→ schema validation  
→ quotation validation  
→ human review  
→ IFRS S2 mapping  
→ gap analysis**

The pilot covers selected IFRS S2 topics such as:

- governance;
- climate resilience;
- Scope 1 emissions;
- Scope 2 emissions;
- climate-related targets.

The AI is used to assist with evidence discovery and organization.

The final interpretation remains with the reviewer.

I also distinguish between three different questions:

1. Is relevant evidence present?
2. Does that evidence actually address the requirement?
3. What is still incomplete or uncertain?

This distinction is important because finding a paragraph that contains the right keywords does not automatically mean a disclosure requirement has been satisfied.

The project is an analytical portfolio pilot, not an audit or formal determination of IFRS compliance.

---

# 4. Scope 3 & Regenerative Agriculture Analytics

**Scope 3 | Agriculture | GHG accounting | Python | Streamlit | Scenario analysis**

[View repository →](https://github.com/haveisi/04_scope3_regenerative_agriculture)

This project looks at the next question after calculating emissions:

> What is actually driving the footprint, and what could change it?

The model evaluates emissions associated with:

- stationary fuel;
- mobile fuel;
- purchased electricity;
- fertilizer use;
- agricultural inputs;
- field operations;
- production intensity.

I then use scenario analysis to explore how changes in agricultural practices could affect emissions.

The workflow is:

**GHG data  
→ emissions hotspot  
→ operational driver  
→ reduction scenario  
→ emissions / cost tradeoff**

An interactive Streamlit dashboard is used to communicate the results.

One methodological point I kept explicit is that modeled soil-carbon effects should not automatically be netted against operational emissions without a defensible accounting basis.

This project helped me practice moving from **carbon accounting to reduction planning**.

---

# 5. Real Estate ESG & GRESB Readiness

**Real estate | Energy | Water | Waste | Carbon | ESG evidence | Python | Excel**

[View repository →](https://github.com/haveisi/real-estate-carbon-benchmarking-gresb-analytics)

This project focuses on the quality of the underlying information before ESG reporting or benchmarking begins.

The analytical workbook brings together:

- property information;
- energy use;
- water;
- waste;
- GHG emissions;
- performance benchmarks;
- climate-risk indicators;
- environmental-justice context;
- retrofit opportunities;
- ESG evidence information.

Python is used to review workbook structure, standardize fields, summarize data, and produce reporting-ready outputs.

The basic flow is:

**Raw asset data  
→ structure  
→ validation  
→ KPI calculation  
→ benchmarking  
→ evidence review  
→ reporting readiness**

This work reinforced another recurring theme across my projects:

> ESG reporting problems are often data-management problems before they become reporting problems.

---

# ESG Disclosure Analytics

Disclosure analysis is another recurring part of my work.

I treat a sustainability report as a source of evidence that can be structured and reviewed, rather than simply as a finished document.

A typical workflow is:

**Report  
→ topic  
→ evidence item  
→ page / source reference  
→ KPI or narrative classification  
→ QA/QC  
→ framework mapping  
→ gap or inconsistency  
→ follow-up action**

Questions I typically ask include:

- Where did this number or statement come from?
- Can the source be traced?
- Is the metric defined consistently?
- Was the value reported, calculated, modeled, or assumed?
- Is it comparable with the previous year?
- Which disclosure requirement does it support?
- What is still missing?
- What action should follow?

This is where I see AI being useful—but mainly as an assistant for retrieval, classification, and evidence organization.

Human review still matters.

---

# How I Connect ESG Reporting with Operations

One area I am increasingly interested in is connecting ESG reporting with the operational systems behind the metrics.

## Environmental performance

**Energy / fuel / water / waste  
→ KPI  
→ hotspot  
→ improvement action  
→ performance tracking**

## EHS

**Observation / incident / risk  
→ CAPA  
→ control improvement  
→ operational performance**

## Finance

**Improvement project  
→ CAPEX / OPEX  
→ savings  
→ NPV / payback  
→ management decision**

The objective is not to force every ESG issue into a financial metric.

It is to make environmental, operational, and financial tradeoffs visible when a decision is being made.

---

# Data and Evidence Governance

Across my projects, I try to label information according to what it actually is.

| Status | Meaning |
|---|---|
| **Reported** | Directly supported by an organizational or public source |
| **Calculated** | Derived through a transparent calculation |
| **Modeled** | Generated through analytical or scenario modeling |
| **Assumed** | Introduced where direct information is unavailable |
| **Proxy** | Substitute used when better data are unavailable |
| **Synthetic** | Demonstration data created specifically for a portfolio model |

This matters because a technically correct calculation does not turn an assumed input into a reported company value.

---

# Core Skills Practiced Across the Portfolio

| ESG & Reporting | Data & BI | Analytics & Controls |
|---|---|---|
| GHG Protocol; Scope 1–3 | Excel; Power Query | Data QA/QC |
| ESG data collection; KPI reporting | Power BI; DAX | Evidence traceability |
| Disclosure evidence review | SQL; Python | Data lineage |
| CDP; GRI; TCFD; IFRS S1/S2 | Databricks; Microsoft Fabric | Process mapping |
| EHS / CAPA / risk concepts | SharePoint; Power Automate | Scenario analysis; human-in-the-loop AI |

---

# Tools

**Data and analytics**  
Python | pandas | SQL | Excel | Power Query

**Business intelligence**  
Power BI | DAX | Streamlit

**Data platforms**  
Databricks | Microsoft Fabric | Delta / Lakehouse | SharePoint

**Workflow**  
Microsoft Forms | Power Automate

**AI-assisted analysis**  
LlamaIndex | semantic retrieval | structured extraction | Pydantic validation | human review

**Sustainability methods**  
GHG accounting | ESG metrics | disclosure mapping | reporting readiness | scenario analysis

**Controls**  
QA/QC | reconciliation | exception review | evidence traceability

---

# Where This Portfolio Fits with My Other Work

I keep this repository focused on:

**ESG reporting + carbon accounting + sustainability data systems + evidence + reporting analytics**

My related work is organized separately.

## Life Cycle Assessment & Product Sustainability

Product LCA, EPD methodology, packaging, product carbon, renewable fuels, construction materials, agriculture, and aquaculture.

[View LCA Portfolio →](https://github.com/haveisi/life-cycle-assessment-portfolio)

---

## Climate, Decarbonization & Sustainability Finance

Climate risk, climate action planning, decarbonization scenarios, capital planning, NPV, IRR, marginal abatement cost, transition risk, and financially informed sustainability decisions.

[View Climate, Decarbonization & Finance Portfolio →](https://github.com/haveisi/climate-decarbonization-finance-portfolio)

That portfolio follows a different decision chain:

**Climate / operational exposure  
→ emissions or risk hotspot  
→ response option  
→ environmental benefit  
→ financial analysis  
→ scenario testing  
→ capital decision**

---

# About

My work sits at the intersection of **sustainability reporting, carbon accounting, environmental data, business intelligence, and decision support**.

I am most interested in the space between reporting and action:

**How was the information produced?  
Can we trust it?  
What does it tell us?  
Where is the problem?  
What should change?  
How do we know whether the change worked?**

That is the thread connecting the projects in this portfolio.
