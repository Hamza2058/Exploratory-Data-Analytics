# 📉 Subscription Cohort Analysis — Churn, Retention & Revenue Insights

## Business Context

A SaaS subscription business with 3,069 total subscribers and a fixed monthly price of $39 needs to understand why it is losing customers faster than industry benchmarks allow for sustainable growth. With 65.3% of all subscribers having cancelled and cancellations accelerating at a rate nearly 6x faster than signup growth, the business faces a retention crisis that — if unaddressed — will eventually outpace new customer acquisition.

This analysis examines one year of subscription data (September 2022 – September 2023) to identify when customers are leaving, how long they stay before churning, and what patterns exist across monthly cohorts that can inform a data-driven retention strategy.

---

## Business Questions

1. What is the overall churn rate and how does it compare to healthy SaaS benchmarks?
2. When in the subscription lifecycle are customers most likely to cancel?
3. Are cancellations accelerating or decelerating over time relative to new signups?
4. Which signup cohorts show the strongest and weakest retention rates?
5. How much revenue is being lost to non-payment and is it recoverable?

---

## Dataset Overview

| Property | Detail |
|---|---|
| Source | Maven Analytics Data Playground |
| Total Records | 3,069 subscribers |
| Date Range | September 1, 2022 – September 8, 2023 |
| Subscription Price | $39/month (fixed) |
| Key Columns | customer_id, created_date, canceled_date, subscription_cost, subscription_interval, was_subscription_paid |
| Active Subscribers | 1,065 (34.7%) |
| Cancelled Subscribers | 2,004 (65.3%) |

---

## Tools & Libraries

- **Python** — core analysis language
- **pandas** — data cleaning, cohort construction and aggregation
- **matplotlib** — charting and visualisations
- **seaborn** — heatmaps, distribution plots and trend lines
- **numpy** — numerical operations

---

## Key Findings

### 🔴 65.3% overall churn rate — well above healthy SaaS benchmarks
Only 1 in 3 subscribers remains active. A sustainable SaaS business targets 2–5% monthly churn. This business is operating significantly above that threshold.

### ⚡ 36.8% of cancellations happen within the first 30 days
737 customers left within their first billing cycle — representing $28,743 in immediately lost monthly recurring revenue. The median subscription duration before cancellation is just 38 days.

### 📈 Cancellations growing 6x faster than signups
New signups grew 41% from Sep 2022 to Jul 2023. Cancellations grew 582% in the same period. Acquisition is working — retention is not.

### 💳 $5,187 lost to failed payments
133 subscriptions (4.3%) went unpaid — a secondary but recoverable revenue leak addressable through automated payment recovery sequences.

### 📊 Early cohorts retain better than later ones
September–November 2022 cohorts show stronger long-term retention than 2023 cohorts, suggesting early adopters had stronger product-market fit or came from higher-quality acquisition channels.

---

## Net Monthly Subscription Trend

| Month | Signups | Cancellations | Net Change |
|---|---|---|---|
| Sep 2022 | 217 | 33 | +184 |
| Dec 2022 | 230 | 123 | +107 |
| Mar 2023 | 266 | 224 | +42 |
| Apr 2023 | 223 | 194 | +29 |
| Jul 2023 | 306 | 207 | +99 |
| Aug 2023 | 268 | 219 | +49 |

The business is still growing but the margin between signups and cancellations has narrowed significantly since launch.

---

## Recommendations

| Priority | Action | Expected Impact |
|---|---|---|
| 🔴 Critical | Implement 30-day onboarding sequence (Day 3, 7, 14, 30 touchpoints) | Reduce early churn rate |
| 🔴 Critical | Survey cancelled customers to identify primary churn drivers | Root cause clarity |
| 🟠 High | Redirect acquisition budget toward retention initiatives | Higher ROI than new signups |
| 🟠 High | Implement dunning sequence for failed payments | Recover $1,000–2,000 of $5,187 lost |
| 🟡 Medium | Analyse Sep–Nov 2022 cohort to replicate better retention conditions | Improve cohort quality |
| 🟡 Medium | Set monthly churn KPI target of <5% | Measurable retention goal |

---

## Project Structure

```
Subscription-Cohort-Analysis/
│
├── Subscription_analysis.ipynb              # Full analysis notebook with insights
├── Subscription_Cohort_Analysis_Data.csv    # Dataset (Maven Analytics)
└── README.md                                # Project documentation
```

---

## How to Run

```bash
# Clone the repository
git clone https://github.com/Hamza2058/Exploratory-Data-Analytics.git

# Navigate to the project folder
cd Exploratory-Data-Analytics/Subscription-Cohort-Analysis

# Install dependencies
pip install pandas matplotlib seaborn numpy

# Open the notebook
jupyter notebook Subscription_analysis.ipynb
```

---

## Limitations

- No product usage or feature engagement data — limits root cause analysis of churn
- Single fixed price point ($39/month) — pricing sensitivity cannot be assessed
- No marketing channel attribution — unable to determine which channels produce the most retained customers
- A longer dataset (2+ years) would strengthen cohort retention conclusions

---

*Analysis by Hamza Awan — Data Analyst*
*Dataset: Maven Analytics — Subscription Cohort Analysis*
*📍 Karachi, Pakistan*
*🔗 [GitHub](https://github.com/Hamza2058) | [Upwork](#)*
