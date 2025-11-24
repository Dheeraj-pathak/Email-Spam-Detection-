📘 SMS Spam Classification using LSTM – README
📌 Project Overview

This project builds an SMS Spam Classifier using Deep Learning (LSTM).
The model reads short text messages and predicts whether they are:

Ham (0) → Normal message

Spam (1) → Unwanted promotional or fraudulent message

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
