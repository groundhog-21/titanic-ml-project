# Gold Model: RFC_FamSz_Baseline

**Date:** 2023-09-09  
**Public LB Score:** 0.78229  
**Rank:** ~76th percentile  
**Model:** RandomForestClassifier + GridSearchCV  

## Why this model matters
This is the highest LB score achieved to date.
Despite later, more complex pipelines, this model remains the best.

## Feature set
- Pclass
- Sex
- Age (imputed)
- SibSp
- Parch
- Embarked
- FamSz

## Key insight
Simple, low-noise family structure features outperform complex social proxies
(Titles, Tickets, CabinDeck).

## Reproduction
Run:
`notebooks/gold/all-time_high_score_titanic_1_really.ipynb`