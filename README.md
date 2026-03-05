# RepairRAG



Evidence-Grounded Repair Intelligence using Retrieval-Augmented Generation

## Project Overview
RepairRAG is a system designed to answer repair-related questions by retrieving relevant information from repair manuals and combining it with a language model to generate accurate and evidence-based responses. 

The goal of the project is to reduce hallucinated answers from language models by grounding responses in real repair documentation such as iFixit manuals and repair guides.

Instead of relying purely on a language model, RepairRAG retrieves relevant document chunks first and then generates answers based on that retrieved evidence.

---

## Problem Statement
Repair manuals and technical documentation contain valuable information, but finding the exact repair instructions can be difficult and time consuming. Traditional search methods often return long documents without clear answers.

RepairRAG addresses this problem by:
- Retrieving the most relevant repair instructions
- Providing concise answers
- Grounding answers with supporting evidence

---

## Project Objectives
The main objectives of this project are:

- Build a Retrieval-Augmented Generation (RAG) pipeline for repair documentation
- Reduce hallucinations in generated responses
- Retrieve repair instructions from technical documentation
- Provide evidence-backed answers to repair questions
- Evaluate different retrieval and model strategies

---

## System Architecture

The system follows a typical RAG pipeline:

User Question  
        ↓  
Document Retrieval  
        ↓  
Relevant Repair Manual Chunks  
        ↓  
Language Model  
        ↓  
Evidence-Grounded Answer

Key components include:
- Document preprocessing
- Chunking repair manuals
- Retrieval mechanism
- Language model generation
- Evaluation of responses

---

## Dataset
The project uses repair documentation and manuals such as:

- iFixit repair guides
- Repair manuals and technical documentation

Dataset processing includes:
- Cleaning the text
- Splitting documents into chunks
- Preparing the data for retrieval

---

## Methodology

### 1. Data Preparation
- Collect repair manuals
- Clean and preprocess text
- Split documents into meaningful chunks

### 2. Retrieval
Relevant document sections are retrieved using retrieval methods such as:
- BM25 (keyword-based retrieval)
- Dense embeddings (semantic search)
- Hybrid retrieval

### 3. Answer Generation
A language model generates answers based on the retrieved document chunks.

### 4. Evaluation
The model is evaluated based on:
- Answer accuracy
- Retrieval relevance
- Model reliability

---

## Key Challenges
Some challenges encountered during the project include:

- Class imbalance in the dataset
- Visually similar repair cases causing prediction confusion
- Model confidence not always reflecting correctness
- Need for more diverse training data

---

## Current Progress
- Exploratory Data Analysis (EDA) completed
- Baseline model trained and evaluated
- Dataset quality analyzed
- Model behavior studied to understand prediction patterns

---

## Future Work
Planned improvements include:

- Expanding dataset diversity
- Improving retrieval accuracy
- Testing different model architectures
- Evaluating ensemble approaches
- Improving overall system reliability

---

## Technologies Used
- Python
- Machine Learning / Deep Learning models
- Retrieval-Augmented Generation (RAG)
- Data analysis and preprocessing tools

---

## Contributors
- Aslesha Sanjana Kodavali
- Sai Nilasha Varma Indukuri
