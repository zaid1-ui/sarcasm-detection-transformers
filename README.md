# Sarcasm Detection in Tweets using Transformer Models

A comparative study of BERT, RoBERTa, and BERTweet transformer models fine-tuned for binary sarcasm classification on the SemEval-2018 Task 3 Twitter dataset.

## Overview

This project evaluates three pre-trained transformer models under two training conditions:
- **Full fine-tuning** — all layers updated
- **Frozen encoder** — only the classification head trained

TF-IDF with Logistic Regression and LinearSVC are used as baselines.

## Results

| Model | F1 Score | Accuracy |
|-------|----------|----------|
| BERTweet (full fine-tune) | 0.780 | 0.840 |
| RoBERTa-base | 0.750 | — |
| BERT-base | 0.720 | — |

> BERTweet achieves the best performance, confirming that domain-adaptive pre-training on tweet corpora provides measurable advantages.

## Dataset

SemEval-2018 Task 3 — binary irony detection in English tweets (3,834 tweets, 35% sarcastic).

## Models Used

- `bert-base-uncased`
- `roberta-base`
- `vinai/bertweet-base`

## Repository Structure

```
├── Sarcasm_Detection_Transformers.ipynb  # Main notebook
├── Sarcasm-Detection-Transformers-Report.docx  # Full report
└── figures/  # Plots and result visualizations
```

## Course

CS4063 — Natural Language Processing, FAST-NUCES Lahore
