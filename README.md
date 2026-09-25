# Sakash Srivastava

**AI Engineer building LLM agents and RAG systems.** Shipped two LLM systems solo this year, one live on Azure with CI/CD, authentication and a full test suite. Research background in computer vision and medical imaging at King's College London.

[LinkedIn](https://linkedin.com/in/sakash-srivastava) · [Email](mailto:sakashsrivastava06@gmail.com) · [SegLit live demo](https://seglit.duckdns.org/)

Open to AI engineer roles and internships. Available remotely now or onsite from January 2027.

---

## Featured projects

### [SegLit: Agentic RAG Research Assistant](https://github.com/SakashSrivastava/Agentic-Research-Assistant-for-Segmentation-Literature) · [Live](https://seglit.duckdns.org/)

Answers comparative questions over 276 medical image segmentation papers, with citations.

- Layout-aware ingestion of 2,435 PDF pages and 732 result tables into 8,139 embeddings across ChromaDB and BM25, queried by a hand-written tool-calling agent.
- Verified metrics table (829 rows) with a verbatim source-match check that discards the 5% of extracted values not found in the source.
- Retrieval benchmarked on 52 hand-labelled questions (recall@5, MRR). Agent re-implemented in LangGraph to compare hand-written and framework designs.
- Secure multi-user Flask app on Azure with Docker, GitHub Actions CI/CD, authentication, rate limiting and a 26-check integration test suite.

`Python` `Flask` `ChromaDB` `SQLite` `LangGraph` `Docker` `Azure` `GitHub Actions`

### [Multi-Agent Orchestration System](https://github.com/SakashSrivastava/Agent-Orchestration)

Supervisor, specialist and reviewer agents built from scratch, with no agent framework.

- A supervisor plans dependency-ordered tasks, specialists run sandboxed tools, and an LLM-as-judge reviewer checks every output against verified tool logs.
- Feeding the reviewer verified tool-call evidence cut false rejections from 5 in 6 to zero.
- SQLite-backed state makes crash recovery and human-in-the-loop approval one pause/resume mechanism, with per-call token, cost and latency tracking in Streamlit.
- 19-test suite including sandbox-escape tests, Docker packaging and documented design decisions.

`Python` `Pydantic` `SQLite` `Streamlit` `Docker`

### [AI Finance Controller](https://github.com/SakashSrivastava/AI_Finance_Controller)

Reconciles invoices, payment-gateway settlements and bank statements. Deterministic matching runs first, an LLM agent only sees what the code couldn't match, and an arithmetic gate re-derives every proposal.

`Python` `LLM Agents`

### [Real Estate Price Prediction](https://github.com/SakashSrivastava/real-estate-price-prediction)

Flask app serving real-time price predictions on 13,000+ Bengaluru listings. XGBoost (80%+ R²) with engineered features and Isolation Forest outlier removal.

`Python` `XGBoost` `Flask`

---

## Open source

- **[BasedHardware/omi](https://github.com/BasedHardware/omi):** 2 merged pull requests.

## Research and experience

- **King's College London**, Visiting Research Intern (2026): built a CT-to-MRI registration pipeline that cut bone annotation from hours per case to minutes across 40+ cases, and set an nnU-Net v2 baseline of 0.938 mean Dice across 9 orbital structures.
- **UpValue Tech**, Machine Learning Intern (2025): built a counterfeit sneaker verification pipeline with OpenCV and dual OCR, chose a custom CNN after benchmarking 6 model families, and explained every flag to moderators with Grad-CAM.
- **NSUT Delhi**, Research Intern (2025): extended the TLcR-RL face super-resolution framework with adaptive per-patch neighbour selection and prototyped an ANFIS model for it.

## Tech stack

- **LLM and agents:** LangGraph, LangChain, RAG, tool calling, structured outputs, embeddings, ChromaDB, vector search
- **ML and vision:** Scikit-learn, XGBoost, OpenCV, nnU-Net, SimpleITK, OCR (Tesseract, EasyOCR)
- **Engineering:** Python, C++, SQL, Flask, REST APIs, Pydantic, Docker, Azure, GitHub Actions

## Highlights

- Top 5% at Adobe India Hackathon 2025
