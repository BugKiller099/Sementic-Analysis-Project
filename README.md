# **Sentiment Analysis Using RoBERTa** 🤖📊
[![License](https://img.shields.io/github/license/BugKiller099/Sementic-Analysis-Project)](https://github.com/BugKiller099/Sementic-Analysis-Project/blob/main/LICENSE)
![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![Transformers](https://img.shields.io/badge/Transformers-4.0%2B-yellow)
![Model Accuracy](https://img.shields.io/badge/Accuracy-93.6%25-green)

---

## **📖 Overview**
This project demonstrates a **sentiment analysis pipeline** using the powerful **RoBERTa model**, a state-of-the-art transformer-based architecture. The pipeline classifies text into the following sentiment categories:
- **Positive**
- **Neutral**
- **Negative**

The model has been fine-tuned on real-world datasets and is optimized for robust performance, handling complex, context-dependent, and ambiguous text inputs effectively.

---

## **🚀 Features**
- Fine-tuned **RoBERTa-base** model for sentiment classification.
- Custom **`SentimentPipeline`** for seamless predictions on custom datasets.
- Tested across diverse real-world examples, ensuring strong **generalization**.
- Capable of identifying nuanced sentiment variations in both concise and elaborate text formats.

---

## **📂 Project Structure**
```plaintext
📦 Sentiment-Analysis
├── data/                       # Optional: Training/validation datasets
├── model/                      # Pre-trained model weights
├── src/                        # Source code files
│   ├── dataset.py              # Custom dataset class for PyTorch
│   ├── model.py                # Model architecture and setup
│   ├── pipeline.py             # Sentiment pipeline implementation
│   └── train.py                # Training and evaluation script
├── README.md                   # Documentation (this file)
└── requirements.txt            # Python dependencies
```


# Sentiment Classification Model

##  📊 Dataset 

The training dataset combines two distinct social media sources:

1. **Twitter Dataset**: Captures concise, real-time sentiment-driven tweets.
2. **Reddit Dataset**: Reflects elaborate, discussion-driven sentiment patterns.

This dual-source strategy enhances the model's ability to generalize across varied content types and language styles.

---

## 📈 Performance

The sentiment classification model achieved an impressive **93.2% accuracy**, with detailed performance metrics for each sentiment category:

| Sentiment      | Precision | Recall | F1-Score | Support |
|----------------|-----------|--------|----------|---------|
| Negative (-1)  | 0.87      | 0.88   | 0.88     | 8,250   |
| Neutral (0)    | 0.95      | 0.97   | 0.96     | 12,778  |
| Positive (1)   | 0.95      | 0.93   | 0.94     | 15,771  |

### Weighted Averages:
- **Precision**: 0.93
- **Recall**: 0.93
- **F1-Score**: 0.93

### Macro Averages:
- **Precision**: 0.92
- **Recall**: 0.93
- **F1-Score**: 0.93

The model demonstrates high precision and recall across all sentiment categories, ensuring consistent cross-platform performance.

---

## 💻 Usage

### Prerequisites  

Ensure you have the following installed:

1. **Python**: Version 3.8 or higher.
2. **Dependencies**: Use the provided `requirements.txt` file to set up the environment:

   ```bash
   pip install -r requirements.txt


## Conclusion

In this notebook, we successfully fine-tuned **RoBERTa**, a robustly optimized version of BERT, for sentiment analysis on social media data. By utilizing a combination of **Twitter** and **Reddit** datasets, we ensured the model's adaptability to diverse language styles and contexts. The Twitter dataset, with its concise nature, helped the model capture clear sentiments, while the more elaborated Reddit comments tested the model's ability to handle longer, more nuanced text.

The fine-tuned model achieved a **93.6% accuracy** in sentiment classification, showcasing its strong performance across different social media platforms. The detailed classification report further highlighted the model's ability to precisely predict sentiment across various categories, with balanced performance in terms of **precision**, **recall**, and **F1-score**.

With this approach, we demonstrated the power of **RoBERTa** in tackling sentiment analysis tasks, making it a valuable tool for analyzing social media data, where sentiments can vary widely depending on the platform and context.

Future work could focus on extending this model to handle even larger datasets, incorporate more social media platforms, and explore the effect of fine-tuning hyperparameters for further performance improvements.

