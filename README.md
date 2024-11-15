# News_SummarizerT5Transformer

A deep learning model based on the T5 Transformer for generating concise and relevant summaries of news articles. This project uses transfer learning with the Hugging Face Transformers library, leveraging the T5 model fine-tuned on a news dataset to achieve high-quality text summarization.

## Project Overview
News_SummarizerT5Transformer is a text summarization tool designed to distill the essential information from lengthy news articles into concise summaries. This project employs the T5 Transformer model, a popular sequence-to-sequence architecture, to generate summaries that retain the key points and overall context of the original articles.

Used a Pre-trained T5-base transformer, and fine-tuned using CNN/Daily-News dataset

## Features
- Summarizes long news articles into concise, readable summaries.
- Fine-tuned on a news-specific dataset for better contextual understanding.
- Evaluates model performance using ROUGE metrics.
- Adjustable parameters for text summarization length and detail.

![Screenshot 2024-11-15 135646](https://github.com/user-attachments/assets/0ab21306-bc2e-4eba-96d8-4202c73f9c14)


```bash
git clone https://github.com/yourusername/News_SummarizerT5Transformer.git
cd News_SummarizerT5Transformer
