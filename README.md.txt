# Adverse Selection & Dynamic Repricing Simulation in R

## Overview
An actuarial simulation modeling the Rothschild-Stiglitz adverse selection death spiral in a health insurance pool of 1,000 policyholders.

## Actuarial Methodology
- **Collective Risk Model:** Claim frequency modeled via Poisson distributions; claim severity modeled via Gamma distributions (Compound Poisson-Gamma framework).
- **Pricing Framework:** Community-rated office premiums derived via the classical Equivalence Principle with a 15% expense loading.
- **Dynamic Lapsing:** Simulates price-elasticity lapse dynamics where low-risk cohorts exit upon premium mispricing.

## Key Findings
- **Baseline Pool:** 1,000 lives (600 low-risk, 400 high-risk).
- **Shock:** 100% low-risk cohort attrition due to community rate disparity.
- **Result:** Required office premium spiked by **134.7%** in Year 2 to maintain pool solvency.

## Execution
Run `adverse_selection_simulation.R` in R or RStudio. Seed is fixed (`set.seed(108)`) for exact reproducibility.