# Bupa-patient-satisfaction-analysis
Healthcare data analytics project using Excel and Power BI to analyse patient satisfaction, service quality, waiting times and complaints.
# Patient Satisfaction & Service Quality Analysis — Bupa Healthcare

**Healthcare Data Analytics | Excel | Power BI | DAX**

> **Data disclosure:** This is an independent portfolio case study using synthetic healthcare data. It is not commissioned by Bupa, affiliated with Bupa, or based on Bupa's internal data or actual performance.

## Project Overview

This project explores how healthcare organisations can use patient feedback and operational data to evaluate patient satisfaction, assess service quality, identify operational challenges and recommend improvements.

Using Excel and Microsoft Power BI, I analysed four synthetic datasets covering patients, service interactions, survey responses and complaints.

The project demonstrates my ability to prepare and validate data, develop a relational data model, create DAX measures, build interactive dashboards and translate analytical findings into practical business recommendations.

## Business Objectives

- Evaluate overall patient satisfaction.
- Identify satisfaction differences across age groups, service categories and departments.
- Analyse waiting-time performance and service-quality ratings.
- Investigate complaint categories and resolution performance.
- Examine the relationship between waiting time and patient satisfaction.
- Develop evidence-based management recommendations.

## Dataset Overview

The project contains four datasets with 4,081 records in total.

| Dataset | Records | Description |
|---|---:|---|
| Patients | 1,000 | Patient demographics and service categories |
| Service Interactions | 1,500 | Departments, dates, waiting times and service ratings |
| Survey Responses | 1,500 | Survey status and satisfaction scores |
| Complaints | 81 | Complaint categories and resolution status |
| **Total** | **4,081** | |

## Tools and Technologies

- **Microsoft Excel:** Data cleaning, preparation and validation.
- **Power BI Desktop:** Data modelling, interactive dashboards and visualisation.
- **DAX:** KPI calculations, performance measures and statistical analysis.
- **GitHub:** Project documentation and portfolio presentation.

## Data Preparation and Validation

Data preparation was completed in Excel before importing the cleaned datasets into Power BI.

Key activities included:

- Reviewing unique identifiers and duplicate records.
- Checking data types and date fields.
- Cleaning text fields.
- Reviewing missing values and preserving legitimate nulls.
- Validating relationships between patient, interaction, survey and complaint records.
- Reconciling record counts and unique identifiers.

**Validation outcomes:**
- All expected record counts and unique identifiers reconciled.
- No orphan patient references were identified.
- No orphan survey or complaint interaction references were identified.
- Missing ratings were retained rather than incorrectly replaced with zero.

## Power BI Dashboard
<img width="1152" height="647" alt="Executive Overview" src="https://github.com/user-attachments/assets/a5f62796-8ef0-47fd-94cf-89d1c9f06896" />

<img width="1157" height="646" alt="Complaints   Resolution" src="https://github.com/user-attachments/assets/975bcb3c-4aeb-4c93-86ea-d96c0bcb555e" />

<img width="1152" height="645" alt="Patient Satisfaction Analysis" src="https://github.com/user-attachments/assets/28409162-5a72-49f6-8b09-a9e4d9d4df18" />

<img width="1147" height="642" alt="Service Quality   Waiting Time" src="https://github.com/user-attachments/assets/acb3790e-e9c2-4a26-9af0-ec9940118e67" />

<img width="1157" height="650" alt="Management Insights" src="https://github.com/user-attachments/assets/868a3e3f-10dd-460f-ab8f-bb4a5fac4552" />






The report contains five analytical pages:

1. **Executive Overview:** Overall performance indicators and headline findings.
2. **Patient Satisfaction Analysis:** Satisfaction distribution and comparisons by age group, service category and department.
3. **Service Quality & Waiting Time:** Waiting-time analysis and service-quality ratings.
4. **Complaints & Resolution:** Complaint categories, status, trends and resolution performance.
5. **Management Insights:** Key findings and recommended improvement priorities.

### Dashboard Screenshots

#### 1. Executive Overview
![Executive Overview](Executive%20Overview.png)

#### 2. Patient Satisfaction Analysis
![Patient Satisfaction Analysis](Patient%20Satisfaction%20Analysis.png)

