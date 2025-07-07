# Financial Data Sentiment Analysis

Perform sentiment analysis on financial text using BERT-based models and advanced prompting techniques.

---

## Table of Contents

1. [Overview](#overview)
2. [Repository Structure](#repository-structure)
3. [Installation](#installation)
4. [Data Preparation](#data-preparation)
5. [Models & Prompting Techniques](#models--prompting-techniques)
6. [Running Experiments](#running-experiments)
7. [Results Summary](#results-summary)
8. [Contributing](#contributing)
9. [License](#license)
10. [References](#references)

---

## Overview

This project fine-tunes BERT-based models (FinBERT, FinBERT-Tone, Financial-BERT, RoBERTa-Financial) on the FinancialPhraseBank dataset to evaluate performance under various prompting strategies:

- **Zero-shot**
- **Few-shot**
- **Chain-of-Thought**
- **Instruction-based**
- **Contrastive**

---

## Installation

1. **Clone the repo**

   ```bash
   git clone https://github.com/<username>/financial-sentiment-bert.git
   cd financial-sentiment-bert
   ```

2. **Set up a virtual environment**

   ```bash
   python3 -m venv venv
   source venv/bin/activate
   pip install -r requirements.txt
   ```

---

## Data Preparation

Download `Sentences_AllAgree.txt` from the [FinancialPhraseBank dataset](https://huggingface.co/datasets/takala/financial_phrasebank).



## Models & Prompting Techniques

**Models:**

- FinBERT
- FinBERT-Tone
- Financial-BERT
- RoBERTa-Financial

**Prompting Strategies:**

1. Zero-shot: direct classification instruction
2. Few-shot: include example prompts
3. Chain-of-Thought: step-by-step reasoning
4. Instruction-based: clear directive
5. Contrastive: sentence comparison

---

## Results Summary

| Model                 | Zero-shot | Few-shot | Chain-of-Thought | Instruction | Contrastive |
| --------------------- | --------- | -------- | ---------------- | ----------- | ----------- |
| **FinBERT**           | 0.7219    | 0.3797   | 0.6269           | 0.7351      | 0.3642      |
| **FinBERT-Tone**      | 0.5033    | 0.2737   | 0.6358           | 0.7616      | 0.3157      |
| **Financial-BERT**    | 0.1192    | 0.1236   | 0.1236           | 0.5055      | 0.1236      |
| **RoBERTa-Financial** | 0.9139    | 0.2671   | 0.8962           | 0.9050      | 0.3245      |

---

## Contributing

Contributions are welcome! Please:

1. Fork the repo
2. Create a feature branch (`git checkout -b feature/...`)
3. Commit your changes (`git commit -m 'Add ...'`)
4. Push to your branch (`git push origin feature/...`)
5. Open a Pull Request

---

## License

This project is licensed under the MIT License. See [`LICENSE`](LICENSE) for details.

---

## References

- [FinBERT](https://github.com/ProsusAI/finBERT)
- [FinBERT-Tone](https://huggingface.co/yiyanghkust/finbert-tone)
- [FinancialPhraseBank](https://huggingface.co/datasets/takala/financial_phrasebank)
- [RoBERTa-Financial](https://github.com/yya518/FinBERT)

