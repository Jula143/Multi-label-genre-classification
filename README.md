# Multi-Label Book Genre Classification
## Project Overview

This project aims to develop an automated classification system that assigns one or more genre labels to book descriptions. For dataset I used a subset of the Goodreads book genres dataset from Hugging Face: https://huggingface.co/datasets/pszemraj/goodreads-bookgenres

In dataset each record contains:
- Book Title
- Short Description 
- Binary-encoded list of genres present in the book

## Selected Models

I experimented with two models for multi-label classification:
1. Support Vector Classifier (SVC) with Binary Relevance
SVC is a machine learning algorithm based on Support Vector Machines (SVM), typically used for binary classification. In this project, SVC is combined with Binary Relevance (BR), which decomposes the problem into multiple independent binary classifiers for each genre label.

3. DeBERTa (Microsoft DeBERTa v3)
The model utilizes an appropriate tokenizer and is designed for contextual and semantic understanding, improving multi-label prediction accuracy.

## Evaluation Metrics

Metrics that evaluate models' performance:
- Hamming Accuracy
- Precision (Micro & Macro)
- Recall (Micro & Macro)
- F1-Score (Micro & Macro)

Using both Micro and Macro versions provides insights at both dataset-wide and per-label levels.
