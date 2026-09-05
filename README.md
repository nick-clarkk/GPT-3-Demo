# Shakespeare Transformer

A character-level transformer language model built from scratch in PyTorch, trained to generate Shakespeare-style text.

## Functionality

The model is trained on a collection of Shakespeare's text and learns to predict the next character given the preceding context. Once trained, it generates new text one character at a time, autoregressively,
producing output that mimics the style, vocabulary, and structure of the training text.

Implemented from scratch (no pretrained models or high-level transformer libraries), including:
- Token and positional embeddings
- Multi-head self-attention
- Dropout and layer normalization
- A full training loop with train/validation loss tracking

## Results

Training loss dropped from ~4.8 to 1.48 over 5,000 iterations.

## Running it

```bash
pip install torch
python gpt.py
```

## Data

Trained on `input.txt`, a plain-text collection of Shakespeare's works (character-level tokenization, no subword/BPE tokenizer).

## Credit

Built by following [Andrej Karpathy's "Let's build GPT" tutorial](https://www.youtube.com/watch?v=kCc8FmEb1nY).
