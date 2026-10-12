[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/CtKjnZeu)
#  ClinicalRAG: Intelligent Healthcare Assistance with LLMs and Medical Knowledge Retrieval


##  Problem Statement

Healthcare professionals often face information overload while searching through thousands of pages of medical references. This project addresses that challenge by building an intelligent assistant capable of retrieving relevant medical knowledge and generating concise, evidence-based responses in real time.

---

##  Objectives

* Build a Retrieval-Augmented Generation (RAG) pipeline for healthcare.
* Retrieve relevant information from the Merck Manual.
* Generate medically grounded responses using Llama-2.
* Reduce hallucinations through document-based retrieval.
* Evaluate the quality of generated responses using relevance and groundedness metrics.

---

##  Dataset

**Source:** Merck Manual

* Medical reference containing over **4,000 pages**
* Covers multiple medical specialties
* Used as the knowledge base for retrieval

---

##  Technologies Used

* Python
* LangChain
* Llama-2
* ChromaDB
* HuggingFace Embeddings
* PyMuPDF
* Google Colab
* Pandas

---

##  Project Workflow

1. Load the Merck Manual PDF.
2. Extract text from the document.
3. Split the document into smaller chunks.
4. Generate embeddings using HuggingFace.
5. Store embeddings in ChromaDB.
6. Retrieve the most relevant chunks based on user queries.
7. Generate grounded responses using the Llama-2 model.
8. Evaluate the responses using LLM-as-a-Judge.

---

##  Features

* Evidence-based medical question answering
* Semantic document retrieval
* Reduced hallucinations
* Fast retrieval using vector search
* Clinically relevant and grounded responses
* Evaluation using relevance and groundedness scores

---

## Evaluation

The system was evaluated using an **LLM-as-a-Judge** framework.

### Metrics

* Relevance Score
* Groundedness Score

### Results

* High relevance across medical questions.
* Strong groundedness through retrieved Merck Manual content.
* Significant reduction in hallucinated responses.
* Reliable and evidence-backed medical answers.

---

##  Project Structure

```text
├── Medical_Manual.pdf
├── Module_II_Project_II.ipynb
├── chroma_db/
├── README.md
└── requirements.txt


##  Future Improvements

* Hybrid Retrieval (BM25 + Vector Search)
* Re-ranking models for improved retrieval
* Integration with newer medical literature
* Multi-document retrieval
* Real-time evaluation dashboard
* Deployment as a web application using Streamlit or Gradio



