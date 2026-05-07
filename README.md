# Pokémon Pack Value Analysis

## Overview

This project explores the expected value of opening Pokémon card packs using real-world pricing data and simulation.

The goal was to answer a simple question:

> Is opening Pokémon packs actually profitable?

To answer this, I built a Monte Carlo simulation in Python and visualized the results to better understand the risk and reward dynamics.

---

## Approach

The project combines data cleaning, feature engineering, and simulation modeling:

- Cleaned and transformed raw pricing data
- Mapped card prices into rarity tiers
- Simulated thousands of pack openings
- Analyzed expected value and profit distribution

This approach allows for a more realistic understanding of pack value beyond simple averages.

---

## Methodology

### Data Preparation
- Removed currency symbols and cleaned numeric fields
- Standardized price data for analysis

### Feature Engineering
Cards were grouped into value-based rarity tiers:
- Common
- Uncommon
- Rare
- Holo
- Ultra Rare
- Secret Rare

### Simulation
- Modeled pack composition using realistic rarity probabilities
- Assigned value based on average price per rarity tier
- Ran thousands of simulations to estimate outcomes

---

## Results

- **Expected Value per pack:** ~$2.85  
- **Average Profit per pack:** ~$-2.15  

### Key Insight

Although the expected value is negative, the distribution of outcomes is highly skewed.

Most packs result in a loss, but occasional high-value pulls create the perception of profitability.

This reflects a lottery-style dynamic where:
- losses are frequent  
- wins are rare but impactful  

---

## Visualization

A Power BI dashboard was created to visualize:

- Profit distribution per pack
- Expected value
- Probability of profit
- Value contribution by rarity tier

---

## Project Structure

```bash
pokemon-pack-analysis/
├── data/                # Dataset placeholder (see README in folder)
│   └── README.md
├── notebooks/           # Analysis and modeling
│   └── pokemon_pack_analysis.ipynb
├── powerbi/             # Dashboard files
├── README.md
└── .gitignore
```

---

## Data

Datasets are not included in this repository due to size limitations.

You can download the data from Kaggle:
- https://www.kaggle.com/datasets/jacklacey/pokemon-trading-cards
- https://www.kaggle.com/datasets/adampq/pokemon-tcg-all-cards-1999-2023

After downloading, place the CSV files in the `data/` folder before running the notebook.

---

## Tools Used

- Python (pandas, numpy, matplotlib)
- Jupyter Notebook
- Power BI
- Git & GitHub

---

## Key Takeaways

- Expected value does not reflect perceived value
- Distribution shape matters more than averages
- Simulation is effective for modeling uncertainty
- Clear data storytelling makes insights actionable

---

## Final Thoughts

This project demonstrates how data can challenge intuition and uncover the true structure behind everyday decisions.

It also highlights the importance of combining technical analysis with clear communication.
