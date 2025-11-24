📘 SMS Spam Classification using LSTM – README
📌 Project Overview

This project builds an SMS Spam Classifier using Deep Learning (LSTM).
The model reads short text messages and predicts whether they are:

Ham (0) → Normal message

Spam (1) → Unwanted promotional or fraudulent message
<<<<<<< HEAD
=======

It uses:

Python

TensorFlow/Keras

LSTM (Long Short-Term Memory)

Tokenization + Embedding

Confusion Matrix + Performance Metrics

This project demonstrates a complete workflow of natural language processing, sequence modeling, and deep learning classification.

🧠 Why LSTM?

SMS messages are sequences of words, and meaning depends on order.
Example:

“Free ticket now” → spam

“Are you free now?” → ham

LSTM is perfect because it:

remembers long-term dependencies

captures sequence patterns

handles text context better than simple models

🚀 Features

✔ Complete cleaning of raw SMS text
✔ Tokenization + Padding
✔ LSTM-based sequential model
✔ Bidirectional LSTM for better context
✔ Training, validation, and testing pipeline
✔ Confusion matrix and metrics
✔ Saved model + tokenizer for future use

🗂️ Dataset

The project uses the popular SMS Spam Collection Dataset, which contains:

4825 ham messages

747 spam messages

Format:

label, message
ham, Go until jurong point...
spam, Congratulations you won...


If using Kaggle version:

Column names may appear as v1 (label), v2 (message).
The script automatically renames them.

🧹 Text Preprocessing Pipeline

The script performs the following steps:

Convert to lowercase

Remove URLs

Remove email addresses

Remove numeric values

Remove punctuation

Clean whitespace

Tokenize using regex (no NLTK required)

Remove stopwords

Join tokens back into a clean sentence

This improves signal quality for the LSTM.

🔢 Tokenization + Padding

Keras Tokenizer converts words → integers.

Vocabulary size: 10,000 words

Max sequence length: 100 tokens

OOV token: <OOV> (handles unknown words)

Padding ensures fixed-length inputs for the network.

🧱 Model Architecture

The LSTM model consists of:

Embedding Layer (100 dimensions)
Bidirectional LSTM (128 units)
Dropout (0.4)
Dense (64 units, ReLU)
Dropout (0.3)
Dense (1 unit, Sigmoid)

Loss & Optimizer

Loss: Binary Cross-Entropy

Optimizer: Adam

Metrics: Accuracy

🏋️ Training Setup

Batch size: 64

Epochs: 10

Validation split: 10%

Callbacks:

EarlyStopping

ModelCheckpoint (saves best model automatically)

📊 Evaluation Metrics

After training, the model generates:

Accuracy

Precision

Recall

F1-Score

Confusion Matrix

These help evaluate correctness on both ham and spam messages.
🏁 Results (Typical Performance)

Most runs achieve:

Accuracy: 95%+

Precision (Spam): 90%+

Recall (Spam): 85%+

📝 Future Improvements

Use GRU or Transformer-based models

Add stemming/lemmatization

Add TF-IDF + classical ML models

Deploy using Flask/FastAPI

Create a web UI

👤 Author

Dheeraj
AIML Student & Android Developer
>>>>>>> 7451d44 (Final commit)
