# HR Headcount Planner

## Business Problem
Organisations often underestimate their true hiring need by focusing only on growth targets while ignoring attrition and internal mobility. This project builds a data-driven headcount planning model that calculates gross hiring requirements by department and spreads them across quarters — giving HR and Finance a realistic, costed workforce plan.

## Key Insight
> The business target requires **175 net new hires**. After factoring in attrition and internal mobility, the true gross hiring requirement is **357 hires** — more than double the headline number.

## Project Summary
| Metric | Result |
|---|---|
| Organisation Size | 1,000 employees across 6 departments |
| Net Headcount Gap | 175 employees |
| Gross Hiring Required | 357 employees |
| Peak Hiring Quarter | Q2 & Q3 (107 hires each) |
| Highest Risk Department | IT (55 days avg time to fill) |
| Total Hiring Investment | 22,683,000 AED |

## Hiring Plan by Department
| Department | Gross Hires | Urgency |
|---|---|---|
| Operations | 115 | Medium |
| IT | 97 | High |
| Sales | 62 | Standard |
| Finance | 49 | Medium |
| HR | 17 | Medium |
| Legal | 17 | High |

## Planning Logic
- **Net gap** = Target headcount − Current headcount
- **Attrition backfill** = Current headcount × Attrition rate
- **Mobility loss** = Current headcount × Internal mobility rate
- **Gross hiring need** = Net gap + Attrition backfill + Mobility loss
- **Hiring cost** = Gross hires × Average monthly salary × 3 months

## Tech Stack
- Python · pandas · numpy
- matplotlib · seaborn

## Files
| File | Description |
|---|---|
| `02_headcount_planner.ipynb` | Full planning notebook |
| `headcount_plan_dashboard.png` | 4-chart visual dashboard |
| `headcount_hiring_plan.csv` | Quarterly hiring plan with urgency flags |
