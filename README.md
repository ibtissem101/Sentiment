# Sentiment Analysis with DeBERTa

This project performs sentiment analysis using the DeBERTa transformer model. All code and experiments are in [`sentimentanalysis.ipynb`](./sentimentanalysis.ipynb).

## Technical Overview

### Data Preprocessing
- **Cleaning:** Input text is lowercased and stripped of special characters.
- **Tokenization:** Text data is tokenized using the HuggingFace DeBERTa tokenizer, ensuring compatibility with the model.

### Model: DeBERTa
- **Architecture:** Utilizes the DeBERTa (Decoding-enhanced BERT with Disentangled Attention) model from HuggingFace Transformers.
- **Fine-tuning:** The model is fine-tuned on a labeled sentiment dataset for multi-class classification (e.g., positive, negative, neutral).
- **Training:** Conducted using PyTorch, with GPU acceleration if available.
- **Evaluation:** Accuracy, precision, recall, and F1-score are calculated on validation/test data.
- **Inference:** The trained model predicts sentiment for new, unseen text.
