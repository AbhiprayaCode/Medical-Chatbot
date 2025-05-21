# CareSense – Precision Care, Anytime You Need

> A digital AI assistant to improve access to reliable health information and guidance.

---

![LangChain](https://img.shields.io/badge/Framework-LangChain-4287f5?logo=langchain&logoColor=white)  
![Pinecone](https://img.shields.io/badge/VectorDB-Pinecone-9B51E0?logo=window&logoColor=white)  
![Hugging Face](https://img.shields.io/badge/Embeddings-Hugging%20Face-FF6A00?logo=huggingface&logoColor=white)  
![Streamlit](https://img.shields.io/badge/UI-Streamlit-FF4E30?logo=streamlit&logoColor=white)  
![MongoDB](https://img.shields.io/badge/Database-MongoDB-47A248?logo=mongodb&logoColor=white)  

---

## 📋 Table of Contents

1. [Theme](#theme)  
2. [Problem & Objectives](#problem--objectives)  
3. [Method](#method)  
   - [Proposed AI Method](#proposed-ai-method)  
   - [Libraries & Tools](#libraries--tools)  
   - [Data Processing](#data-processing)  
4. [Expected Results](#expected-results)  
5. [References](#references)  
6. [Log Hours](#log-hours)

---

## Theme

Leveraging AI to improve access to health information and guidance by building a responsive chatbot that delivers timely, personalized medical advice—helping users make informed decisions without overloading healthcare systems.

---

## Problem & Objectives

### Problem

- Many people face long wait times, limited specialist access, and unreliable online information.  
- Delays or misinformation can worsen health outcomes.

### Objectives

1. **Easy Access**  
   - Build an AI assistant that answers common medical questions using trusted sources.  
2. **Personalized Advice**  
   - Tailor guidance to individual user needs for more actionable insights.  
3. **Preventive Healthcare**  
   - Encourage early detection and healthy habits with clear risk information.  
4. **Reduce Healthcare Strain**  
   - Automate basic inquiries to free up professionals for complex cases.

---

## Method

### Proposed AI Method

- **Chatbot Core**  
  - Uses NLP models for understanding and responding to health queries.  
  - LangChain orchestrates document loading, splitting, and QA workflows.  
  - Pinecone stores and retrieves vectorized medical knowledge.

### Libraries & Tools

| Component              | Role                                     |
|------------------------|------------------------------------------|
| **LangChain**          | Orchestrates document processing & QA    |
| **Pinecone**           | Vector database for semantic search      |
| **Hugging Face**       | Embedding models for text vectorization  |
| **Streamlit**          | Web UI framework for the chatbot         |
| **PyPDFLoader / CSVLoader** | Load and parse PDF/CSV medical data  |
| **MongoDB**            | Stores chat logs & user interactions     |

### Data Processing

1. **Extraction**  
   - Load PDFs via PyPDFLoader; CSVs via CSVLoader.  
2. **Chunking**  
   - Split text into manageable segments with RecursiveCharacterTextSplitter.  
3. **Embedding**  
   - Convert chunks into vectors using Hugging Face embeddings.  
4. **Indexing & Retrieval**  
   - Index embeddings in Pinecone for rapid, context-aware lookup.

---

## Expected Results

- A live AI chatbot “CareSense” capable of accurate, on-demand health advice.  
- Improved user access to reliable medical information and preventive guidance.  
- Reduced routine query load on healthcare providers.  
- Clear, jargon-free summaries of complex health topics.  
- A modular framework ready to incorporate new medical datasets and features.

---

## References

- [LangChain Documentation](https://www.langchain.com/)  
- [Pinecone Documentation](https://www.pinecone.io/)  
- [Hugging Face](https://huggingface.co/)  
- [Streamlit Docs](https://docs.streamlit.io/)  
- [MongoDB Manual](https://www.mongodb.com/)

