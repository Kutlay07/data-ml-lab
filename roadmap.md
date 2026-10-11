# Data + ML + MLOps Roadmap

## Goal

Build a strong hands-on foundation for:

- Data Analyst internships
- Data Scientist internships
- ML Engineer internships
- AI Engineer internships
- Quant / Financial Data roles
- Production ML / MLOps

Kutlang remains the main AI engineering project.

This side-project roadmap focuses on:

- messy real-world data
- SQL
- Excel
- statistics
- machine learning
- data pipelines
- deployment
- Docker
- GitHub Actions
- Terraform
- AWS
- monitoring
- production ML

---

# Phase 1 — Get Comfortable With Real Data

## Day 1 — Dataset Exploration

Download a market dataset and inspect:

- columns
- data types
- missing values
- distributions
- suspicious values
- timestamps
- categorical inconsistencies

Use:

- pandas
- NumPy
- `info()`
- `describe()`

### Goal

> Understand a dataset before modifying or modeling it.

---

## Day 2 — Market Data Cleaner

Clean deliberately messy data.

Handle:

- missing values
- duplicate rows
- invalid timestamps
- malformed numeric values
- impossible prices
- inconsistent ticker names
- inconsistent date formats
- corrupted rows

### Goal

> Turn raw data into a trustworthy analytical dataset.

---

## Day 3 — Data Quality Auditor

Build reusable data-quality checks.

Implement:

- schema validation
- null-rate checks
- duplicate detection
- range validation
- data type validation
- timestamp continuity checks
- outlier detection
- row-count comparisons

Generate an automatic quality report.

### Goal

> Detect bad data automatically instead of inspecting everything manually.

---

## Day 4 — pandas vs Polars

Repeat part of the data pipeline using Polars.

Compare:

- syntax
- execution time
- memory usage
- developer ergonomics

### Goal

> Become comfortable with modern dataframe tooling and basic performance thinking.

---

## Day 5 — Excel Analysis

Export the cleaned dataset to Excel.

Practice:

- filtering
- sorting
- PivotTables
- XLOOKUP
- conditional formatting
- charts
- summary sheets

### Goal

> Build practical Data Analyst workflow skills.

---

# Phase 2 — SQL and Data Analyst Core

## Day 6 — SQL Basics

Load the cleaned dataset into:

- SQLite or
- PostgreSQL

Practice:

```sql
SELECT
WHERE
GROUP BY
ORDER BY
HAVING
```

Use your own financial dataset instead of tutorial databases.

### Goal

> Query real project data with SQL.

---

## Day 7 — Intermediate SQL

Practice:

```sql
JOIN
CTE
CASE WHEN
SUBQUERY
```

Example questions:

- What is the average return by sector?
- Which companies have the highest volatility?
- Which industries have the strongest momentum?

### Goal

> Combine tables and answer meaningful analytical questions.

---

## Day 8 — Analytical SQL

Practice window functions:

```sql
ROW_NUMBER()
RANK()
LAG()
LEAD()
AVG() OVER(...)
SUM() OVER(...)
```

### Goal

> Become comfortable with SQL patterns used in real analyst work.

---

## Day 9 — Analyst Case Study

Choose one business or research question.

Example:

> Which sectors experienced the largest increase in risk over the last 12 months?

Use:

- SQL
- Python
- Excel
- visualization

Produce:

- 3 meaningful charts
- short written analysis
- clear conclusion

Avoid producing 10 charts with no interpretation.

### Goal

> Learn data storytelling and decision-support analysis.

---

# Phase 3 — Applied Statistics

## Day 10 — Descriptive Statistics

Practice:

- mean
- median
- variance
- standard deviation
- percentiles
- skewness
- correlation
- covariance

Apply everything directly to real data.

### Goal

> Understand distributions instead of only training models.

---

## Day 11 — Sampling and Confidence Intervals

Practice:

- sampling
- confidence intervals
- bootstrapping

Example:

> Estimate a confidence interval for the average return of a sector.

### Goal

> Understand uncertainty in statistical estimates.

---

## Day 12 — Hypothesis Testing

Create a real hypothesis.

Example:

> Is technology-sector volatility significantly different from utilities-sector volatility?

Work through:

- null hypothesis
- alternative hypothesis
- test selection
- p-value
- effect size
- interpretation

### Goal

> Build practical statistical inference skills.

---

## Day 13 — Regression Analysis

Use linear regression.

Inspect:

- coefficients
- residuals
- assumptions
- statistical significance
- interpretation

Do not use regression only for prediction.

### Goal

> Understand regression as both an analytical and predictive tool.

---

# Phase 4 — Multi-Source Real Data

Price data alone is not enough.

