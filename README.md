# Sentiment Analysis with Parameter-Efficient Fine-Tuning

This project demonstrates parameter-efficient fine-tuning (PEFT) using the LoRA (Low-Rank Adaptation) technique to improve sentiment classification. The goal is to enhance a pre-trained model's performance on sentiment classification by fine-tuning it with LoRA, making it both efficient and adaptable without retraining the entire model.

## Project Overview

1. **Objective**: Evaluate a pre-trained model for sentiment classification, apply parameter-efficient fine-tuning with LoRA, and observe improvements in model performance.
2. **PEFT Technique**: LoRA is applied to enable efficient and focused fine-tuning of specific model layers, reducing the need to modify the entire model. This technique is beneficial for limited computational resources and allows more targeted adaptation.
3. **Model**: The pre-trained `cardiffnlp/twitter-roberta-base-sentiment-latest` model is used, which is well-suited for text classification.
4. **Dataset**: Sentiment analysis dataset from Hugging Face's `FinanceInc/auditor_sentiment`.

## Installation

To run this project, please install the necessary dependencies from `requirements.txt`:

```bash
pip install -r requirements.txt
```

## Project Description
The project loads a pre-trained model, evaluates its baseline performance on a sentiment classification task, and then fine-tunes it using LoRA. After training with LoRA, the model achieved a 20% performance improvement over the base model, demonstrating the effectiveness of parameter-efficient fine-tuning. This approach shows the potential for faster, resource-efficient training with enhanced results, making it suitable for environments with computational constraints.