# Text Summarization Project

## Overview

This project compares Seq2Seq with LSTM and Transformer models for text summarization, focusing on their performance across large and small datasets.

## Features

- **Abstractive Summarization:** Comparison of Seq2Seq LSTM and Transformer models.
- **Dataset Utilization:** Evaluation with large (CNN/Daily Mail) and small (news articles) datasets.
- **Handling Long-Range Dependencies:** Assessing each model's effectiveness in summarizing articles.

## Tools

- **Seq2Seq with LSTM:** Encoder-decoder architecture for capturing long-range dependencies.
- **Transformer:** Utilizes self-attention and positional encoding for improved performance.
- **SPACY:** For text preprocessing and tokenization.
- **Keras/TensorFlow:** For building and training models.

## Dataset

1. **Large Dataset:** Alpaca CNN/Daily Mail (286,817 training pairs).
2. **Small Dataset:** News articles from Hindu, Indian Times, and Guardian (4,515 samples).

## Model Details

### Seq2Seq with LSTM

- **Architecture:** Encoder with 1 embedding layer and 3 LSTM layers; decoder with 1 embedding layer and LSTM.
- **Performance:** Effective on smaller datasets; challenges with larger datasets due to memory limitations.

### Transformer

- **Architecture:** Includes positional encoding, multi-head attention, and encoder-decoder layers.
- **Performance:** Benchmarked on smaller dataset, showing strong handling of long-range dependencies.

## Data Processing

- **Pre-processing:** Cleaned text, tokenized using SPACY, and padded sequences. Split into training (90%) and validation (10%) sets.

## Conclusion

The Transformer model outperforms Seq2Seq LSTM, particularly in handling long-range dependencies and scalability.