The goal of this phase is to work with multiple heterogeneous datasets.

---

## Day 14 — Company Metadata

Combine market data with:

- ticker
- sector
- industry
- market cap
- exchange

Practice joins and entity resolution.

### Goal

> Learn how multiple datasets connect around business entities.

---

## Day 15 — Fundamental Data

Add:

- revenue
- earnings
- P/E
- cash flow
- debt
- valuation ratios

### Goal

> Work with financial statement and company-level data.

---

## Day 16 — Macro Data

Add:

- interest rates
- inflation
- market indexes
- unemployment
- other macro indicators

Final dataset:

```text
Market Data
+
Company Fundamentals
+
Macroeconomic Data
```

### Goal

> Build a realistic multi-source analytical dataset.

---

# Phase 5 — Predictive Machine Learning

## Day 17 — Baselines

Create simple baselines first.

Examples:

```text
Tomorrow = Today
```

or:

```text
Majority Class
```

Then train Logistic Regression.

### Goal

> Determine whether machine learning actually adds value over simple heuristics.

---

## Day 18 — Tree-Based Models

Train:

- Random Forest
- XGBoost or LightGBM

Compare:

- accuracy
- precision
- recall
- F1
- ROC-AUC

Do not optimize only for accuracy.

### Goal

> Compare multiple model families and evaluation metrics.

---

## Day 19 — Feature Engineering

Create features such as:

- lagged returns
- rolling volatility
- moving averages
- volume changes
- financial ratios
- macro features

### Goal

> Learn how useful predictive signals are created from raw data.

---

## Day 20 — Explainability

Use:

- feature importance
- permutation importance
- SHAP

Ask:

> Why did the model make this prediction?

### Goal

> Improve model interpretability and Data Scientist reasoning.

---

# Phase 6 — Robust ML Evaluation

## Day 21 — Data Leakage Lab

Intentionally create leakage.

Observe unrealistically strong model performance.

Then remove the leakage.

Compare the results.

### Goal

> Build strong intuition for data leakage and false model performance.

---

## Day 22 — Time-Series Validation

Avoid random train/test splits.

Example:

```text
TRAIN
2018–2023

VALIDATION
2024

TEST
2025
```

Then implement:

- walk-forward validation

### Goal

> Learn correct temporal model evaluation.

---

## Day 23 — Distribution Shift and Drift

Compare feature distributions across time.

Example:

```text
2018 Data
vs
2026 Data
```

Practice:

- histogram comparison
- KS test
- PSI
- drift detection concepts

### Goal

> Understand how production models degrade as the data distribution changes.

---

# Phase 7 — Data Pipeline Engineering

This phase is not about becoming a Data Engineer.

It teaches the amount of data engineering that a strong Data Scientist or ML Engineer should know.

---

## Day 24 — ETL Pipeline

Automate:

```text
Download Raw Data
        ↓
Validate
        ↓
Clean
        ↓
Transform
        ↓
Load Into Database
```

Run everything with:

```bash
python pipeline.py
```

### Goal

> Move from notebook-based work to reproducible data pipelines.

---

## Day 25 — Reliable Data Pipelines

Add:

- logging
- error handling
- retries
- idempotency
- configuration management

### Goal

> Build production-minded data workflows.

---

# Phase 8 — ML Engineering

## Day 26 — Reproducible Training

Create:

```bash
python train.py
```

Outputs:

```text
model.pkl
metrics.json
config.json
```

Make training reproducible.

### Goal

> Separate experimentation from production training code.

---

## Day 27 — FastAPI Inference Service

Create an inference endpoint:

```http
POST /predict
```

Example request:

```json
{
  "features": []
}
```

Implement:

- request validation
- model loading
- prediction generation
- error handling

### Goal

> Serve the trained model as an application.

---

## Day 28 — Docker and Testing

Add:

- Dockerfile
- pytest
- reproducible environment

Run:

```bash
docker build .
docker run ...
pytest
```

### Goal

> Turn the model into a testable and portable ML service.

---

# Phase 9 — CI/CD + AWS + Terraform

Terraform should exist from the beginning of the roadmap where useful.

Example structure:

```text
infra/
├── main.tf
├── variables.tf
└── outputs.tf
```

Even without a real AWS deployment, practice:

```bash
terraform fmt
terraform validate
terraform plan
```

---

## Day 29 — GitHub Actions

Create a CI pipeline:

```text
Git Push
   ↓
Lint
   ↓
Tests
   ↓
Docker Build
```

### Goal

> Learn basic CI/CD.

---

## Day 30 — Terraform Infrastructure

Design infrastructure using:

- S3
- IAM
- ECR
- compute
- basic networking

Practice:

