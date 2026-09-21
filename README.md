# KPIs_Productivity_T_T2026

> **Analytics from daily trackers performance | Excel/GSheets**
---
Author: Walter Orlando Vargas  ·  Version 4 
Version Date: September 20th, 2026

---

## About this Project

This document is the Readme/reference manual for the project “KPIs Productivity T&T_2025-2026,” a personal data analysis exercise based on the daily performance of the night shift trackers (Track & Trace representatives) at Circle Logistics. This is not a logistics operations project; rather, it's a descriptive and analytical statistical exercise using internal team KPIs (verification calls, status updates, and incoming/outgoing calls). It serves as a practice exercise in data analysis, information cleaning, and the creation of pivot tables, dashboards, and, later, SQL queries.

The data source is entirely manual: each shift, supervisors post the day's KPIs in a Google Chat space so the team can review their performance at the end of the shift. This data is in plain text format, derived from the workloads processed in the organization's TMS system, along with the call system (Transport Pro TMS and the 8x8 voice call app). From there, the author copies that text and transforms it with the help of an AI prompt (Gemini) into a table ready to paste into Excel/Sheets, and then consolidates it into the historical dataset that feeds the dynamic tables, graphs and — more recently — the SQL queries of this project.


## The Dataset
The “KPI´s Productivity T&T_2025-2026 V-GH 1.0” file contains the historical dataset used for this project.


<p align="center"><b>CIRCLE LOGISTICS · TRACK & TRACE</b></p>

# KPI's Circle Logistics T&T2025
### ( Readme Optimized by AI )

*Analytics from daily trackers performance*

Author: Walter Orlando Vargas · Version 4 — Writing and analysis assisted by AI (Claude)
Version date: September 20, 2026

> **Note:** tracker names shown below have been replaced with aliases to protect the privacy of real coworkers.

---

## Introduction

This document is the Readme / reference manual for the **"KPI's Productivity T&T_2025-2026"** project, a personal data analysis exercise built on the daily performance of trackers (Track & Trace representatives) on the night shift at Circle Logistics. This is not a logistics-operations project: it is an exercise in descriptive statistics and internal team KPI analytics (verification calls, status updates, and inbound/outbound calls), used as practice in data analysis, data cleaning, and building pivot tables, dashboards, and — later on — SQL queries.

The data originates entirely from a manual process: each shift, supervisors post that day's KPIs in a Google Chat space so the team can see their performance at the end of the shift, in plain-text format based on the loads worked in the organization's TMS along with the calling system (Transport Pro TMS and the 8x8 voice call app). From there, the author copies that text and, with the help of an AI prompt (Gemini), turns it into a table ready to paste into Excel/Sheets, which is then consolidated into the historical dataset that feeds the pivot tables, charts, and — more recently — the SQL queries in this project.

![KPIs posted by shift supervisors in the "Baby Got TRACK" chat space](./fig1-chat-evidence.png)
*Fig. 1 — KPIs posted by shift supervisors in the "Baby Got TRACK" chat space, the original source of the data. Supervisor and tracker names have been replaced with aliases.*

![AI prompt used to build the KPI table](./fig2-gemini-prompt.png)
*Fig. 2 — AI prompt used to turn the supervisors' plain text into a table ready to copy into Excel. Names have been replaced with aliases.*

> **NOTE:** the project was created, along with the first version of this Word document, on February 16, 2026. Starting with this version, on September 20, 2026, "Version 4" of this Readme begins: the document moves on from being a template with unwritten sections ("Write your text here") to bringing together, in an organized way, the author's own progress notes along with an analysis generated with AI (Claude) on the consolidated data file (.xlsx). From this conversation onward, the goal is to use AI as ongoing support for consulting and teaching in data analysis, big data, and logistics, to improve the project's focus, segmentation, cleanup, and overall organization.

## Source and Scope of the Data

The Excel file **"KPI's Productivity T&T_2025-2026 V-GH 1.0"** holds the project's consolidated history.

![Spreadsheet view with the daily log per tracker](./fig3-sheet-dashboard.png)
*Fig. 3 — View of the spreadsheet with the daily log per tracker and the summary of global hourly averages, a direct precursor to the consolidated dataset. Tracker names have been replaced with aliases.*

## Methodological Considerations and Limitations

**Important notes to keep in mind:**

- From January 2026 onward, every KPI for the shift is captured in full, so those months are considerably more representative than earlier ones.
- At the moment, January has 4 rows with no data, and February also has some incomplete rows.

**This is a practice exercise and should not be read as a real, rigorous analysis of the KPIs, since:**

- The formula used so far has made it impossible to compare week over week cleanly: the calculation accumulates the total of previous weeks, so the average keeps normalizing instead of clearly showing when someone's numbers go up or down in a given week.
- Data cannot be extracted the same way for every shift, since some supervisors share the report as text and others as screenshots (images), which makes consistent extraction difficult.
- Tracker names had to be cleaned up and standardized so they wouldn't distort the totals: "Moriah" was sometimes logged as "Moria."
- On Sunday, July 28, 2025, the decision was made to work with pivot tables and totals instead of averages: the monthly sheets produced very different results when estimating weekly productivity from an average; with totals, the real total is instead divided across the 4 weeks of each month.

In addition, when reviewing the dataset there are rows categorized as "No KPIs" and error values (#DIV/0!) in some of the per-tracker average tables — further evidence of the data gaps noted above, and a cleanup item still pending before drawing any definitive conclusions per tracker.
