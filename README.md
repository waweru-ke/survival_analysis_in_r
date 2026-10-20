# Survival Analysis in R

A small R project exploring **time-to-event data** using the `lung` dataset from the `survival` package.

The goal is to practise the core ideas behind survival analysis: estimating survival over time, comparing groups, and modelling how a predictor relates to the hazard of an event.

## What’s Covered

- Preparing event-status and date variables
- Kaplan–Meier survival estimation
- Visualising survival curves with confidence intervals and risk tables
- Estimating one-year and median survival
- Comparing male and female survival using the log-rank test
- Fitting and interpreting a Cox proportional hazards model

## A Few Results

Using the example dataset:

- Estimated **1-year survival:** 41% (95% CI: 34%–49%)
- Estimated **median survival:** 310 days (95% CI: 285–363)
- The log-rank test indicated a difference in survival curves by sex (*p* = 0.001).
- In the Cox model with sex as the predictor, the estimated hazard ratio was approximately **0.59** per one-unit increase in the sex variable.

These are results from an instructional analysis of the built-in dataset, not conclusions intended to generalise beyond it.

## Tools

- R
- `survival`
- `dplyr`
- `lubridate`
- `ggsurvfit`
- `gtsummary`
- `tibble`
- `knitr`
- `tidycmprsk`

## Run It

1. Install R and [Quarto](https://quarto.org/).
2. Install the packages listed above if they are not already installed.
3. Open `tutorial.qmd` in RStudio or run:

   ```bash
   quarto render tutorial.qmd
   ```

The document uses the `lung` dataset included with the `survival` package.

## Project Files

```text
survival-analysis-in-r/
├── README.md
└── tutorial.qmd
```