```bash
terraform init
terraform validate
terraform plan
```

### Goal

> Learn Infrastructure as Code.

---

## Day 31 — AWS Deployment

Use one of:

- AWS Educate
- AWS sandbox
- AWS free resources
- available credits

Deploy the application if possible.

Inspect:

- application logs
- CloudWatch
- requests
- failures
- health

### Goal

> Gain real cloud deployment experience.

---

# Phase 10 — End-to-End Flagship Project

## Days 32–35

Build one complete system using everything learned so far.

Possible research questions:

> Can company earnings growth be predicted using market, fundamental, and macroeconomic data?

or:

> Can financial volatility be forecast using market and macroeconomic features?

System architecture:

```text
Multiple Data Sources
        ↓
Data Ingestion
        ↓
Validation
        ↓
Cleaning
        ↓
SQL Database
        ↓
EDA
        ↓
Statistical Analysis
        ↓
Feature Engineering
        ↓
Machine Learning
        ↓
Evaluation
        ↓
Model Artifact
        ↓
FastAPI
        ↓
Docker
        ↓
GitHub Actions
        ↓
Terraform
        ↓
AWS
        ↓
Monitoring
```

### Goal

> Build a portfolio-quality end-to-end Data Science and ML Engineering system.

This is the project that should become the strongest portfolio piece.

Earlier projects can remain smaller learning labs.

---

# Rules for Every Project

## Development Rules

- Do not create notebook graveyards.
- Exploration notebooks are fine.
- Final reusable logic should move into `src/`.
- Do not blindly copy tutorials.
- Learn a concept, then apply it to your own dataset.
- Use Git from the beginning.
- Write README files in English.
- Add tests where they provide real value.
- Use Terraform where infrastructure is relevant.
- Keep projects small enough to finish.
- Prefer finishing over endless polishing.
- If something becomes too large, write it down as future work and continue.

---

## Data Rules

Prefer real messy datasets.

Look for problems such as:

- missing values
- duplicate rows
- inconsistent categories
- invalid data types
- incorrect timestamps
- malformed values
- impossible values
- outliers
- inconsistent schemas
- data-source mismatches
- broken joins
- temporal alignment issues
- data leakage

If the dataset is unrealistically clean, inject realistic corruption and test whether the cleaning and validation pipeline detects it.

---

## Analysis Rules

Do not ask only:

> What accuracy did the model achieve?

Also ask:

- Why did the result happen?
- Is the result statistically meaningful?
- Is there leakage?
- Is the validation strategy correct?
- Can the result generalize?
- What assumptions are being made?
- What are the limitations?
- What decision could someone make from this analysis?

---

# Project Report Template

After completing a project, report:

```text
Project:

What I built:

What I learned:

What confused me:

Results:

Mistakes:

GitHub:
```

Then perform a senior-style review of:

- data methodology
- code quality
- statistics
- ML evaluation
- leakage
- testing
- architecture
- documentation
- portfolio quality

---

# Target Skill Coverage

## Data Analyst

Develop:

- SQL
- Excel
- pandas
- visualization
- dashboarding
- KPI analysis
- business questions
- data storytelling
- analytical communication

---

## Data Scientist

Develop:

- messy-data handling
- data cleaning
- EDA
- statistics
- hypothesis testing
- regression
- classification
- feature engineering
- machine learning
- model evaluation
- explainability
- multi-source data
- leakage detection
- time-series validation
- experiment design

---

## ML Engineer

Develop:

- reproducible training
- training pipelines
- testing
- model artifacts
- inference APIs
- FastAPI
- Docker
- CI/CD
- monitoring
- AWS
- Terraform
- production ML

---

## Quant / Financial Data Exposure

Develop:

- market data
- financial statements
- returns
- volatility
- time-series
- macroeconomic data
- noisy financial datasets
- temporal validation
- financial feature engineering

---

# Main Career Structure

```text
Kutlang
   ↓
AI Engineering
Software Engineering
Agent Systems
LLM Systems

Side Projects
   ↓
Data Analyst
Data Scientist
ML Engineer
Quant Exposure

AWS + Terraform + CI/CD
   ↓
Production Engineering
MLOps

Tiny Model Experiments
   ↓
Research Engineering
```

---

# Final Objective

At the end of this roadmap, the target is to be able to say:

> I can take messy real-world data, validate and clean it, analyze it using SQL and statistics, build machine-learning models, evaluate them correctly, productionize them, deploy them, and monitor them.

Target internship families:

- Data Analyst Intern
- Data Scientist Intern
- Machine Learning Engineer Intern
- Applied AI Engineer Intern
- AI Engineer Intern
- Financial Data / Quant Data roles
