# PROJECT-SENTIMENT-ANALYSIS-OF-YOUTUBE-COMMENTS

![YouTube Logo](https://i.imgur.com/nuSO2Au.png)

Analyze sentiment on YouTube video comments end-to-end: **fetch → clean → classify → visualize**.  
Supports a fast **VADER** baseline and optional **Transformer** models (RoBERTa/BERT via 🤗 Transformers).
Includes a small **Streamlit** dashboard for interactive exploration.

---

## Features
- Pull top-level comments (and optional replies) using **YouTube Data API v3**.
- Robust preprocessing: lowercase, URL/emoji/mention handling, deduping, optional language filter.
- Two sentiment engines:
  - **VADER** (rule-based, fast, social-text friendly).
  - **Transformer** (e.g., `cardiffnlp/twitter-roberta-base-sentiment-latest` or multilingual models).
- Saves predictions (CSV/JSONL) with timestamps, likes, author, label & scores.
- **Streamlit** dashboard: filters, timelines, label distribution, top ± comments, word clouds.
- CLI scripts + notebooks; lightweight tests with `pytest`.

---

## Tech Stack
**Python 3.9+**, YouTube Data API v3, `pandas`, `numpy`, `nltk` / `vaderSentiment`,  
`transformers` + `torch` (optional), `langdetect` (optional), `streamlit`, `plotly`, `wordcloud`.

---
