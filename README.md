# Consumer Insights from Online Reviews

## Overview

This project analyzes consumer reviews to identify patterns in customer sentiment, product experience, dissatisfaction, and review helpfulness.

The analysis uses Python-based text and sentiment analysis on a dataset of consumer reviews of Amazon products.

## Research Questions

- How does review sentiment relate to star ratings?
- What product experience themes appear in positive and negative reviews?
- What review characteristics are associated with helpfulness?
- How do dissatisfaction-related themes vary across ratings?

## Dataset

**Source:** Datafiniti Consumer Reviews of Amazon Products

**Final dataset:** 34,626 reviews

The dataset contains review text, star ratings, product information, recommendation information, helpful votes, and other review metadata.

## How to Run

### 1. Download the Dataset

Download the **Datafiniti Consumer Reviews of Amazon Products** dataset from Kaggle.

Use the file:

`1429_1.csv`

### 2. Open the Notebook

Open `Consumer_Review_Analysis.ipynb` in Google Colab or Jupyter Notebook.

### 3. Upload the Dataset

Upload `1429_1.csv` to the notebook environment.

### 4. Run the Notebook

Run the notebook cells from top to bottom.

The notebook performs data cleaning, sentiment analysis, keyword-based theme analysis, and review helpfulness analysis.

> **Note:** The analysis uses the same `1429_1.csv` dataset and skips malformed CSV rows during loading using `on_bad_lines="skip"`.

## Methodology

1. Data loading and cleaning
2. Missing-value handling
3. Review text preprocessing
4. Sentiment analysis using TextBlob
5. Rating-sentiment analysis
6. Keyword-based theme analysis
7. Comparison of themes across star ratings
8. Review helpfulness analysis
9. Correlation analysis

## Key Findings

- Higher star ratings were generally associated with more positive review language.
- Rating and sentiment polarity had a correlation of **0.236**.
- Dissatisfaction/return-related language appeared in **27.56% of 1-star reviews** compared with **1.09% of 5-star reviews**.
- Performance-related terms such as slow, broken, freeze, and lag were more prevalent in lower-rated reviews.
- Difficulty-related language was also more prevalent in lower-rated reviews.
- Reviews receiving helpful votes were longer on average: **48.75 words vs 28.29 words**.
- Review length had a correlation of **0.177** with receiving at least one helpful vote.
- Helpful reviews were slightly less positive in sentiment on average, suggesting that helpfulness was not simply associated with positive sentiment.

## Tools & Technologies

- Python
- Pandas
- NumPy
- Matplotlib
- NLTK
- TextBlob
- Google Colab
- GitHub

## Limitations

- TextBlob sentiment is an automated signal and may misclassify mixed or context-dependent reviews.
- Keyword-based theme detection does not capture every expression of a theme.
- Themes can overlap within the same review.
- The dataset is heavily concentrated in Amazon-branded products.
- The analysis identifies associations rather than causal relationships.
- Some malformed CSV rows were skipped during loading using `on_bad_lines="skip"`.

## Project Structure

```text
consumer-review-analysis/
│
├── Consumer_Review_Analysis.ipynb
└── README.md

## Author

**Ishant Yadav**

B.S. (Hons.) Computer Science with Research  
Guru Ghasidas Vishwavidyalaya
