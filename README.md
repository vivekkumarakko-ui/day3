# Data Science Portfolio

## Project: Exploratory Data Analysis — SaaS Customer Churn (CloudPulse)

**Notebook:** [`EDA_Customer_Churn_Portfolio.ipynb`](./EDA_Customer_Churn_Portfolio.ipynb)

### Business Context
CloudPulse, an enterprise B2B SaaS platform, experienced a sharp rise in customer churn over two consecutive quarters. With a Customer Acquisition Cost (CAC) of **$450** and an Average Annual Contract Value (ACV) of **$1,200**, every churned customer represents a significant loss. This analysis identifies who churns, why, and where the Customer Success team should intervene.

---

### Executive Summary — Top 3 Findings

1. **Contract type is the dominant churn driver.** Month-to-Month customers churn at a dramatically higher rate than One-Year and especially Two-Year contract holders — contract commitment is the strongest protective factor in the dataset.
2. **Support ticket volume is a leading indicator of churn.** Churn probability accelerates sharply as ticket counts climb; customers filing multiple tickets are signaling dissatisfaction well before they leave.
3. **Early-tenure, high-charge customers are the highest-risk segment.** Churn is concentrated in the first months of the lifecycle and among customers with above-average monthly charges — particularly those paying via Electronic Check.

---

###  Methodology

Structured six-stage EDA workflow:

| Stage | Focus |
|-------|-------|
| 1 | Business context & problem framing |
| 2 | Data profiling & structural health audit (dtypes, missing values, cardinality) |
| 3 | Univariate analysis (distributions, skew, outliers) |
| 4 | Bivariate analysis (churn vs. contract, tenure, tickets, charges) |
| 5 | Multivariate analysis (correlation heatmap, segmented interactions) |
| 6 | Insight synthesis & strategic recommendations |

**Dataset:** 1,200 customers × 9 features (tenure, contract type, payment method, tech support, support tickets, monthly/total charges, churn label), including realistic missing values handled during profiling.

**Visualizations:** histograms & KDE plots, count plots, box plots by churn segment, correlation heatmaps, and segmented churn-rate bar charts — built with Matplotlib and Seaborn.

**Tools:** Python, pandas, NumPy, Matplotlib, Seaborn, SciPy.

---

### Recommended Strategic Interventions

1. **Contract migration campaign** — incentivize Month-to-Month customers to upgrade to annual/two-year plans (discounts, loyalty pricing) to lock in the strongest churn-reducing factor.
2. **Proactive support-ticket triggers** — flag accounts crossing a ticket-volume threshold for immediate Customer Success outreach before dissatisfaction converts to churn.
3. **Early-lifecycle onboarding program** — target the first 6 months of tenure with structured onboarding and check-ins, prioritizing high-monthly-charge and Electronic Check payers where churn risk concentrates.

---


