# Encoder_Decoder_Architecture # 
# Neural Machine Translation (PT → EN) using Seq2Seq LSTM

This project demonstrates a simple Sequence-to-Sequence (Seq2Seq) model using LSTM to translate sentences from Portuguese to English. The dataset used is the TED Talks Portuguese-to-English dataset from TensorFlow Datasets (TFDS).

# 1. Project Summary

Loads the TED HRLR PT→EN translation dataset.

Preprocesses and tokenizes text sequences.

Builds an Encoder–Decoder LSTM model.

Trains the model on a small subset of 1,000 samples.

Shows basic neural machine translation workflow.

This project is mainly for learning and demonstration.

# 2. Technologies Used

Python

TensorFlow / Keras

TensorFlow Datasets

NumPy, Pandas

# 3. Dataset

Dataset: ted_hrlr_translate/pt_to_en
Source: TensorFlow Datasets
Includes aligned Portuguese–English sentence pairs from TED talks.

# 4. Model Architecture

Encoder:

Input layer

Embedding layer

LSTM (returns hidden + cell states)

Decoder:

Input layer

Embedding layer

LSTM with encoder states

Dense layer with softmax for predictions

Total parameters: ~47M
Trainable parameters: ~15M

# 5. Training Details

Number of samples used: 1000

Batch size: 32

Epochs: 3

Loss function: Sparse Categorical Crossentropy

Optimizer: Adam

Training accuracy reaches around 35%, which is expected for a small dataset.
