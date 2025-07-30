# LLaMA3_1-Financial-Sentiment-Analysis

## 📌 Project Overview

This project fine-tunes **LLaMA 3.1 8B**, a large language model, for **financial sentiment analysis** using multiple financial-specific datasets. It also integrates a **Retrieval-Augmented Generation (RAG)** component to improve accuracy and contextual understanding of real-world financial news.

---

## 📂 Directory Structure


---

## 🧠 Model Details

- **Base Model**: Meta's [LLaMA 3.1 8B]
- **Finetuning Method**: Supervised Fine-Tuning (SFT) + LoRA
- **Language**: English (Financial domain)
- **Purpose**: Classify financial news into sentiment categories such as:
  - Strong Negative
  - Moderately Negative
  - Mildly Negative
  - Neutral
  - Mildly Positive
  - Moderately Positive
  - Strong Positive

---

## 📊 Datasets Used

| Dataset        | Description                                        |
|----------------|----------------------------------------------------|
| FPB            | Financial Phrase Bank - sentiment-labeled phrases |
| FiQA           | Financial QA dataset with sentiment annotations   |
| TFNS           | Financial News Sentiment (2024 edition)           |
| NWGI           | News headline sentiment based on global index     |
| Bloomberg 2024 | Scraped & cleaned news headlines (custom)         |

All datasets were cleaned, deduplicated, and mapped into 7 sentiment classes.

---


## 🔍 RAG System

A **Retrieval-Augmented Generation (RAG)** component

## 📉 Evaluation Results

| Model Version        | Accuracy | Macro-F1 |
|----------------------|----------|----------|
| Baseline (LLaMA 3.1) | 58.2%    | 0.61     |
| Finetuned            | 87%    | 0.77     |

Evaluation conducted on the validation sets.




