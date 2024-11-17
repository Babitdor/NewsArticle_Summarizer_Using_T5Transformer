# News Summarizer Using T5 - Transformer

A deep learning model based on the T5 Transformer for generating concise and relevant summaries of news articles. This project uses transfer learning with the Hugging Face Transformers library, leveraging the T5 model fine-tuned on a news dataset to achieve high-quality text summarization.

## Project Overview
News_SummarizerT5Transformer is a text summarization tool designed to distill the essential information from lengthy news articles into concise summaries. This project employs the T5 Transformer model, a popular sequence-to-sequence architecture, to generate summaries that retain the key points and overall context of the original articles.

## Training
The model is trained for abstractive summarization by fine-tuning T5 on the CNN/Daily Mail dataset. The fine-tuning is performed using the following settings:

Loss function: Cross-entropy loss
Optimizer: Adam optimizer with learning rate decay
Evaluation metrics: ROUGE-1, ROUGE-2, ROUGE-L

## Features
- Summarizes long news articles into concise, readable summaries.
- Fine-tuned on a news-specific dataset for better contextual understanding.
- Evaluates model performance using ROUGE metrics.
- Adjustable parameters like max_length and beam search size for text summarization length and detail.

![Screenshot 2024-11-15 135646](https://github.com/user-attachments/assets/0ab21306-bc2e-4eba-96d8-4202c73f9c14)

## Model

The **T5 (Text-to-Text Transfer Transformer)** model, pretrained on a large corpus of text data, is used for generating summaries. It uses the same architecture for all text tasks, such as translation, summarization, and question answering, by framing all tasks as text-to-text transformations.

### Architecture:
1. **T5 Transformer**: Pretrained on large-scale data for general text generation tasks.
2. **Fine-tuning**: The model is fine-tuned on the CNN/Daily Mail dataset for abstractive summarization.
3. **Input/Output Format**: The input is the full article, and the output is the summary.


## Fine-tuning Procedure:
Preprocessing of CNN/Daily Mail articles and summaries.
Tokenization using the T5 tokenizer.
Training using the fine-tuning dataset and validation split.
Evaluation using the ROUGE score metrics to evaluate the summary generation quality.



## NOTE: 
The model can still perform much better with more data, the model in it's current state has been fine-tunning with a subset size of 4000, due to <b>hardware limitations</b>

1. Clone the repository:

   ```bash
   git clone https://github.com/yourusername/News-Article-Summarization.git
   cd News-Article-Summarization

2. Create a Virtual Environment: 
   python -m venv .env
   then Run: .env/Scripts/Activate


3. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
