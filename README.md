# Comparing-Arabic-Transformer-Models-for-Question-Answering-Task-NLP-PROJECT-


This repository contains the full pipeline used to fine-tune and evaluate **two Arabic transformer models** for **extractive question answering**:

- **MARBERTv2**
- **CAMeLBERT** (Classical Arabic variant / CA)

The project follows the standard extractive QA setup (SQuAD-style), where the model predicts the **start** and **end** token positions of the answer span within the context.

---

## Project Overview

### What we did
- Unified multiple Arabic QA datasets into a **consistent SQuAD-style format**:
  `(id, question, context, answers)`
- Fine-tuned **MARBERTv2** and **CAMeLBERT** using the **HuggingFace Trainer**.
- Applied HuggingFace **post-processing** to convert model logits into final text answers.
- Evaluated performance using:
  - **Exact Match (EM)**
  - **F1-score** (token-level overlap)

### Key notes
- We used the **original dataset splits** provided by the dataset authors.
- Reported results are presented on the **test set** (depending on the training configuration).

---

