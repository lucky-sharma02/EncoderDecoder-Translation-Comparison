# English → Spanish Neural Machine Translation using BiLSTM with Attention

## Project Overview

This project implements a Neural Machine Translation (NMT) system using a Seq2Seq Encoder–Decoder architecture with a Bidirectional LSTM (BiLSTM) encoder and Bahdanau Attention decoder.

The model translates short English sentences into Spanish and is inspired by the research paper:

**Efficient Machine Translation with a BiLSTM-Attention Approach (2024)**

---

## Features

* English → Spanish translation
* BiLSTM Encoder
* Bahdanau Attention Mechanism
* Seq2Seq Architecture
* Attention Heatmap Visualization
* Comparison between:

  * Seq2Seq with Attention
  * Seq2Seq without Attention

---

## Dataset

The project uses a small hardcoded English–Spanish dataset containing:

* Greetings
* Colors
* Animals
* Numbers
* Simple phrases

### Example Dataset

| English      | Spanish     |
| ------------ | ----------- |
| hello        | hola        |
| cat          | gato        |
| red          | rojo        |
| good morning | buenos días |

---

## Model Architecture

```text
English Sentence
       ↓
Embedding Layer
       ↓
BiLSTM Encoder
       ↓
Bahdanau Attention
       ↓
LSTM Decoder
       ↓
Dense + Softmax
       ↓
Spanish Translation
```

---

## Technologies Used

* Python
* PyTorch
* NumPy
* Matplotlib

---

## Training Details

| Parameter      | Value              |
| -------------- | ------------------ |
| Optimizer      | Adam               |
| Loss Function  | CrossEntropyLoss   |
| Epochs         | 30                 |
| Attention Type | Bahdanau Attention |

---

## Results

### Seq2Seq WITH Attention

* Lower validation loss
* Better translation quality
* Improved contextual understanding

### Seq2Seq WITHOUT Attention

* Higher validation loss
* Poorer word alignment
* Lower translation accuracy

The attention-based model performed significantly better than the basic Seq2Seq model.

---

## Attention Heatmap

The project visualizes attention weights using a heatmap.

The heatmap shows:

* Which English words the decoder focuses on
* How attention changes during translation generation

Example:

* Source sentence: `"the cat is small"`
* Predicted translation: `"el gato es pequeno"`

---

## Learning Outcomes

This project helps understand:

* Seq2Seq models
* Encoder–Decoder architecture
* BiLSTM networks
* Attention mechanisms
* Neural Machine Translation
* Attention visualization

---

## Reference Paper

**Efficient Machine Translation with a BiLSTM-Attention Approach (2024)**

https://arxiv.org/abs/2410.22335
