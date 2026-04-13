# TeamprojectX - XAI: INSIDE

This repository contains the code and implementation for our Explainable AI (XAI) course project in the 6th Semester, 3rd year.

**Authors:**
- Ishan Srivastava (23BDS023)
- Tejas Chalwadi (23BDS063)

**Course:** Explainable AI
**Supervisor:** Dr. Siddharth R.

## Project Description

This project implements and explores the concepts presented in the following research paper:

> **[INSIDE: LLMs' Internal States Retain the Power of Hallucination Detection](https://arxiv.org/abs/2402.03744)**

### What Does the Script Do?
The provided Jupyter notebook (`INSIDE_Team_ProjectX.ipynb`) demonstrates hallucination detection in Large Language Models (LLMs) by analyzing their internal states. 
- It examines the dense semantic information retained within the models.
- It applies the **EigenScore** metric to evaluate the self-consistency of model responses by exploiting the eigenvalues of the responses' covariance matrix in the dense embedding space.
- It explores a **test-time feature clipping approach** to truncate extreme activations in the internal states, which effectively reduces overconfident generations and aids in detecting hallucinations.

### Testing INSIDE in RAG Architecture
In addition to the core methodology, this project extends the evaluation by testing the INSIDE framework within a **Retrieval-Augmented Generation (RAG)** architecture. We evaluate the effectiveness of hallucination detection when the LLM is grounded with external context, investigating how internal state patterns and metrics like EigenScore behave during retrieval-augmented reasoning.
