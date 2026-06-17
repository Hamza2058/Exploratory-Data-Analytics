# 📚 Books Market Analysis — Sales, Pricing & Genre Performance

## Business Context

A book retail business wants to understand what drives sales performance across its catalogue of ~1,000 titles. With books spanning from 1901 to 2016 across multiple genres, languages, and price points, the business needs clarity on which genres generate the most reader engagement, how pricing affects volume, and which authors deliver the highest gross revenue. This analysis provides data-driven answers to inform procurement, pricing, and marketing decisions.

---

## Business Questions

1. Which publishing years dominate the catalogue — are recent or classic titles driving the business?
2. Which genres have the strongest reader engagement based on ratings volume?
3. How does sale price affect units sold — is there an optimal pricing range?
4. Which authors generate the highest gross sales revenue?
5. Which languages dominate the catalogue and what does that mean for market reach?

---

## Dataset Overview

| Property | Detail |
|---|---|
| Total Books | 988 (after cleaning) |
| Publishing Range | 1901 – 2016 |
| Genres | Fiction, Nonfiction, Children |
| Price Range | $0.99 – $33.86 |
| Languages | 8 language codes |
| Key Columns | Book Name, Author, Genre, Sale Price, Units Sold, Gross Sales, Book Ratings Count |

---

## Tools & Libraries

- **Python** — core analysis language
- **pandas** — data cleaning and manipulation
- **matplotlib** — charting and visualisations
- **seaborn** — statistical plots
- **numpy** — numerical operations

---

## Key Findings & Recommendations

**1. Modern titles dominate the catalogue**
The publishing year distribution is right-skewed, with the majority of books published post-1990. Recommendation: prioritise stocking recent titles in procurement cycles while maintaining a selective catalogue of high-performing classics.

**2. Fiction drives volume, but Nonfiction has untapped potential**
Fiction accounts for 82% of catalogue titles (813 books) vs Nonfiction at 16% (160 books). However, rating counts across genres show strong engagement pockets in Nonfiction. Recommendation: expand Nonfiction inventory selectively in high-engagement sub-categories to diversify revenue streams.

**3. Lower-priced books sell in higher volumes**
The scatter plot of sale price vs units sold shows a negative relationship — books priced under $10 consistently outsell higher-priced titles. Recommendation: for new catalogue additions, an entry price point of $7–$10 is likely to maximise volume without significantly compressing margin.

**4. Top 3 authors account for disproportionate gross sales**
Harper Lee ($47,795), Stephen King ($43,323) and David Sedaris ($42,323) are the top gross revenue generators. Recommendation: ensure these authors' catalogues are always fully stocked and featured prominently in marketing materials.

**5. English dominates — 8 languages represent a growth opportunity**
The catalogue is heavily English-language focused. With 8 language codes present, there is an opportunity to expand into underserved language markets with targeted, lower-cost digital offerings.

---

## Project Structure

```
books-market-analysis/
│
├── EDA_Books_dataset.ipynb   # Main analysis notebook
├── Books_Data_Clean.csv      # Cleaned dataset
└── README.md                 # Project documentation
```

---

## How to Run

```bash
# Clone the repository
git clone https://github.com/Hamza2058/Exploratory-Data-Analytics.git

# Navigate to the project folder
cd Exploratory-Data-Analytics/Books-Market-Analysis

# Install dependencies
pip install pandas matplotlib seaborn numpy

# Open the notebook
jupyter notebook EDA_Books_dataset.ipynb
```

Or open directly in Google Colab using the badge at the top of the notebook.

---

## Limitations & Next Steps

This analysis is based on a static snapshot of ~1,000 titles and does not account for seasonal demand, promotional pricing, or real-time inventory data. Next steps would include integrating time-series sales data to identify seasonal trends, and building a simple pricing model to predict optimal price points per genre.

---

*Analysis by Hamza Awan — Data Analyst | Python · SQL · Power BI*
*📍 Karachi, Pakistan*
