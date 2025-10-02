## 📈HR Attrition Analysis Using PowerBI

## 📌Project Summary  
A focused, interactive Power BI dashboard that converts employee records into actionable HR intelligence. The report surfaces attrition drivers, role- and cohort-level risk, satisfaction signals, and compensation patterns to guide targeted retention and people-strategy decisions.

## 🎯Highlights  
Deliverable: Single Power BI report file HR_Analytics.pbix containing data model, visuals, Power Query steps, and DAX measures.  
Primary Objectives: Monitor attrition, identify root causes, prioritise retention actions, quantify workforce risk.  
Audience: HR leaders, people analytics teams, department managers, executive stakeholders.

## 🚀Dashboard Features - Executive KPIs  
- The dashboard displays executive KPIs including employee count, attrition rate, attrition count, average years at company, average age, and average income.
- It shows attrition share by education category to reveal which educational backgrounds have higher churn.
- It presents attrition counts by age group to highlight vulnerable career stages.
- It breaks down attrition across salary bands to surface compensation-related churn patterns.
- It lists role-level attrition counts so high-risk roles can be quickly identified.
- It provides tenure-based attrition by years at company to spot early-tenure leakage and mid-tenure trends.
- It includes a job satisfaction table by role with counts across satisfaction levels to correlate morale with churn.
- It offers interactive slicers for Date, Department, Role, Education, and Salary Band to filter analyses dynamically.
- It supports drill-through to employee-level detail pages for investigative follow-up on specific cohorts.
- It contains ready-to-use DAX measures for attrition count, attrition rate, and average years at company.
- It enables cohort and trend analysis to measure the impact of interventions over time.
- It is designed for quick decision-making with actionable visuals and exports for stakeholder reporting.


## 🟰Key DAX Samples  
Attrition Count  
```DAX
Attrition Count = CALCULATE(COUNTROWS(Employees), Employees[Status] = "Terminated")
```
Attrition Rate  
```DAX
Attrition Rate = DIVIDE([Attrition Count], COUNTROWS(Employees))
```
Average Years at Company  
```DAX
Avg Years = AVERAGE(Employees[YearsAtCompany])
```

## 📈Inferences from the HR Attrition Dashboard

🧾Material turnover: Attrition Rate is **16.21%** with **229** leavers from **1413** employees, indicating a meaningful retention challenge requiring prioritized interventions.

⏱Early-tenure leakage: Highest counts at Years 0–2 (~60, ~50, ~40) point to onboarding, role clarity, or expectation-mismatch problems in the first year(s). Implement immediate onboarding fixes.

👥Mid-career concentration: Peak attrition in the 25–35 age bands suggests career progression, development, or work–life balance issues for early-to-mid career employees.

🏷Role hotspots: Sales Executives and Research Scientists exhibit the highest attrition counts; role-targeted retention plans and manager interventions should be prioritised.

🎓Education skew: Life Sciences and Medical-educated employees account for large shares of attrition (31% and 25% respectively), indicating possible role-fit, expectation, or culture alignment issues within those hiring streams.

💷Mid-band churn: Salary bands 4000–8000 show elevated attrition counts, suggesting mid-level compensation may be less competitive or progression unclear in those cohorts.

🙂Job satisfaction distribution shows many roles with moderate-to-low satisfaction counts; low satisfaction correlates with higher churned roles and should guide targeted engagement.

## 💡Actionable Recommendations

1. Strengthen early retention: Implement a structured 90-day onboarding, role clarity sessions, and scheduled manager check-ins for new hires.  
2. Role-level retention plans: Design tailored interventions for Sales Executives and Research Scientists—compensation review, career-path clarity, mentoring, and manager coaching.  
3. Compensation benchmarking: Reassess mid-band salaries and promotion criteria; introduce transparent progression frameworks.  
4. Boost job satisfaction: Launch targeted engagement surveys, manager training, and role-specific improvements where satisfaction is low.  
5. Hiring and role-fit review: Rework job descriptions and interview scorecards for hires from Life Sciences and Medical backgrounds to reduce expectation mismatches.  
6. Early-warning KPIs: Add retention KPIs by cohort (hire month, manager, role) and implement alerting for sudden spikes in early-tenure exits.  
7. Measure impact: Run controlled pilots (onboarding tweaks, pay adjustments) and track lift using cohort retention and cost-of-attrition metrics.

