# RepairRAG

Evidence-Grounded Repair Intelligence using Retrieval-Augmented Generation

---

## Project Overview
RepairRAG is a system designed to answer repair-related questions by retrieving relevant information from repair manuals and combining the retrieved evidence with a language model to generate accurate, grounded, and reliable answers.

The main purpose of this project is to reduce hallucinations in language model outputs by making sure responses are based on real repair documentation such as iFixit guides and technical repair manuals.

Instead of directly asking a language model for an answer, RepairRAG first retrieves the most relevant repair content and then uses that evidence to generate a final response.

---

## Demo Screenshot

![RepairRAG Demo]("C:\Users\nilas\OneDrive\Desktop\1.png")

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
