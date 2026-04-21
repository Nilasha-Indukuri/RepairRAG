# RepairRAG

Evidence-Grounded Repair Intelligence using Retrieval-Augmented Generation

---

## Project Overview
RepairRAG is a system designed to answer repair-related questions by retrieving relevant information from repair manuals and combining the retrieved evidence with a language model to generate accurate, grounded, and reliable answers.

The main purpose of this project is to reduce hallucinations in language model outputs by making sure responses are based on real repair documentation such as iFixit guides and technical repair manuals.

Instead of directly asking a language model for an answer, RepairRAG first retrieves the most relevant repair content and then uses that evidence to generate a final response.

---

## Demo Screenshot

<img width="1401" height="541" alt="image" src="https://github.com/user-attachments/assets/dd6f54fe-64bf-4449-8dbd-bfb9fc22dc44" />


---

## Problem Statement
Repair manuals and technical documentation contain valuable repair information, but users often face several difficulties while using them:

- Manuals are long and difficult to navigate
- Traditional keyword search may return incomplete or irrelevant results
- Users may struggle to locate exact repair steps quickly
- Language models alone may generate hallucinated or unsupported answers

RepairRAG addresses this problem by:

- Retrieving the most relevant repair instructions
- Providing concise and useful answers
- Grounding all generated responses in real documentation

---

## Project Objectives
The main objectives of this project are:

- Build a Retrieval-Augmented Generation (RAG) pipeline for repair documentation
- Reduce hallucinations in generated responses
- Retrieve accurate repair instructions from technical manuals
- Provide evidence-backed answers to user questions
- Evaluate different retrieval and answer-generation strategies

---
## Interface
The RepairRAG interface is a clean, dark-themed dashboard designed for querying repair questions and viewing evidence-grounded answers.

🔑 Key Features (Concise)
Search Bar: Enter natural language repair queries
Pipeline Display: Shows BM25 + Dense + Fusion + Re-ranking + LLM
System Sidebar: Displays chunks, models, and system status
Retrieval Slider: Adjusts number of retrieved results
Suggested Queries: Quick-access example questions
Abstention Mechanism: Avoids hallucinations when evidence is insufficient
Sources Panel: Shows retrieved guides with links and snippets

<img width="1024" height="580" alt="WhatsApp Image 2026-04-13 at 11 05 26 PM" src="https://github.com/user-attachments/assets/56c296cb-e139-40a0-865a-c8d3a93c3351" />

<img width="1470" height="832" alt="Screenshot 2026-04-13 at 11 03 30 PM" src="https://github.com/user-attachments/assets/db9a0ade-5e9f-4b95-b25e-eaecfda970c3" />


<img width="1470" height="832" alt="Screenshot 2026-04-13 at 11 03 35 PM" src="https://github.com/user-attachments/assets/1dc81a2f-b708-4cbe-90b2-1f082178efad" />
<img width="1470" height="832" alt="Screenshot 2026-04-13 at 11 03 40 PM" src="https://github.com/user-attachments/assets/53b827cb-d9de-4493-bc95-02ff3ccf9ba9" />

## System Architecture

The system follows a standard RAG pipeline:

```text
User Question
      ↓
Document Retrieval
      ↓
Relevant Repair Manual Chunks
      ↓
Language Model
      ↓
Evidence-Grounded Answer

