# Semantic Search & Retrieval Engine

A modern Information Retrieval (IR) platform that explores the evolution of search systems—from traditional keyword matching to semantic retrieval using transformer embeddings and the foundations of Retrieval-Augmented Generation (RAG).

Originally developed as an NLP project, this repository is being modernized into a document retrieval platform capable of indexing, searching, and discovering information across multiple documents using lexical and semantic retrieval techniques.

---

## Overview

Modern search systems are no longer limited to exact keyword matching. They combine linguistic preprocessing, semantic embeddings, vector search, and intelligent ranking to retrieve the most relevant information.

This project demonstrates that progression by implementing multiple retrieval strategies and incrementally evolving toward a lightweight Retrieval-Augmented Generation (RAG) architecture.

---

## Current Features

### Keyword Search

* Exact keyword matching
* Token-based retrieval
* Fast lexical search

### Lemmatized Search

* POS-aware lemmatization using NLTK
* Root-word matching
* Improved lexical recall

### Semantic Search

* Sentence Transformer embeddings
* Cosine similarity ranking
* Context-aware retrieval beyond exact keywords

### Web Interface

* Flask-based application
* Interactive search interface
* Multiple retrieval modes

---

## Modernization Roadmap

The project is being expanded into a modern semantic retrieval platform with the following capabilities:

### Phase 1 — Embedding Modernization

* Upgrade to modern embedding models (BGE Small / MiniLM)
* Faster and more accurate semantic retrieval
* Embedding caching

### Phase 2 — Document Retrieval

* PDF ingestion
* Text file ingestion
* Multi-document collections
* Metadata extraction

### Phase 3 — Chunk-Based Retrieval

* Intelligent document chunking
* Configurable chunk overlap
* Retrieval granularity optimization

### Phase 4 — Vector Search

* ChromaDB integration
* Persistent vector storage
* Efficient Top-K similarity search

### Phase 5 — Hybrid Retrieval

* Combine lexical and semantic retrieval
* Improved ranking strategies
* Retrieval evaluation and relevance scoring

### Phase 6 — Lightweight RAG

* Context construction from retrieved chunks
* LLM integration (OpenAI/Gemini)
* Source-grounded answer generation

---

## Architecture

```
                User Query
                     │
                     ▼
           Query Preprocessing
                     │
         ┌───────────┴───────────┐
         │                       │
         ▼                       ▼
 Keyword/Lexical Search   Semantic Embeddings
         │                       │
         └───────────┬───────────┘
                     ▼
              Hybrid Retrieval
                     ▼
              Similarity Ranking
                     ▼
              Top-K Results
                     ▼
        (Optional) Context Builder
                     ▼
               LLM Response
```

---

## Tech Stack

### Current

* Python
* Flask
* NLTK
* Sentence Transformers
* PyTorch
* NumPy

### Planned

* FastAPI
* ChromaDB
* SQLite
* PyMuPDF
* BAAI/bge-small-en-v1.5
* OpenAI / Gemini API

<!---

## Project Structure

```
semantic-search-retrieval-engine/

├── app.py
├── search/
├── nlp/
├── ingestion/
├── retrieval/
├── vector_store/
├── rag/
├── templates/
├── static/
├── documents/
└── README.md
```

--->

## Example Use Cases

* Search enterprise documentation
* Knowledge base exploration
* CMS content discovery
* Blog and article retrieval
* Product documentation search
* Internal knowledge search
* Semantic content discovery

Example queries:

* Find documents related to pet nutrition.
* Show content discussing probiotics.
* Retrieve pages mentioning puppies.
* Search documentation about authentication.

---

## Learning Objectives

This project explores:

* Natural Language Processing (NLP)
* Information Retrieval (IR)
* Semantic Search
* Transformer Embeddings
* Vector Databases
* Search Ranking
* Document Chunking
* Retrieval Evaluation
* Retrieval-Augmented Generation (RAG)

---

## Future Enhancements

* Hybrid BM25 + Semantic Retrieval
* Query Expansion
* Cross-Encoder Re-ranking
* Metadata Filtering
* Search Analytics
* REST API
* Docker Deployment
* Evaluation Benchmarks

---

## Why This Project?

Most AI projects begin with an LLM.

This project begins with **retrieval**, focusing on how modern search systems understand, rank, and retrieve information before introducing language models.

The objective is not to build another chatbot, but to understand the engineering principles behind semantic search, enterprise knowledge retrieval, and Retrieval-Augmented Generation systems.


<!-- # Semantic Search & Retrieval Engine

## Overview

The Semantic Search & Retrieval Engine offers three distinct search options:

- Basic Search functionality in this identifies sentences that directly contain the exact form of specified keywords, without any lemmatization applied. This search method is effective for precise matches based on the literal appearance of keywords in the text.

- Root Word Search employs lemmatization to match sentences based on the root forms of the provided keywords. This approach allows for a more comprehensive search, capturing variations of the keywords and enhancing the scope of relevant results.

- Context Search leverages BERT embeddings, a state-of-the-art natural language processing technique. By assessing contextual similarity, this search option identifies sentences that contextually align with the input keywords, offering a nuanced and semantic understanding of the text. This method is particularly useful for uncovering sentences with similar meanings or themes.

## SetUp

1. Open the directory.
2. Install libraries: `pip install requirements.txt`
3. Run: ` python your_app_name.py`
4. By running run_app.py, it will download:

- nltk.download('punkt')
- nltk.download('averaged_perceptron_tagger')
- nltk.download('wordnet')

5. Open http://127.0.0.1:5000 on a browser.

## How to test ?

- Open TestCases Folder
- Use any test cases present in the folder.
- Add the paragraph in first input box and the keywords only in the second input box.
- Select what type of search you want to perform from the options: Basic, Root, Context -->
