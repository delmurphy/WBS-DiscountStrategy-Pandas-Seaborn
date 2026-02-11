# Eniac Discount Strategy — Data Analysis Case Study

### Python: Pandas & Seaborn | WBS Data Science Bootcamp Project 2

--------------------------------------

## Project Overview

This project is a business-driven data analysis case study conducted as part of the **WBS Data Science bootcamp**. The goal is to help **Eniac**, a European e-commerce company, evaluate whether offering product discounts is an effective strategy for driving growth without harming revenue.

Within Eniac, there is an ongoing strategic debate:

- The **Marketing Team** believes discounts improve customer acquisition, satisfaction, and retention.
- The **Board and main investors** are concerned that discounts increase order volume while reducing total revenue and weakening Eniac’s premium positioning.

Using Eniac’s internal sales and pricing data, this project analyzes pricing structures, discount behavior, and seasonality effects to assess **when and whether discounts are beneficial**.

The final outcome is a **concise, data-driven presentation (5 minutes)** aimed at Eniac’s board, clearly communicating insights, limitations, and recommendations.

---

## Tools Used

- **Python (Pandas)**  
  Used for data cleaning, transformation, and exploratory analysis of Eniac’s internal datasets.

- **Seaborn & Matplotlib**  
  Used to create visualizations that illustrate price distributions, discount patterns, and seasonal trends.

- **Google Colab & VSCode**  
  Development environments for collaborative analysis and reproducibility.

- **Google Slides**  
  Used to present findings and recommendations as the Eniac Data Analytics Team.

---

## Project Files

- **Presentation file:** `Eniac_Discount_Strategy.pdf`  
  A PDF of the final presentation to the board, summarizing key findings, insights, and recommendations regarding product discounts.

- **Notebooks folder:** `notebooks/`  
  Python notebooks containing:
  - Data quality assessment
  - Data cleaning steps
  - Exploratory analysis
  - Visualizations supporting the final conclusions

- **Data folder:** `data/`  
  Raw and cleaned versions of Eniac’s internal datasets used in the analysis.

---

## How to Use the Files

- **Review the presentation**  
  The presentation provides a high-level summary of the business problem, analytical findings, and final recommendations.

- **Explore the notebooks**  
  The notebooks document the full analytical workflow, from data cleaning to insight generation.

- **Inspect the data**  
  The data folder includes both raw and cleaned datasets, highlighting common real-world data quality issues.

## Environment Setup

This project was developed using Python 3.13.

To recreate the environment:

```bash
python -m venv .venv

# macOS / Linux
source .venv/bin/activate

# Windows
.venv\Scripts\activate

pip install -r requirements.txt
```

---

## Summary of Key Insights

### Price Structure Is Highly Variable

- Product prices vary **significantly across and within categories**
- Some categories include both low- and high-priced products, making category-level averages potentially misleading
- Careful product classification is required to support reliable pricing and discount analysis

### Discounts Are Widely Used

- **Most products have been discounted at some point**
- Typical discounts cluster around **~15% of the product price**
- Discounting appears to be a common tactic rather than an exception

### Discounts and Seasonality Matter More Than Discount Size

- **November 2017**
  - A slight increase in discounts coincided with **higher order volume and increased revenue**
  - The effect was particularly strong around **Black Friday and Cyber Monday**

- **March 2018**
  - Similar discount levels coincided with **lower orders and reduced revenue**
  - Suggests that discounts alone do not drive demand outside peak shopping periods

These patterns indicate that **timing and context** play a critical role in determining whether discounts are effective.

---

## Recommendations

### Avoid Aggressive Discounting

- Refrain from applying large or blanket discounts across all products
- Be especially cautious with:
  - Categories that show **wide price dispersion**
  - Categories with **low sales volume share**
- In these cases, aggressive discounts risk eroding revenue without delivering meaningful volume gains

### Adopt a Test-Driven Discount Strategy

- Implement **explicit testing** (e.g. A/B testing) to evaluate how discounts affect:
  - Sales volume
  - Revenue
  - Customer acquisition
  - Customer satisfaction
  - Customer retention
- Use controlled experiments to separate:
  - Seasonal effects
  - Promotional uplift
  - Long-term customer value

---

## Limitations & Data Quality Considerations

- The dataset contained multiple inconsistencies, requiring extensive cleaning
- Results reflect **correlations, not causation**
- Limited customer-level and margin data restrict deeper profitability analysis

Improving data pipelines and tracking would significantly increase confidence in future pricing decisions.

---

## Overall Takeaway

- Discounts can be effective when aligned with **high-intent seasonal events**
- Outside peak periods, discounts may increase risk without improving performance
- A **targeted, data-driven, and test-based discount strategy** is preferable to aggressive or continuous discounting
- Better data quality and experimentation are essential to making discounts a reliable growth lever for Eniac
