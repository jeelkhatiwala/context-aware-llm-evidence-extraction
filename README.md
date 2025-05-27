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

| RQ      | Focus                                                                                 |
| ------- | ------------------------------------------------------------------------------------- |
| **RQ1** | Does using context-aware record representations improve evidence extraction accuracy? |
| **RQ2** | Is the method generalizable across different apps and schemas?                        |
| **RQ3** | Which context component (schema, metadata, raw values) matters most?                  |
| **RQ4** | Can the method scale with increasing data size and schema complexity?                 |
