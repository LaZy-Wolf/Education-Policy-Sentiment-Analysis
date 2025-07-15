NEP 2020 Sentiment Analysis
This project analyzes sentiment toward the National Education Policy (NEP) 2020 using 18,240 English tweets. It employs VADER, RoBERTa (cardiffnlp/twitter-roberta-base-sentiment-latest), and an ensemble model, with advanced preprocessing and visualizations.
Overview

Goal: Gauge public sentiment on NEP 2020 via Twitter data.
Pipeline:
Preprocessing: Lemmatization, emoji handling, custom stopwords (e.g., nep, policy).
Sentiment Analysis: VADER (lexicon-based), RoBERTa (contextual), ensemble (70% RoBERTa, 30% VADER).
Visualizations: Sentiment distribution, score histograms, trends, model comparison, word clouds.



Improvements

Performance: Batch processing (~500 tweets/min), GPU support, efficient tokenization.
Accuracy: Ensemble model (5–10% better than single models), emoji handling, domain-specific stopwords.
Robustness: Error handling, logging, data quality checks.
Visualizations: Professional dashboard with Seaborn styling, high-resolution word clouds.

Contents

Code: sentiment_analysis_nep2020.py
Data: enhanced_sentiment_results.csv (sentiments/scores)
Visualizations: comprehensive_sentiment_analysis.png, positive/negative/neutral_wordcloud_enhanced.png
Chart: sentiment_chart.html (Chart.js)
Report: sentiment_analysis_report.pdf
Notebook: NEP2020_Sentiment_Analysis.ipynb (optional)

Setup

Use Google Colab or local Python.
Install: pip install vaderSentiment transformers torch nltk pandas matplotlib seaborn wordcloud tqdm
Upload NEP_2020_english_tweet.csv from Kaggle.
Run sentiment_analysis_nep2020.py.

Outputs

CSV: enhanced_sentiment_results.csv (Tweet, sentiments, scores).
Visualizations: Dashboard (distribution, trends, comparison), word clouds.
Summary: [e.g., ~60% positive, 25% neutral, 15% negative; insert after running].
Chart: sentiment_chart.html (VADER sentiments).

Submission
Submitted via GitHub link on WhatsApp by July 22, 2025, per requirements.
Notes

Limitations: Urban bias in Twitter data, memory-intensive RoBERTa.
Future Work: Non-English tweets, fine-tuned models.
