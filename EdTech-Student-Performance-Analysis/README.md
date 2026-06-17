# 🎓 Real-Life Student Learning Platform Analysis

## Business Context

This analysis was conducted during a live internship engagement for an educational foundation operating a digital learning platform across schools in Pakistan. The platform consists of a **suite of 7 learning apps**, and this analysis focuses specifically on one app within that suite.

With 48,569 total student records across multiple cities, the goal was to understand what drives learning outcomes among students who used this app during the reporting window, and to surface actionable insights for the foundation around performance, school-level differences, and data quality.

---

## ⚠️ Critical Data Context

Three factors must be understood before interpreting any figures:

1. **This is 1 of 7 apps** — students have access to a full suite. A student not present here may be actively engaged elsewhere in the platform.
2. **3-day reporting window (June 9–11, 2026)** — this is a snapshot, not a long-term engagement measure. Regular users may simply not have opened this app during these 3 days.
3. **Database includes ex-students** — 28,025 of 48,569 accounts belong to students who have dropped out, left, or graduated and are marked Inactive. All engagement analysis is scoped to the 522 students who actively used this app during the window.

---

## Business Questions

1. What drives lesson completion among students who used this app?
2. Are there meaningful performance differences between genders?
3. Which schools are achieving the strongest outcomes and why?
4. How is time split between core curriculum and library content?
5. Are there data quality issues that need engineering attention?

---

## Dataset Overview

| Property | Detail |
|---|---|
| Total Records | 48,569 |
| Active Accounts (current students) | 20,544 |
| Inactive Accounts (ex-students) | 28,025 |
| Students who used this app in window | 522 |
| Reporting Period | June 9–11, 2026 (3 days) |
| Subjects | Math, English, BI, BM |
| Key Metrics | Play Time, Core Time, Library Time, Earned Stars, Completed Lessons |

> ⚠️ This dataset contains real student data from an active educational programme. The raw data file is kept private and is not published in this repository.

---

## Tools & Libraries

- **Python** — core analysis language
- **pandas** — data cleaning, transformation and aggregation
- **matplotlib** — charting and visualisations
- **seaborn** — statistical plots (KDE, violin, jointplot, ECDF)
- **scipy** — Pearson correlation analysis

---

## Key Findings

### 📈 Play Time is the strongest predictor of lesson completion (r = 0.78)
Students who spend more time in the app complete significantly more lessons. Top 10% of learners average 101 minutes and complete 8+ lessons per session.

### ♀️ Gender engagement patterns differ meaningfully
Female students earn more stars (avg 44.91 vs 7.19), male students complete more lessons (avg 3.52 vs 2.59) — similar play times suggest different engagement behaviour rather than different effort levels.

### 🏫 MPK and MLR region schools outperform consistently
School 290-MS-MPK-MPK achieved a 47.4% adoption rate among its active students during the window. 288-MS-MPK-MPK led in average lessons completed (12.25). These schools represent a replicable model.

### 📚 Core curriculum dominates over library content (5.7:1 ratio)
Students spend nearly 6x more time on core content than library time — suggesting library features may need better promotion or integration into session structure.

### 🐛 Data quality issues detected
5 students have negative Earned Stars (as low as -4,048) and 10 active students show zero play time — both require engineering review.

---

## Recommendations

| Priority | Action |
|---|---|
| 🔴 Critical | Report negative stars bug to engineering with affected Student IDs |
| 🟠 High | Interview top-performing schools and document replicable practices |
| 🟠 High | Set 30-minute session targets when teachers assign this app |
| 🟡 Medium | Investigate gender differences in stars vs lesson completion |
| 🟡 Medium | Promote library content within structured session formats |
| 🟢 Low | Request cross-app data for a complete platform engagement picture |

---

## Project Structure

```
Real-Life-Student-Analysis/
│
├── Real_Life_Student_Data_Analysis.ipynb   # Full analysis + insights
└── README.md                               # Project documentation
```

> Raw data file not included — contains real student information.

---

## How to Run

```bash
# Clone the repository
git clone https://github.com/Hamza2058/Exploratory-Data-Analytics.git

# Navigate to the project folder
cd Exploratory-Data-Analytics/Real-Life-Student-Analysis

# Install dependencies
pip install pandas matplotlib seaborn scipy openpyxl

# Open the notebook
jupyter notebook Real_Life_Student_Data_Analysis.ipynb
```

---

## Limitations

- 3-day window only — not representative of long-term engagement
- Single app view — cross-app data needed for full picture
- Small school-level samples (3–4 students) should be interpreted cautiously
- Lesson completion and stars are proxy metrics — actual learning outcomes require assessment data to validate

---

*Analysis by Hamza Awan — Data Analyst Intern*
*📍 Karachi, Pakistan*
*🔗 [GitHub](https://github.com/Hamza2058)*
