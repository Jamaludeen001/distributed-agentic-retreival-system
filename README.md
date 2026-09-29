# Distributed Agentic Retrieval System

A research-driven framework for exploring distributed retrieval pipelines, agent-based orchestration, semantic search, and document intelligence.

This repository contains experiments and implementations focused on Retrieval-Augmented Generation (RAG), document processing, vector search, query understanding, and multi-agent workflows. The project serves as a learning and experimentation platform for building scalable retrieval systems that combine document intelligence with agentic reasoning.

---

## Overview

Modern AI systems depend heavily on the quality of information retrieval. This project explores how multiple specialized components can work together to improve retrieval quality, relevance, and response generation.

The repository includes:

- Query Understanding (NLU)
- Document Chunking Strategies
- PDF Preprocessing
- Vector Embedding Generation
- FAISS-Based Semantic Search
- Retrieval Evaluation Workflows
- Agent-Oriented Retrieval Experiments
- Spark-Based Embedding Pipelines

---

## Key Features

### Document Processing

- PDF cleaning and normalization
- Preprocessing pipeline for downstream retrieval tasks
- Chunk generation for semantic indexing

### Chunking Strategies

- Sentence-based chunking
- Structure-aware chunking
- Chunk storage and management

### Query Understanding

- Natural Language Understanding (NLU)
- Query preprocessing
- Retrieval-oriented query analysis

### Vector Retrieval

- FAISS vector indexing
- Embedding-based search
- Similarity retrieval experiments
- Retrieval performance evaluation

### Agentic Workflows

- Agent orchestration experiments
- Retrieval-focused agents
- Distributed decision-making concepts
- Response generation pipelines

### Scalable Processing

- Spark-based embedding workflows
- Metadata handling
- Large-scale document experimentation

---

## High-Level Architecture

```text
                    User Query
                         │
                         ▼
              Query Understanding
                         │
                         ▼
               Document Processing
                         │
        ┌────────────────┼────────────────┐
        │                │                │
        ▼                ▼                ▼
  PDF Cleaning   Sentence Chunking  Structure-Aware
                                      Chunking
        │                │                │
        └────────────────┼────────────────┘
                         ▼
              Embedding Generation
                         │
                         ▼
                 FAISS Vector Store
                         │
                         ▼
                     Retrieval
                         │
                         ▼
                    Agent Layer
                         │
                         ▼
                 Generated Response
```

---

## Repository Structure

```text
distributed-agentic-retreival-system/
│
├── environment 1/
│   ├── query understanding(NLU) notebook.py
│   ├── sentence_chunking_notebook.py
│   ├── structure_aware_chunking_notebook.py
│   ├── server.py
│   │
│   ├── Agents/
│   │   ├── agent.py
│   │   ├── agent.md
│   │   └── dataq_agent.py
│   │
│   └── staging/
│       └── chunks/
│
├── environment 2/
│   ├── FAISS_index_vectorstore_notebook.py
│   ├── faiss_retreival_testing_notebook.py
│   ├── spark_embedding_store_notebook.py
│   ├── spark_metadata_notebook.py
│   ├── unloading_dbfs_zip_notebook.py
│   ├── dbfs_testing_noteook.py
│   └── test.py
│
├── tools/
│   ├── chunker/
│   │   └── sentence_chunker.py
│   │
│   ├── pdf_cleaner/
│   │   └── cleaner.py
│   │
│   └── tree_plot/
│       └── nx_plotly_treeplot.py
│
├── staging/
│   └── chunk/
│
├── _spark_test_out/
│
├── LICENSE
├── README.md
├── reference_in.md
├── reference_out.md
└── sample_test.txt
```

---

## Project Components

### Query Understanding

Responsible for analyzing user input and preparing queries for downstream retrieval components.

Files:

```text
environment 1/query understanding(NLU) notebook.py
```

### Chunking Module

Implements multiple chunking approaches to improve retrieval effectiveness.

Files:

```text
environment 1/sentence_chunking_notebook.py
environment 1/structure_aware_chunking_notebook.py
tools/chunker/sentence_chunker.py
```

### PDF Processing

Handles document cleaning and preprocessing before chunking and indexing.

Files:

```text
tools/pdf_cleaner/cleaner.py
```

### Vector Retrieval

Contains experiments related to embedding generation, vector indexing, and retrieval testing.

Files:

```text
environment 2/FAISS_index_vectorstore_notebook.py
environment 2/faiss_retreival_testing_notebook.py
environment 2/spark_embedding_store_notebook.py
environment 2/spark_metadata_notebook.py
```

### Agent Experiments

Explores agent-based coordination and retrieval workflows.

Files:

```text
environment 1/Agents/
```

---

## Installation

### Clone Repository

```bash
git clone https://github.com/Jamaludeen001/distributed-agentic-retreival-system.git

cd distributed-agentic-retreival-system
```

### Create Virtual Environment

```bash
python -m venv venv
```

### Activate Environment

#### Windows

```bash
venv\Scripts\activate
```

#### Linux / Mac

```bash
source venv/bin/activate
```

### Install Dependencies

```bash
pip install -r requirements.txt
```

> Note: Some experimental modules may require additional dependencies depending on the environment being used.

---

## Running Experiments

### Query Understanding

```bash
python "environment 1/query understanding(NLU) notebook.py"
```

### Sentence Chunking

```bash
python "environment 1/sentence_chunking_notebook.py"
```

### Structure-Aware Chunking

```bash
python "environment 1/structure_aware_chunking_notebook.py"
```

### Retrieval Server

```bash
python "environment 1/server.py"
```

### Build FAISS Index

```bash
python "environment 2/FAISS_index_vectorstore_notebook.py"
```

### Retrieval Testing

```bash
python "environment 2/faiss_retreival_testing_notebook.py"
```

---

## Technologies Used

- Python
- FAISS
- Apache Spark
- Vector Embeddings
- Semantic Search
- Retrieval-Augmented Generation (RAG)
- Information Retrieval
- Agentic AI Concepts
- Natural Language Understanding (NLU)

---

## Research Goals

This project explores:

- Agent-based retrieval architectures
- Efficient document chunking strategies
- Semantic retrieval optimization
- Embedding generation workflows
- Retrieval evaluation techniques
- Distributed retrieval pipelines
- Scalable RAG system design

---

## Future Improvements

- Hybrid retrieval (Dense + Sparse Search)
- Vector database integration
- Advanced reranking models
- LangGraph-based orchestration
- Multi-modal retrieval
- Agent memory systems
- Distributed deployment
- Real-time document ingestion pipelines

---

## Related Work

This repository focuses primarily on retrieval systems, document intelligence, and agentic experimentation.

Some experimental components included in this repository have since evolved into independent projects with their own repositories and documentation.

---

## License

This project is licensed under the MIT License.

See the LICENSE file for details.

---

## Author

**Jamaludeen**

GitHub: https://github.com/Jamaludeen001
``
