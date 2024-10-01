# Sentiment Analysis on Movie Reviews

## Introduction

This project develops a sentiment analysis pipeline to classify movie reviews from the IMDb dataset as positive or negative. Utilizing advanced deep learning models like BERT, the aim is to accurately gauge the sentiment expressed in user reviews.

## Data Analysis & Feature Engineering

- **Data Cleaning**: Removed HTML tags, non-alphabetic characters, and converted text to lowercase.
- **Tokenization**: Used BERT's tokenizer to convert text into token sequences.
- **Padding/Truncating**: Standardized review lengths to 500 tokens.
- **Data Splitting**: Divided the dataset into training, validation, and test sets to ensure robust model evaluation.

## Modeling & Prediction

- **Model Architecture**: Fine-tuned `BertForSequenceClassification` for binary sentiment classification.
- **Training Strategy**:
  - **Optimizer**: AdamW with a learning rate of 2e-5.
  - **Loss Function**: Binary Cross-Entropy with Logits Loss.
  - **Scheduler**: Linear learning rate scheduler with warmup.
  - **Gradient Clipping**: Applied to prevent exploding gradients.
- **Evaluation Metrics**: Monitored accuracy, precision, recall, and F1-score during training and validation.

## Results

- **Test Accuracy**: 93.35%
- **Precision**: 0.95
- **Recall**: 0.92
- **F1-Score**: 0.93
- **Confusion Matrix**: Demonstrated effective classification with minimal misclassifications.

## Conclusion

The project successfully built a deep learning-based sentiment analysis system capable of accurately classifying IMDb movie reviews. By leveraging BERT and implementing effective data preprocessing and training strategies, the model achieved high performance metrics. This pipeline serves as a strong foundation for further enhancements and real-world NLP applications.

---
