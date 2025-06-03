# 📜 RAG-Based Semantic Quote Retrieval System

This project is part of an internship assignment from **Vijayi WFH Technologies Pvt Ltd**, aimed at building a semantic quote retrieval system using **RAG (Retrieval-Augmented Generation)**. The system can find quotes based on natural language queries like _"funny quotes by Oscar Wilde"_ and return relevant quotes with author and tags.

---

## 📌 Project Features

-  **Semantic Search**: Retrieve quotes using sentence embeddings and FAISS index.
-  **Transformer-based Embeddings**: Uses `all-MiniLM-L6-v2` from `sentence-transformers`.
-  **FAISS Indexing**: Fast similarity search on thousands of quotes.
-  **Streamlit App**: User interface to enter queries and get results.
-  **Manual Evaluation**: Sample queries to demonstrate retrieval accuracy.

---

## 🧰 Tech Stack

- `pandas`
- `sentence-transformers`
- `faiss`
- `streamlit`
- Dataset: [Abirate/english_quotes](https://huggingface.co/datasets/Abirate/english_quotes)

---


## 📊 Evaluation
A few test queries were run to evaluate the system. The retrieved quotes were found to be semantically accurate in most cases. Edge cases like vague or compound queries sometimes resulted in less relevant matches due to limitations in the base model and lack of context enrichment.

### Limitations:

- Retrieval is based only on quote + author + tags (not full context).

- Ambiguous queries (e.g., “life quotes that are sarcastic”) may confuse the index.

- Evaluation was done manually; RAGAS or Arize Phoenix could be added for future scoring.

