# 🔍 Improved Retrieval-Augmented Generation (RAG)

This project implements a **Retrieval-Augmented Generation (RAG)** system and enhances it using **query refinement, re-ranking, and context filtering** to improve answer quality.

---

## 📌 Overview

Traditional Large Language Models (LLMs) suffer from **hallucination** and lack of up-to-date knowledge.
RAG addresses this by retrieving relevant documents and using them as context.

In this project:

* A **baseline RAG system** is implemented
* An **improved RAG system** is proposed and evaluated

---

## 🚀 Features

### 🔴 Baseline RAG

* PDF document loading
* Text chunking
* Embedding generation (Sentence Transformers)
* Vector storage using FAISS
* Similarity-based retrieval
* Answer generation using FLAN-T5

### 🟢 Improved RAG

* ✅ Query Refinement (reduces ambiguity)
* ✅ Re-ranking using cosine similarity
* ✅ Context Filtering (removes noise)
* ✅ Improved answer quality

---

## 🧠 Architecture

### Baseline Pipeline

User Query → Embedding → FAISS Retrieval → LLM → Answer

### Improved Pipeline

User Query → Query Refinement → Retrieval → Re-ranking → Filtering → LLM → Answer

---

## 🛠️ Tech Stack

* Python (Jupyter Notebook)
* FAISS (Vector Database)
* Sentence Transformers (Embeddings)
* Transformers (FLAN-T5 for generation)
* NumPy, Scikit-learn

---

## 📂 Dataset

* Custom PDF documents (AI, NLP, RAG concepts)
* Text is split into chunks for embedding and retrieval

---

## ⚙️ How It Works

1. Load PDF documents
2. Split text into chunks
3. Convert text to embeddings
4. Store embeddings in FAISS
5. Input user query
6. Retrieve top-k relevant chunks
7. Apply improvements (refinement, re-ranking, filtering)
8. Generate final answer

---

## 📊 Results

| Model        | Performance                       |
| ------------ | --------------------------------- |
| Baseline RAG | Noisy, less relevant responses    |
| Improved RAG | More accurate and focused answers |

---

## 🔬 Key Contributions

* Identified limitations of similarity-based retrieval
* Proposed improvements in retrieval stage
* Demonstrated qualitative performance gain

---

## 📄 Base Paper

This work is based on:

**Retrieval-Augmented Generation for Knowledge-Intensive NLP Tasks**
(Lewis et al., 2020)

---

## 🔮 Future Work

* LLM-based query refinement
* Advanced re-ranking (cross-encoders)
* Hybrid retrieval (dense + sparse)
* Quantitative evaluation metrics

---

## 📌 How to Run

1. Clone the repository
2. Install dependencies:

   ```bash
   pip install faiss-cpu sentence-transformers transformers
   ```
3. Open the Jupyter Notebook:

   ```bash
   jupyter notebook
   ```
4. Run all cells step-by-step

---

## 📎 Example Queries

* What is RAG?
* Explain transformers
* What is hallucination?

---

## 🎯 Conclusion

The project demonstrates that **improving the retrieval stage** significantly enhances the performance of RAG systems.

---

## 👨‍💻 Author

Jeel Patel

---

## ⭐ Acknowledgement

Inspired by research in Generative AI and Retrieval-Augmented Generation.
