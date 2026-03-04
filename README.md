# HuggingFace Sentiment App 🤖

**Real-time sentiment analysis powered by transformer models from HuggingFace.**

---

## Overview

This app performs real-time sentiment analysis on text input using pre-trained transformer models from the HuggingFace model hub. Users can enter any text and instantly receive a sentiment classification (Positive, Negative, or Neutral) along with a confidence score.

Built as a demonstration of NLP/ML model integration in a web interface — bridging the gap between raw ML models and practical, usable applications.

---

## Features

- **Real-time sentiment classification** — Positive, Negative, or Neutral
- **Confidence scoring** — Shows model confidence percentage for each prediction
- **HuggingFace Transformers** — Powered by state-of-the-art NLP models
- **Clean, minimal UI** — Fast and focused user experience
- **Multi-input support** — Analyze single sentences or longer text blocks

---

## Tech Stack

| Layer | Technology |
|---|---|
| **ML Framework** | HuggingFace Transformers |
| **Language** | Python |
| **Model** | DistilBERT / BERT fine-tuned for sentiment |
| **Interface** | Gradio / Streamlit |

---

## Getting Started

### Prerequisites
- Python 3.8+
- pip

### Installation

```bash
git clone https://github.com/ashleyhoward002/huggingface-sentiment-app.git
cd huggingface-sentiment-app
pip install -r requirements.txt
```

### Run the App

```bash
python app.py
```

The app will launch in your browser at `http://localhost:7860` (Gradio) or `http://localhost:8501` (Streamlit).

---

## How It Works

1. User enters text in the input field
2. The app tokenizes the text using a HuggingFace tokenizer
3. The pre-trained transformer model processes the tokens
4. The model outputs a sentiment label and confidence score
5. Results are displayed in real time

---

## Example Output

| Input | Sentiment | Confidence |
|---|---|---|
| "This product is amazing!" | Positive | 98.2% |
| "I'm really disappointed with the service." | Negative | 94.7% |
| "It arrived on Tuesday." | Neutral | 87.1% |

---

## Model Details

Uses a DistilBERT model fine-tuned on the SST-2 sentiment dataset — one of the most widely used benchmarks for sentiment analysis. DistilBERT provides near-BERT accuracy at 60% fewer parameters.

---

## Built By

Ashley Howard — [github.com/ashleyhoward002](https://github.com/ashleyhoward002)
