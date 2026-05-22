# FAERS Adverse Event Analysis

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-11557C?style=for-the-badge&logo=matplotlib&logoColor=white)
![Power BI](https://img.shields.io/badge/Power%20BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)

## Project Overview
This portfolio project analyzes adverse event reports from the FDA Adverse Event Reporting System (FAERS) using Python-based data analytics workflows. The analysis focuses on identifying patient demographic patterns, adverse reaction trends, severe outcomes, and drug-related safety signals that support evidence-based pharmacovigilance insights.

## Business Objective
The goal is to transform raw FAERS reporting data into actionable intelligence for healthcare and life sciences stakeholders by:
- Highlighting high-risk demographic groups
- Identifying reactions associated with severe outcomes (death and hospitalization)
- Detecting drugs and drug-reaction combinations with elevated reporting frequency
- Enabling data-driven safety monitoring and risk prioritization

## Dataset Description
The analysis uses four core FAERS tables:

- **DEMO**: Patient demographic information (age, gender, country, report metadata)
- **DRUG**: Drug-level details and role code (e.g., primary suspect, secondary suspect)
- **REAC**: Reported adverse reactions linked to each case
- **OUTC**: Clinical patient outcomes (including severe outcomes such as death and hospitalization)

## Methodology
1. Data extraction and ingestion of selected FAERS tables
2. Data cleaning and preparation (null handling, type normalization, filtering)
3. Table joins and analytical feature engineering at case/report level
4. Exploratory and comparative analysis by demographic, reaction, and drug dimensions
5. Visualization and dashboarding in Python and Power BI for communication of insights

## Key Analyses Performed

### Module 1 – Demographic Analysis
- Age Distribution of Reports
- Gender Distribution
- Top Countries by Report Volume
- Death vs Hospitalization by Age Group
- Severe Outcome Percentage by Age Group

### Module 2 – Reaction Analysis
- Top 20 Most Reported Reactions
- Reactions Associated with Death
- Reactions Associated with Hospitalization
- Young vs Elderly Reaction Patterns
- Country-wise Reaction Analysis

### Module 3 – Drug Risk Analysis
- Top 20 Drugs by Adverse Event Reports
- Drugs Associated with Death
- Drugs Associated with Hospitalization
- Drug Role Distribution (Primary Suspect vs Secondary Suspect)
- Top Drug–Reaction Pairs

## Sample Visualizations

### Age Distribution
![Age Distribution](images/age_distribution.png)
*Distribution of adverse event reports across patient age groups.*

### Gender Distribution
![Gender Distribution](images/gender_distribution.png)
*Breakdown of reported adverse events by patient gender.*

### Top Reported Reactions
![Top Reported Reactions](images/top_20_reactions_distribution.png)
*Most frequently reported adverse reactions in the FAERS dataset.*

### Young vs Elderly Reaction Patterns
![Young vs Elderly Reaction Patterns](images/reaction_young_vs_elderly.png)
*Comparison of reaction patterns between younger and elderly patients.*

### Top Drug–Reaction Associations
![Top Drug–Reaction Associations](images/top_20_drug_reactions.png)
*Leading drug–reaction combinations by reporting frequency.*

## Key Findings
- Reporting volume varies significantly by age bands, with clear differences in severe outcome rates.
- Death and hospitalization outcomes are concentrated in specific age cohorts and reaction categories.
- A subset of drugs and drug-reaction pairs appears repeatedly in serious adverse event reports.
- Geographic variation in report volume and reaction patterns indicates potential regional reporting and risk differences.

## Technologies Used
- **Python**
- **Pandas**
- **NumPy**
- **Matplotlib**
- **Google Colab**
- **Power BI**

## Future Enhancements
- Add temporal trend analysis (monthly/quarterly change in reaction frequency)
- Integrate disproportionality metrics (e.g., PRR/ROR) for stronger signal detection
- Build automated data refresh and reproducible ETL workflows
- Add model-based risk stratification for severe outcomes
- Publish an interactive dashboard with drill-down capabilities
