# Insurance Customer & Claims Analysis

Power BI analysis of 10K+ insurance policies to understand policy performance, claim outcomes, financial exposure, and customer feedback sentiment.

## Dashboard Preview

> Screenshots will be added here after exporting the three Power BI report pages.

## Business Problem

Insurance companies need to monitor policy portfolios, understand claim outcomes, evaluate financial exposure, and identify customer experience issues.

This project analyzes insurance policy and claims data together with customer feedback to answer questions such as:

- What is the overall premium and coverage exposure?
- How are claims distributed across settled, pending, and rejected statuses?
- Which policy types contribute the most premium and claim amounts?
- How does claim activity vary across customer age groups?
- What does customer feedback indicate about service quality and claims experience?
- Where are there potential opportunities to improve claims handling and customer experience?

## Objectives

- Analyze the insurance policy portfolio and financial metrics.
- Evaluate claim volumes and claim outcomes.
- Compare premium and claim performance across policy types.
- Examine claim amounts across customer age groups.
- Provide policy-level claim and customer details through an interactive detail view.
- Analyze customer feedback and sentiment to identify experience-related themes.

## Dataset

### Insurance Data

The main dataset contains **10,000 insurance policy records** and 13 fields.

| Field | Description |
|---|---|
| PolicyNumber | Unique policy identifier |
| CustomerID | Customer identifier |
| Gender | Customer gender |
| Age | Customer age |
| PolicyType | Type of insurance policy |
| PolicyStartDate | Policy start date |
| PolicyEndDate | Policy end date |
| PremiumAmount | Premium paid for the policy |
| CoverageAmount | Coverage associated with the policy |
| ClaimNumber | Claim identifier |
| ClaimDate | Claim date |
| ClaimAmount | Claim amount |
| ClaimStatus | Claim outcome/status |

### Customer Feedback Data

The customer feedback dataset contains **97 feedback records** with customer name, feedback text, sentiment, and sentiment score.

## Key Findings

### Portfolio & Financial Exposure

- **10,000** insurance policies were analyzed.
- Total premium amount was approximately **$5.97M**.
- Total coverage amount was approximately **$600.33M**.
- Total claim amount was approximately **$16.90M**.
- Average premium per policy was approximately **$597**.

### Claim Outcomes

| Claim Status | Records | Share |
|---|---:|---:|
| Rejected | 4,354 | 43.54% |
| Settled | 3,386 | 33.86% |
| Pending | 2,260 | 22.60% |

Rejected claims represent the largest claim-status category in the dataset, followed by settled and pending claims.

### Policy Type

Travel policies represent the largest share of the portfolio at **41.45%**, followed by:

- Health — 20.00%
- Auto — 15.94%
- Life — 12.48%
- Home — 10.13%

Travel also has the highest total premium and claim amount among the policy types in the dataset.

### Customer Feedback

The feedback dataset contains:

- **69 positive** responses
- **18 neutral** responses
- **10 negative** responses

Positive feedback is the dominant sentiment category, while negative and neutral comments reveal recurring themes around claim-processing delays, customer-service responsiveness, policy clarity, billing issues, and website/account accessibility.

## Power BI Dashboard

### Page 1 — Insurance Overview

The main dashboard provides a high-level view of the insurance portfolio, including:

- Active vs. inactive policy distribution
- Total premium amount
- Total coverage amount
- Total claim amount
- Gender distribution
- Claim status distribution
- Premium amount by policy type
- Claim amount by age group
- Policy type and claim-status analysis

Interactive policy and customer selectors allow the dashboard to be filtered for focused analysis.

### Page 2 — Policy & Claim Details

A detailed table provides policy- and claim-level information, including policy number, customer ID, claim number, age, gender, coverage, premium, policy dates, policy type, claim status, claim date, claim amount, age group, and active/inactive status.

This page is designed for detailed record-level investigation after identifying patterns on the overview page.

### Page 3 — Customer Feedback & Sentiment

The customer experience page analyzes the 97 customer feedback records through:

- Sentiment distribution
- Customer feedback details
- Sentiment classification
- Qualitative review of customer comments

The analysis connects operational insurance metrics with customer experience observations.

## Business Insights

1. **Travel insurance is the largest portfolio segment**, accounting for more than 40% of policy records and generating the highest premium and claim amounts.
2. **Rejected claims form the largest claim-status category**, highlighting an area that warrants deeper investigation into rejection reasons and claims processes.
3. **Claim exposure is concentrated in the largest policy segments**, particularly Travel and Health.
4. **Customer feedback is predominantly positive**, but negative and neutral comments reveal recurring themes around response times, claim processing, policy complexity, and digital accessibility.
5. Combining quantitative claims data with qualitative customer feedback provides a broader view of both operational performance and customer experience.

> These findings describe patterns in the dataset and should not be interpreted as causal conclusions.

## Tools & Skills

- Microsoft Power BI
- Data Analysis
- Data Visualization
- Data Modeling
- Business Intelligence
- Insurance Analytics
- Claims Analysis
- Customer Experience Analysis
- Sentiment Analysis
- Financial Analysis

## Project Structure

```text
insurance-customer-claims-analysis/
├── data/
│   ├── Insurance_Data.csv
│   └── Insurance_Customer_Feedback.xlsx
├── powerbi/
│   └── Insurance_Customer_Claims_Analysis.pbix
├── screenshots/
│   ├── insurance-overview.png
│   ├── policy-claim-details.png
│   └── customer-feedback-sentiment.png
├── .gitignore
└── README.md
```

## Key Takeaway

This project demonstrates how Power BI can combine portfolio-level insurance metrics, claim analysis, detailed policy investigation, and customer feedback to support data-driven decision making across insurance operations and customer experience.

## Disclaimer

This project is intended for portfolio and educational purposes. The analysis is based on the provided dataset and should not be interpreted as professional insurance, financial, or actuarial advice.
