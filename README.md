# Global Alcohol Consumption Analysis (2000-2022)

## Project Overview

This project analyses global alcohol consumption patterns across 196+ countries over a 23-year period (2000-2022) to identify optimal markets for international beverage expansion. 

**Business Context:** This analysis was conducted as a personal project simulating a strategic market entry study for an international alcohol beverage company. The hypothetical stakeholder is the Head of Market Expansion, tasked with identifying which countries to prioritise for market entry, deeper investment, or deprioritisation.

**Objective:** To deliver data-driven recommendations that balance growth potential with market stability, enabling informed resource allocation and reducing the risk of entering volatile markets.

The analysis evaluates markets across five dimensions: global consumption trends, regional dynamics, country-level growth trajectories, market stability, and risk-return relationships.

---

## Business Questions

The analysis aims to answer the following key strategic questions:

1. **Are global alcohol consumption levels trending upward or downward overall?**
2. **How have regional alcohol consumption patterns evolved over time, and which regions are becoming more or less attractive markets?**
3. **Which countries have experienced the largest increases or decreases in alcohol consumption since 2000?**
4. **How stable are countries today, and which high-consumption markets are standout stable bets?**
5. **Do countries with higher average alcohol consumption also show greater year-to-year volatility in consumption?**

---

## Dataset

- **Source:** [WHO Global Alcohol Consumption Dataset (Kaggle)](https://www.kaggle.com/datasets/ibrahimqasimi/global-alcohol-consumption-who-20002022)
- **Time Period:** 2000-2022 (23 years of annual data)
- **Geographic Scope:** 196+ countries across all continents
- **Format:** CSV

The dataset was validated for completeness and accuracy before analysis. Data quality checks confirmed zero missing values, no negative consumption records, and valid year ranges across all 4,508 country-year observations.

---

## Tools and Technologies

- **Python** – Primary analysis language
- **Pandas & NumPy** – Data manipulation and statistical calculations
- **Matplotlib & Seaborn** – Data visualisation
- **Jupyter Notebook** – Interactive analysis environment
- **Git/GitHub** – Version control and project management
- **Microsoft Excel** – Initial data validation and sanity checks

---

## Data Cleaning and Preparation

**Purpose:** To ensure data integrity and prepare the dataset for robust statistical analysis whilst creating business-relevant metrics for stakeholder interpretation.

### Key Steps

1. **Data Quality Validation:** Verified absence of missing values, negative consumption records, and duplicate country-year combinations
2. **Feature Engineering:** Created derived metrics to improve business interpretability:
   - Converted annual litres to weekly UK standard units for easier comparison
   - Calculated percentage of UK recommended weekly guideline (14 units)
3. **Geographic Mapping:** Assigned continent classifications to all countries for regional trend analysis
4. **Baseline Calculations:** Established 2000 consumption levels as baseline for percentage change analysis

All data preparation was performed programmatically in Python to ensure reproducibility and transparency.

---

## Key Insights

### 1. **Global Market Contraction Requires Targeted Strategy**
   - **Problem:** Understanding whether to pursue broad market expansion or targeted entry
   - **Finding:** Global per capita consumption declined 3% (2000-2022), with a consistent downward trend (-0.0077L/year)
   - **So What:** Broad geographic expansion is not viable. Success requires identifying specific high-growth or high-volume markets that defy the global decline

### 2. **Regional Divergence Creates Clear Winners**
   - **Problem:** Which geographic regions offer the best opportunities?
   - **Finding:** Asia demonstrates strongest growth trajectory; Europe declining but remains highest volume market overall
   - **So What:** Prioritise Asia for growth-focused investment whilst maintaining European presence for stable volume and operational learning

### 3. **Exceptional Growth Markets Identified**
   - **Problem:** Which specific countries show transformational growth potential?
   - **Finding:** Mongolia (+180%), Viet Nam (+165%), and Congo (+134%) achieved explosive growth despite global headwinds
   - **So What:** These markets represent first-mover advantage opportunities with established upward trajectories, warranting feasibility studies for market entry

### 4. **Stable High-Volume Markets Provide Revenue Anchors**
   - **Problem:** Where can the company find predictable, reliable demand?
   - **Finding:** Czechia (14.02L avg, 0.44L volatility), Austria (12.35L, 0.44L), and Slovenia (11.66L, 0.50L) combine exceptional volume with low year-to-year fluctuation
   - **So What:** These mature European markets offer low-risk revenue foundations to balance more volatile growth investments

### 5. **Risk-Return Trade-off Demands Portfolio Approach**
   - **Problem:** Can high-volume markets also be low-risk?
   - **Finding:** Strong positive correlation (r=0.71, p<0.001) between consumption volume and volatility
   - **So What:** No single market type offers both scale and predictability. Success requires portfolio strategy balancing stable European anchors against high-growth emerging markets

---

## Project Value

This project demonstrates the ability to:

- **Translate business questions into analytical frameworks** – Converted strategic ambiguity into five testable hypotheses
- **Perform end-to-end data analysis** – From data validation through statistical testing to actionable recommendations
- **Apply statistical techniques appropriately** – Linear regression, correlation analysis (Spearman), volatility calculations, and hypothesis testing
- **Communicate insights to non-technical stakeholders** – Clear visualisations, executive summary, and business-focused language
- **Balance analytical rigor with practical constraints** – Acknowledged limitations whilst delivering decision-ready recommendations
- **Think strategically about business problems** – Developed portfolio approach balancing risk and opportunity

**Particularly relevant for internships:** The project showcases skills in exploratory data analysis, statistical thinking, data visualisation, and the ability to structure ambiguous problems—all critical for data analytics roles.

---

## Repository Contents

```
├── analysis.ipynb          # Complete Jupyter Notebook with analysis, visualisations, and commentary
├── who_alcohol.csv         # Raw WHO dataset (2000-2022 global alcohol consumption)
├── requirements.txt        # Python package dependencies
└── README.md              # Project documentation (this file)
```

---

## How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/Huang-Hao-Gao/global-alcohol-consumption-analysis.git
   cd global-alcohol-consumption-analysis
   ```

2. Install dependencies from `requirements.txt`:
   ```bash
   pip install -r requirements.txt
   ```

3. Open the Jupyter Notebook:
   ```bash
   jupyter notebook analysis.ipynb
   ```

4. Run all cells to reproduce the analysis

---

**Author:** Huang Hao Gao  
**Project Type:** Data Analytics Portfolio Project  
**Last Updated:** January 2026