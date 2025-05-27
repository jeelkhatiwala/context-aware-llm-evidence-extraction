# CARE-LLM: Context-Aware LLM-based Evidence Extraction from SQLite Databases

This repository contains all datasets, code, and prompts related to the paper:

**"Leveraging LLMs for Context-Aware Extraction of Digital Evidence from SQLite Databases"**

The work introduces **CARE-LLM**, a novel framework that applies large language models (LLMs) to automate forensic evidence extraction from SQLite databases, especially from mobile applications.

---

## Repository Structure

Each folder corresponds to a Research Question (RQ) evaluated in the paper:

```
.
├── RQ1/                       # Accuracy comparison: context-aware vs. context-free
├── RQ2/                       # Generalizability across mobile apps (e.g., WhatsApp, Chrome)
├── RQ3(Schema_only)/          # Impact of schema-only context
├── RQ3(Schema_Value_only)/   # Impact of raw values only (no schema or metadata)
├── RQ4/                       # Scalability tests (small, medium, large databases)
└── README.md
```

Each folder includes:

* Input SQLite rows or test data
* Prompts used for LLMs
* Annotated ground truth
* Output results (e.g., JSON or CSV)
* Evaluation metrics (Precision, Recall, F1-score)

---

## Key Research Goals

| RQ      | Focus                                                                                                                                  |
| ------- | -------------------------------------------------------------------------------------------------------------------------------------- |
| **RQ1** | Does the context-aware record representation improve the accuracy of evidence entity extraction from SQLite databases when using LLMs? |
| **RQ2** | How generalizable is the context-aware extraction method across different mobile applications and database schemas?                    |
| **RQ3** | Which Components of the Context (Metadata vs. Schema Attributes) Contribute Most to the Accuracy of Evidence Extraction                |
| **RQ4** | How Does the Context-Aware LLM Extraction Method Scale with Increasing Database Size and Complexity in Forensic Investigations?        |
