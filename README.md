# CaseStudy_3_ShivamKumar_234

# Sentiment Analysis on Amazon Product Reviews

## Case Study 3 – Machine Learning

### 1. Project Overview
This project focuses on sentiment analysis of Amazon product reviews using Natural Language Processing (NLP) and Deep Learning.

The objective is to classify customer reviews into three sentiment categories:
- **Positive**
- **Neutral**
- **Negative**

Two models will be explored and compared:
1. **BERT (DistilBERT):** A pre-trained transformer model fine-tuned for sentiment classification.
2. **LSTM:** A deep learning baseline for text classification.

### 2. Objectives
- Perform text preprocessing on product reviews.
- Fine-tune a pre-trained transformer model using Hugging Face.
- Build an LSTM baseline model.
- Compare both models using standard evaluation metrics.
- Understand transfer learning efficiency and real-world deployment constraints.

### 3. Technologies Used
- Python
- Google Colab
- PyTorch
- Hugging Face Transformers
- Hugging Face Datasets
- Pandas and NumPy
- Scikit-learn
- Matplotlib

### 4. Dataset
The project uses Amazon product reviews.

The initial prototype uses the Amazon Polarity dataset, which contains positive and negative sentiment labels.

**Dataset limitation:** Amazon Polarity supports binary classification only. The final three-class experiment requires a dataset containing neutral sentiment labels or a documented rating-based labeling strategy.

For rating-based labeling:
- 1–2 stars: Negative
- 3 stars: Neutral
- 4–5 stars: Positive

These labels are derived from ratings and may not always reflect the actual sentiment expressed in the review.

### 5. Methodology
1. Load and inspect the dataset.
2. Clean and preprocess review text.
3. Prepare training, validation, and test datasets.
4. Tokenize text for model training.
5. Fine-tune DistilBERT for sentiment classification.
6. Train an LSTM baseline using the same data splits.
7. Evaluate and compare both models.
8. Discuss deployment considerations.

### 6. Model Evaluation
The models will be evaluated using:

- Accuracy
- Precision
- Recall
- Macro F1-score
- Confusion Matrix
- Training Time
- Inference Latency
- Model Size

Results will be added after completing the experiments.

| Metric | DistilBERT | LSTM |
|---|---|---|
| Accuracy | Pending | Pending |
| Macro F1-score | Pending | Pending |
| Training Time | Pending | Pending |
| Inference Latency | Pending | Pending |
| Model Size | Pending | Pending |

### 7. Transfer Learning Efficiency
DistilBERT uses knowledge learned during pre-training, which can reduce task-specific training requirements compared with training a transformer from scratch.

The project will examine:
- Training time and computational requirements.
- Performance with limited training data.
- Model size and inference efficiency.

### 8. Real-World Deployment Constraints
Potential challenges include:
- GPU and computational costs.
- Prediction latency and throughput.
- Memory requirements.
- Privacy of customer reviews.
- Sarcasm, ambiguous sentiment, and multilingual text.
- Class imbalance and domain shifts.
- Model monitoring and periodic retraining.

### 9. Project Status
**Status:** In Progress

The initial dataset exploration and model setup have been started. Final three-class training, LSTM comparison, and evaluation are pending.

### 10. Repository Structure
```text
Case-Study-3-Sentiment-Analysis/
├── sentiment_analysis.ipynb
├── results/
│   └── comparison.csv
├── README.md
└── requirements.txt
```

### 11. Conclusion
This project aims to compare transformer-based transfer learning with an LSTM baseline for sentiment analysis of Amazon product reviews. The final findings will be based on experimental results and measured computational performance.

### 12. Author
**Student Project – Machine Learning Case Study**
