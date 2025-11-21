# news-popularity-classifier

BSc ML project, part of Minor Data Science and AI @ UvA.
Project in collaboration with <Martyna Zimek>, <Anass Airad>

**Description**

A machine learning project that predicts whether online news articles will be popular (>1400 shares) based on article features like content length, sentiment, keywords, and publication timing.

## Project Overview

This project analyzes the Online News Popularity dataset from Mashable to build classification models that predict article popularity. Three different algorithms are compared: Logistic Regression, K-Nearest Neighbors, and Decision Trees.

## Dataset

- **Source**: Online News Popularity dataset (39,644 articles)
- **Features**: 60 attributes including:
  - Article metadata (publication day, content length, keywords)
  - Sentiment analysis (polarity, subjectivity)
  - Topic channels (lifestyle, entertainment, business, tech, world)
  - Reference statistics
 
## Models & Results

| Model | Accuracy | F1 Score | Best Hyperparameters |
|-------|----------|----------|---------------------|
| Logistic Regression | 0.65 | 0.65 | C=1 |
| K-Nearest Neighbors | 0.63 | 0.63 | n_neighbors=11 |
| Decision Tree | 0.64 | 0.64 | max_depth=5, criterion=gini |

## Key Findings

**Most Important Features:**
- Average keyword shares (`kw_avg_avg`)
- Article sentiment and subjectivity
- Publication timing (weekday vs weekend)
- Data channel (tech, entertainment, etc.)

## Requirements
```
numpy
pandas
matplotlib
scikit-learn
```

## Project Structure
```
├── data/
│   └── online_news_popularity.csv
├── main_project.ipynb
├── README.md
├── requirements.txt
└── results/
    └── feature_importance_plots/
```
