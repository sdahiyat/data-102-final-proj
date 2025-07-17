# Modeling Residential Energy Usage in the U.S.

**Team members**: Mira Bhatt, Hannah Brown, Sierra Dahiyat, Sophia Chan

---

## Overview

This project explores patterns in residential electricity usage across the United States, with a focus on how **home energy assistance programs** impact consumption. Using a combination of **exploratory data analysis**, **causal inference**, and **Bayesian hierarchical modeling**, we examine geographic variation in energy usage at both the state and region levels.

Our goal is to identify causal relationships and uncover latent structure in energy consumption that may be influenced by socioeconomic factors and federal energy programs.

---

## Repository Contents

| File                          | Description                                                                 |
|-------------------------------|-----------------------------------------------------------------------------|
| `EDA.ipynb`                   | Exploratory data analysis. Includes visualization of energy consumption patterns across states and regions, and highlights features that informed our modeling decisions. |
| `Causal_Inference.ipynb`      | Investigates the impact of home energy assistance using inverse propensity weighting to estimate causal effects. |
| `bayesian_hierarchical_model.ipynb` | Implements a three-level Bayesian model (state → division → region). Includes posterior predictive plots, sampling diagnostics, and model evaluation. |
| `recs2020_public_v7.csv`      | Public-use microdata from the U.S. Energy Information Administration’s Residential Energy Consumption Survey (RECS 2020). Used as the primary dataset. |

---

## How to Run

Each notebook is standalone but builds upon the previous one:

1. **Start with `EDA.ipynb`** to understand the dataset and key features.
2. **Continue with `Causal_Inference.ipynb`** to explore causal effects of energy assistance programs.
3. **Run `bayesian_hierarchical_model.ipynb`** for the full generative modeling and inference.

All notebooks assume access to `recs2020_public_v7.csv` in the working directory.

---

## Environment Requirements

Install dependencies with:

```bash
pip install numpy pandas matplotlib seaborn pymc arviz
