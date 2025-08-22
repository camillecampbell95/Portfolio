<!-- Hero -->
<p align="center">
  <img src="assets/cover.png" alt="Data Visualization banner" width="100%" />
</p>

<h1 align="center">Hi, I'm Camille Campbell 👋</h1>
<p align="center">
  <b>Power BI Developer • Data Visualization Specialist • SQL/DAX/SSRS</b><br/>
  Los Angeles, CA · <a href="mailto:camillecampbell95@gmail.com">camillecampbell95@gmail.com</a> · (312) 343-7631
</p>

<p align="center">
  <a href="https://img.shields.io/badge/Power%20BI-Expert-000000.svg"><img src="https://img.shields.io/badge/Power%20BI-Expert-000000.svg" /></a>
  <a href="#"><img src="https://img.shields.io/badge/SQL-Advanced-000000.svg" /></a>
  <a href="#"><img src="https://img.shields.io/badge/DAX-Advanced-000000.svg" /></a>
  <a href="#"><img src="https://img.shields.io/badge/SSRS-Experienced-000000.svg" /></a>
  <a href="#"><img src="https://img.shields.io/badge/Azure%20DevOps-Workflow-000000.svg" /></a>
  <a href="#"><img src="https://img.shields.io/badge/Certification-PL--300-000000.svg" /></a>
</p>

---

## 🎯 What I Do
I turn messy, high-volume data into clear, actionable visuals. I design performant data models, write robust SQL/DAX, and ship dashboards that leaders actually use to make decisions—in real time.

- Design & enhance Power BI dashboards with advanced DAX and optimized models  
- Build SQL Server stored procedures and ETL automations for reliable datasets  
- Maintain enterprise reporting (400+ SSRS reports & subscriptions)  
- Collaborate across data architecture, development, and stakeholders for seamless delivery

> Toolbelt: **Power BI, SQL Server, DAX, SSRS, Azure DevOps, JIRA, Python, R, Looker**

---

## 🧪 Featured Visual Projects
> Replace preview images with your own thumbnails (export PNGs) and link to public reports or GIF demos.

<table>
  <tr>
    <td width="33%">
      <a href="projects/turnpike-ops/README.md">
        <img src="projects/turnpike-ops/cover.png" alt="Turnpike Ops Dashboard" />
        <h4>Turnpike Ops KPIs</h4>
      </a>
      <p>Real-time operational metrics with role-based drill-downs, optimized with calculation groups.</p>
      <code>Power BI · DAX · SQL Server</code>
    </td>
    <td width="33%">
      <a href="projects/opm-hiring/README.md">
        <img src="projects/opm-hiring/cover.png" alt="OPM Hiring Pipeline" />
        <h4>Gov Hiring Pipeline</h4>
      </a>
      <p>Funnel analytics, time-to-fill trends, and interactive drill-through for bottleneck analysis.</p>
      <code>Power BI · DAX · Python ETL</code>
    </td>
    <td width="33%">
      <a href="projects/marketing-ab/README.md">
        <img src="projects/marketing-ab/cover.png" alt="Marketing A/B Dashboard" />
        <h4>Marketing A/B Uplift</h4>
      </a>
      <p>Experiment tracking, cohort views, and uplift calculations across omni-channel campaigns.</p>
      <code>Power BI · SQL · DAX</code>
    </td>
  </tr>
</table>

---

## 🧱 Data Modeling & DAX Patterns
- **Star schemas** with surrogate keys, incremental refresh, and composite models where needed  
- **Calculation groups** for time intelligence and dynamic formatting  
- **Row-level security (RLS)** for safe cross-department sharing  
- **Performance**: VertiPaq Analyzer, measure branching, minimized bi-directional filters

```DAX
-- Example: Reusable YoY pattern with calculation group compatibility
YoY % =
VAR Cur = [Total KPI]
VAR Prev = CALCULATE([Total KPI], DATEADD('Date'[Date], -1, YEAR))
RETURN DIVIDE(Cur - Prev, Prev)
