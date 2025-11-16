# Project Overview

This project evaluates different approaches to sentiment classificaiton on movie review datasets ([IMDB](https://huggingface.co/datasets/stanfordnlp/imdb) and [Rotten Tomatoes](https://huggingface.co/datasets/cornell-movie-review-data/rotten_tomatoes)):
1. **Baseline Lexical CLassifier**: Logistic regression with TF-IDF
2. **Prompting with [Flan-T5-small](https://huggingface.co/google/flan-t5-small)**: Zero-shot and few-shot prompting experiments
3. **Supervised Fine-tuning [DistilBERT](https://huggingface.co/distilbert/distilbert-base-uncased)**: fine-tuned on labeled training data

The notebooks contains all code to reproduce the experiments, generate figures, and compute evaluation metrics (accuracy, macro-F1, and Brier score).

```## 📁 Repository Structure
dsa4213project/
│
├─ notebooks/               # Jupyter notebooks with experiment code
│  ├─ 1.0-baseline-report.ipynb
│  ├─ 2.0-prompting-report.ipynb
│  └─ 3.0-fine-tuning-report.ipynb
│
├─ results/                 # Outputs from experiments
│  ├─ figures/              # Generated figures (plots, reliability curves)
│  └─ tables/               # Result tables (accuracy, macro-F1, Brier score)
│
├─ requirements.txt         # Python dependencies
```
## Prerequisites
Download the packages listed in requirements.txt using:
```
pip install -r requirements.txt
```

## Usage
1. Open the relevant notebook in the `notebooks/` folder.
2. Run each notebook to reproduce results. Figures and tables will be automatically saved to the `results/` folder.

