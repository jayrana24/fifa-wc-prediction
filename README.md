# World Cup 2026 Prediction Project

A football analytics project that predicts World Cup 2026 team probabilities using Poisson models and Monte Carlo simulation.

## Purpose

The goal of this project is to estimate each team’s chance of reaching different stages of the 2026 FIFA World Cup, from the group stage to winning the tournament.

## What was done

* Collected and cleaned historical international football match data.
* Prepared the 2026 World Cup fixtures, group-stage structure, knockout bracket, FIFA ranking data, and confederation data.
* Built pre-match Elo ratings for teams.
* Created match-level features such as:

  * home Elo
  * away Elo
  * Elo difference
  * neutral venue
  * tournament weight
  * home and away confederations
* Trained two Poisson regression models:

  * one model for home-team goals
  * one model for away-team goals
* Converted expected goals into win, draw, and loss probabilities.
* Simulated:

   * group-stage matches
  * group tables
  * best third-placed teams
  * Round of 32 bracket
  * knockout rounds
  * full tournaments
* Ran Monte Carlo simulations to estimate stage probabilities.

## Tools used

* Python
* pandas
* NumPy  
* statsmodels
* uv
* Jupyter notebooks
* Matplotlib / pandas plotting

The 1,000-run Monte Carlo simulation showed that the model strongly favored teams with the highest Elo ratings, especially Argentina and Spain. The final results were saved to:

```text
processed/experiments/no_conf_clean_probs.csv

```