#### 3. Service Quality & Waiting Time
![Service Quality and Waiting Time](Service%20Quality%20%26%20Waiting%20Time.png)

#### 4. Complaints & Resolution
![Complaints and Resolution](Complaints%20%26%20Resolution.png)

#### 5. Management Insights
![Management Insights](Management%20Insights.png)

## Key Findings

### 1. Overall Patient Satisfaction

| Metric | Result |
|---|---:|
| Average satisfaction | 4.02 / 5 |
| Positive satisfaction | 73.95% |
| Completed surveys | 975 |
| Survey response rate | 65% |

### 2. Waiting-Time Performance

| Metric | Result |
|---|---:|
| Average waiting time | 40.43 minutes |
| Median waiting time | 34 minutes |
| Maximum waiting time | 166 minutes |
| Highest department average | Authorisations: 43.61 minutes |
| Lowest department average | Member Support: 37.16 minutes |

### 3. Satisfaction by Patient Group

- Highest age-group satisfaction: 45–59, scoring 4.07/5.
- Lowest age-group satisfaction: 30–44, scoring 3.96/5.
- Highest service-category satisfaction: Health Insurance, scoring 4.092/5.
- Lowest service-category satisfaction: Care Services, scoring 3.978/5.
- Highest department satisfaction: Care Services, scoring 4.176/5.
- Lowest department satisfaction: Appointments, scoring 3.966/5.

### 4. Waiting Time and Patient Satisfaction

Pearson correlation analysis produced:

- Correlation coefficient: **-0.370**
- Valid paired observations: **975**

This indicates a negative association between waiting time and satisfaction at the individual interaction level. Longer waits tended to be associated with lower satisfaction scores.

Correlation does not establish causation. The department-level comparison also showed a different pattern, demonstrating why analysis at different levels is important.

### 5. Complaints and Resolution

| Metric | Result |
|---|---:|
| Total complaints | 81 |
| Resolved complaints | 62 |
| Open complaints | 5 |
| In-progress complaints | 14 |
| Resolution rate | 76.54% |

The largest complaint category was Billing or Claims, with 20 complaints, followed by Care Coordination with 15 and Waiting Time with 13.

## Management Recommendations

Based on the findings, five improvement priorities were identified:

1. Review Authorisations workflows to identify approval bottlenecks and long waiting times.
2. Improve the appointment experience through better scheduling, accessibility and patient communication.
3. Investigate recurring Billing or Claims complaints.
4. Strengthen complaint ownership, follow-up and resolution timelines.
5. Improve survey participation and completeness of service-quality feedback, particularly discharge ratings.

## Data Limitations

- The dataset is synthetic and does not represent actual Bupa performance.
- Only 65% of survey records were completed.
- There were 525 missing satisfaction scores.
- Only 257 of 1,500 interactions had valid discharge ratings (17.13%).
- Correlation indicates association, not causation.
- Group averages alone do not establish statistically significant differences.

These limitations were considered when interpreting results and developing recommendations.

## Project Structure

```text
bupa-patient-satisfaction-analysis/
│
├── README.md
│
├── data/
│   └── synthetic_dataset.xlsx
│
├── powerbi/
│   └── Bupa_Patient_Satisfaction_Analysis.pbix
│
├── presentation/
│   ├── Bupa_Patient_Satisfaction_Analysis.pptx
│   └── Bupa_Patient_Satisfaction_Analysis.pdf
│
└── screenshots/
    ├── executive-overview.png
    ├── patient-satisfaction.png
    ├── service-quality.png
    ├── complaints-resolution.png
    └── management-insights.png
```

*The filenames above are suggested examples. Replace them with the actual filenames uploaded to the repository.*

## What This Project Demonstrates

Through this project, I demonstrated practical skills in:

- Healthcare data analysis.
- Data cleaning and validation.
- Relational data modelling.
- Power BI dashboard development.
- DAX calculations and KPI development.
- Descriptive and diagnostic analysis.
- Statistical interpretation.
- Business insights and management recommendations.
- Communicating analytical findings to stakeholders.

---

**Project Category:** Healthcare Data Analytics  
**Tools:** Excel, Power BI, DAX  
**Programme:** Amdari Internship Program  
**Author:** Helen Ojo  
**LinkedIn:** https://www.linkedin.com/in/helen-ojo-7b85a1247/ 
