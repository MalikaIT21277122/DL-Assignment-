# IMDB Movie Review Sentiment Analysis Using Deep Learning

## Project Overview

This project focuses on performing **sentiment analysis** on movie reviews from the **IMDB dataset** using deep learning models. The goal is to classify each review as either **positive** or **negative**, based on the sentiment expressed in the text. We implemented four different models, each designed to capture patterns and context within the reviews to make accurate predictions.

## Models Implemented
Each team member was responsible for implementing and evaluating a specific deep learning model:
- **Withanagamage J.C (IT21250156)** – **Convolutional Neural Network (CNN)**: Used to capture local features and patterns within the text.
- **Degaldoruwa D.W.S.S.W.M.R.M.B.B (IT21277122)** – **Long Short-Term Memory (LSTM)**: Applied to capture long-term dependencies within the review sequences.
- **Weerakoon W.M.B.B (IT21303302)** – **Recurrent Neural Network (RNN)**: Used to process the text sequentially but with limited capacity for long-term dependencies.
- **Wijerama H.J.K.S.R (IT21343520)** – **Bidirectional LSTM (BiLSTM)**: Implemented to process the text in both forward and backward directions to capture both past and future context.

## Dataset
The dataset used for this project is the **IMDB Movie Review Dataset**, containing **50,000 reviews** split evenly into **25,000 positive** and **25,000 negative** samples. The reviews are free-form text, and the dataset is balanced, making it ideal for binary classification tasks.

## Preprocessing
We performed the following preprocessing steps:
1. **Text Cleaning**: Removed HTML tags and irrelevant characters.
2. **Tokenization**: Converted the text reviews into sequences of integers using Keras's Tokenizer.
3. **Padding**: Ensured all sequences had a uniform length of 200 tokens.
4. **Word Embedding**: Converted the sequences into dense word vectors using an embedding layer.

## Performance Comparison
Each model was trained and evaluated on the IMDB dataset. Below is a summary of the model performances:

| **Model**   | **Accuracy** |
|-------------|--------------|
| **CNN**     | 85.6%        |
| **LSTM**    | 87.4%        |
| **RNN**     | 82.5%        |
| **BiLSTM**  | 89.1%        |

## Conclusion
The **Bidirectional LSTM (BiLSTM)** achieved the highest accuracy, demonstrating the effectiveness of processing text in both forward and backward directions. The **LSTM** also performed well, but the **RNN** showed limitations in capturing long-term dependencies. The **CNN** effectively captured local patterns but was less effective for long sequences. 

Each model contributed to a deeper understanding of the task, and the comparison shows the strengths and weaknesses of different deep learning architectures in sentiment analysis.