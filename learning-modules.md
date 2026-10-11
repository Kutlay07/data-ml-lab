# Learning Modules

This checklist tracks progress through [`roadmap.md`](roadmap.md). Module numbers describe learning order, not a daily schedule. A module may take a few hours, a day, or several days. Move on when the core idea is understood and the small deliverable is complete—not just because time passed.

## How to use this checklist

- Check a module only when its goal has been met and its work is saved in the repository.
- Keep short notes in the module's project README or notebook; avoid turning this file into a second roadmap.
- If a module grows too large, record unfinished items as future work and keep the core scope manageable.
- Use English for project READMEs and practice explaining findings in English. Turkish explanations are always fine during learning.

## Phase 1 — Real Data Foundations

- [ ] 01 — Explore a market dataset: columns, types, missing values, distributions, suspicious values, and timestamps.
- [ ] 02 — Clean messy market data: duplicates, invalid dates, malformed values, impossible prices, and inconsistent tickers.
- [ ] 03 — Build a reusable data-quality auditor and automatic report.
- [ ] 04 — Recreate part of the pipeline in Polars and compare it with pandas.
- [ ] 05 — Analyze cleaned data in Excel: filters, sorting, PivotTables, XLOOKUP, conditional formatting, charts, and a summary sheet.

## Phase 2 — SQL and Analyst Core

- [ ] 06 — SQL basics with the project dataset in SQLite or PostgreSQL.
- [ ] 07 — Intermediate SQL: joins, CTEs, CASE, and subqueries.
- [ ] 08 — Analytical SQL: window functions and time-aware calculations.
- [ ] 09 — Analyst case study: answer one research question with SQL, Python, Excel, visualizations, and a concise written conclusion.

## Phase 3 — Applied Statistics

- [ ] 10 — Descriptive statistics applied to real data.
- [ ] 11 — Sampling, confidence intervals, and bootstrapping.
- [ ] 12 — Hypothesis testing, including effect size and interpretation.
- [ ] 13 — Regression analysis: coefficients, residuals, assumptions, and interpretation.

## Phase 4 — Multi-Source Data

- [ ] 14 — Join company metadata to market data; practice entity resolution.
- [ ] 15 — Add and inspect fundamental financial data.
- [ ] 16 — Add macroeconomic data and align sources carefully in time.

## Phase 5 — Predictive Machine Learning

- [ ] 17 — Establish simple baselines, then compare with Logistic Regression.
- [ ] 18 — Train and compare tree-based models using suitable metrics.
- [ ] 19 — Create and document features such as lagged returns and rolling volatility.
- [ ] 20 — Explain model behavior with feature and permutation importance; try SHAP if useful.

## Phase 6 — Robust ML Evaluation

- [ ] 21 — Demonstrate data leakage, remove it, and explain the difference in results.
- [ ] 22 — Use chronological splits and implement walk-forward validation.
- [ ] 23 — Compare data across time and investigate distribution shift and drift.

## Phase 7 — Data Pipeline Engineering

- [ ] 24 — Build a repeatable extract, validate, clean, transform, and load pipeline.
- [ ] 25 — Add logging, error handling, retries, idempotency, and configuration.

## Phase 8 — ML Engineering

- [ ] 26 — Create reproducible training that saves a model, metrics, and configuration.
- [ ] 27 — Serve predictions through a FastAPI endpoint with input validation and error handling.
- [ ] 28 — Package the service with Docker and add useful tests.

## Phase 9 — CI/CD, Terraform, and AWS

- [ ] 29 — Create a GitHub Actions workflow for linting, tests, and a Docker build.
- [ ] 30 — Describe infrastructure with Terraform; practice formatting, validation, and planning.
- [ ] 31 — Deploy a small service to AWS if a suitable low-cost or credited option is available; inspect logs and health.

## Phase 10 — End-to-End Flagship Project

- [ ] 32 — Choose a focused research question and define data and evaluation boundaries.
- [ ] 33 — Build ingestion, validation, analysis, and modeling stages.
- [ ] 34 — Package and deploy the model service with CI/CD and infrastructure configuration.
- [ ] 35 — Add basic monitoring, document limitations, and prepare the portfolio presentation.

## Optional advanced ML extension

Do this after the core ML modules, when the learner can already explain training, automatic differentiation, evaluation, and why a framework is useful. It is an extension, not a prerequisite for completing the roadmap.

- [ ] 36 — Learn JAX fundamentals: arrays, transformations, automatic differentiation, and JIT compilation.
- [ ] 37 — Reimplement a small learning exercise in JAX and compare its behavior and trade-offs with a familiar tool.

## Module notes

For each module, keep a brief record in its project folder:

```text
What I built:
What I learned:
What confused me:
What I would improve:
```
