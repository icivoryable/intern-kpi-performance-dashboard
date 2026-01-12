# intern-kpi-performance-dashboard
KPI Dashboard
# Intern KPI Performance Dashboard

## Executive Summary
This project reconstructs and analyzes intern recruiting KPIs using Power BI under real-world constraints, including incomplete source data, inconsistent reporting cutoffs, and evolving performance definitions.

Rather than enforcing a single interpretation, the model supports multiple reporting lenses (official cutoff, month-end, and submission window) to highlight how timing decisions materially impact KPI narratives.

The dashboard emphasizes transparency, consistency, and decision usefulness over surface-level accuracy.

---

## Business Context
This analysis supported a multi-state intern training program designed to:
- Teach data collection discipline
- Introduce Tableau and Power BI workflows
- Track KPI accountability across geographic regions

As a result, the data reflects learning curves, reporting delays, and shifting definitions — all explicitly handled in the model.

---

## Technical Environment
- Power BI Desktop (Windows VM)
- Azure Virtual Machine with secure RDP access
- Cross-OS development from macOS (M1)
- Power BI Service (Web)

This setup mirrors enterprise BI environments where local tooling constraints require cloud-based development.

---

## Data Model
The model follows a simplified star schema:

- **Fact_Performance**: KPI activity by intern and date
- **Dim_Intern**: Intern metadata
- **Dim_Calendar**: Time intelligence support

Synthetic data was used to reconstruct observed KPI totals after original source files became unavailable.

---

## Key Capabilities
- Dynamic KPI evaluation using DAX measures
- Time-aware performance analysis (WoW, cumulative)
- Performance tiering with icon-based indicators
- Intern-level and state-level rollups
- Explicit handling of reporting cutoff ambiguity

---

## Repository Structure
