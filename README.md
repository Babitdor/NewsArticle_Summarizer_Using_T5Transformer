# News Summarizer Using T5 - Transformer

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

## Results:

The current state the model has some decent performance as per the score below, 

Step	Training Loss	  Validation Loss	    Rouge1	  Rouge2	  Rougel	  Gen Len
200	  No log	        0.214724	          0.625500	0.364300	0.586500	73.466000
400	  No log	        0.217768	          0.620300	0.360400	0.580300	73.472000
600	  1.053100	      0.213199	          0.625600	0.366000	0.586200	73.468000
800	  1.053100	      0.211047	          0.629800	0.369000	0.590200	73.473000
1000	0.249100	      0.209719	          0.631300	0.372700	0.592800	73.473000

## NOTE: 
The model can still perform much better with more data, the model in it's current state has been fine-tunning with a subset size of 4000, due to <b>hardware limitations</b>

```bash
git clone https://github.com/yourusername/News_SummarizerT5Transformer.git
cd News_SummarizerT5Transformer
