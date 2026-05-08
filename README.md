# BERT Question Answering System

This project implements an extractive Question Answering (QA) system using BERT and the Stanford Question Answering Dataset (SQuAD).

## Models Used
- DistilBERT
- BERT Base Uncased

## Dataset
- Stanford Question Answering Dataset (SQuAD)

## Final Results

| Model | Exact Match (EM) | F1 Score |
|---|---|---|
| DistilBERT (20k) | 68.15 | 76.42 |
| BERT Base (20k) | 73.25 | 81.61 |
| BERT Base (40k) | 76.20 | 84.39 |

## Features
- Fine-tuned transformer QA model
- Interactive question answering UI
- Multiple question support
- Robustness testing with noisy text
- EM/F1 evaluation metrics

## Technologies
- Python
- PyTorch
- HuggingFace Transformers
- Google Colab

## How to Run

Install dependencies:

```bash
pip install -r requirements.txt
```

Open the notebook and run all cells.

## Author
Rabii El Dawi

## Reproducing the Results

### 1. Install Dependencies

```bash
pip install -r requirements.txt
```

### 2. Open the Notebook

Open:

```text
notebook/BERT_SQuAD_Question_Answering.ipynb
```

using Google Colab or Jupyter Notebook.

### 3. Enable GPU (Recommended)

In Google Colab:

Runtime → Change runtime type → GPU

### 4. Run the Notebook

Run all cells sequentially from top to bottom.

### 5. Training

The notebook includes experiments using:
- DistilBERT
- BERT Base Uncased

The final experiment trains BERT Base on:
- 40,000 training samples
- 3,000 validation samples

### 6. Evaluation

The model is evaluated using:
- Exact Match (EM)
- F1-score

### 7. Interactive Demo

The notebook includes an interactive QA interface where users can:
- input custom paragraphs,
- ask multiple questions,
- receive extracted answers with confidence scores.