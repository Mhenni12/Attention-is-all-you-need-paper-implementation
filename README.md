# Transformer Implementation — "Attention Is All You Need"

This repository contains my implementation of the Transformer architecture inspired by the seminal paper *“Attention Is All You Need”* (Vaswani et al., 2017).

The goal of this project was to deeply understand and reimplement the core ideas behind the Transformer model from scratch, focusing on its key building blocks and how they interact in both the encoder and decoder stacks.

---

## 🚀 Project Overview

The implemented model follows the original Transformer architecture and is built by composing all fundamental components manually, rather than relying on high-level library abstractions.

### 🔑 Key Implemented Components

- **Positional Encoding**
  - Injects sequential information into the model since Transformers lack recurrence.
  
- **Multi-Head Attention**
  - Allows the model to jointly attend to information from different representation subspaces.

- **Position-wise Feed-Forward Networks**
  - Fully connected layers applied independently to each position.

- **Encoder Block**
  - Stack of:
    - Multi-head self-attention
    - Feed-forward network
    - Residual connections + Layer normalization

- **Decoder Block**
  - Stack of:
    - Masked multi-head self-attention
    - Encoder-decoder attention
    - Feed-forward network
    - Residual connections + Layer normalization

- **Full Transformer Architecture**
  - Stacked encoder and decoder layers forming the complete sequence-to-sequence model.

---

## 🧠 What I Learned

- How attention mechanisms replace recurrence and convolution in sequence modeling
- The importance of positional encoding in order-aware representations
- How encoder-decoder attention enables effective sequence-to-sequence learning
- The role of residual connections and normalization in stabilizing deep architectures
- Practical challenges in implementing Transformers from scratch

---

## 🛠️ Tech Stack

- Python
- NumPy / PyTorch
- Jupyter Notebook

---

## 📌 Future Improvements

- Add training pipeline on a real dataset (e.g., translation task)
- Implement label smoothing and learning rate scheduling (warmup + decay)
- Experiment with different attention heads and depth configurations
- Optimize performance using modern transformer variants

---

## 📚 Reference

- Vaswani et al., 2017 — *Attention Is All You Need*

---

## ⭐ Acknowledgements

This project is part of my learning journey in deep learning and NLP, aimed at building a strong intuitive and practical understanding of transformer-based architectures.