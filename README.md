# RAG---QA-System-using-LlamaIndex-on-Coca-Cola-Data
Enterprise Question Answering (QA) System built using LlamaIndex and RAG to query and extract insights from Coca-Cola's 2024 Annual Report.

## Overview

This project demonstrates how to build an enterprise-style Question Answering (QA) system using LlamaIndex and Retrieval-Augmented Generation (RAG) techniques.

The system ingests Coca-Cola's 2024 Annual Report (10-K filing), converts the document into searchable chunks, generates embeddings, builds vector indexes, and answers user questions using Large Language Models (LLMs).

The project explores multiple retrieval strategies available in LlamaIndex and compares their effectiveness in answering questions from financial and corporate reports.

---

## Business Problem

Organizations store large volumes of unstructured information in annual reports, financial statements, policies, and research documents.

Manually searching these documents for answers is time-consuming and inefficient.

This project demonstrates how AI-powered retrieval systems can:

* Extract relevant information from lengthy documents
* Improve information accessibility
* Enable natural language querying
* Support faster decision-making

---

## Dataset

**Source:** Coca-Cola 2024 Annual Report (10-K Filing)

The report was downloaded directly from Coca-Cola's investor relations website and used as the knowledge source for the QA system.

---

## Technology Stack

* Python
* LlamaIndex
* OpenAI
* HuggingFace Embeddings
* ChromaDB
* PyMuPDF
* Google Colab

---

## Solution Architecture

1. Download and load Coca-Cola annual report
2. Parse PDF using PyMuPDFReader
3. Split document into chunks using SentenceSplitter
4. Generate embeddings using BAAI/bge-small-en-v1.5
5. Create VectorStoreIndex
6. Persist index for reuse
7. Build retrieval pipelines
8. Query using natural language questions
9. Generate responses using OpenAI LLMs

---

## Retrieval Techniques Implemented

### Basic Vector Retrieval

Standard semantic search using vector embeddings.

### Sentence Window Retriever

Retrieves surrounding context to improve answer quality.

### Auto Merging Retriever

Combines related chunks dynamically before response generation.

### Auto Retriever

Automatically determines optimal retrieval parameters.

### Router Query Engine

Routes questions to the most suitable retrieval strategy.

### Sub Question Query Engine

Breaks complex questions into smaller questions and synthesizes results.

---

## Example Questions

* Tell me about Coca-Cola's business.
* What are Coca-Cola's major risks?
* What properties does Coca-Cola own?
* What are the company's growth strategies?
* Summarize key financial highlights.

---

## Key Learning Outcomes

* Retrieval-Augmented Generation (RAG)
* Document indexing and retrieval
* Embedding models
* Vector databases
* Query engine design
* Multi-step question answering
* Enterprise document intelligence

---

## Future Enhancements

* Deploy as a web application
* Add conversational memory
* Support multiple documents
* Integrate hybrid search
* Add evaluation metrics for retrieval quality
* Compare embedding models

---

## Author

**Antony Pradeep Raj**

Product Manager | AI & Generative AI Enthusiast

This project was completed as part of the Generative AI Pinnacle learning journey.

