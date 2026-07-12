<h1 align="center">Soubhik Sinha</h1>
<h3 align="center">AI Engineer — GenAI Platform Infrastructure & Production RAG Systems</h3>

<p align="center">
  <a href="https://www.linkedin.com/in/sinhasoubhik/">LinkedIn</a> •
  <a href="mailto:work.soubhiksinha@gmail.com">Email</a> •
  <a href="https://github.com/SoubhikSinha">GitHub</a>
</p>

<p align="center">
Architected a PostgreSQL read/write routing layer offloading <b>60–70% of read traffic</b> on a production GenAI platform — designing for scale from a 3.5K-user launch toward 20K.
</p>

---

## About

AI Engineer at Hexaware, owning the infrastructure layer under a production GenAI platform — not the LLM calls themselves, but everything that has to work correctly around them.

- Architected PostgreSQL read/write routing with automatic SQL safety classification, cutting replica read load by **60–70%** while preserving write consistency
- Built a caching layer that took repeat embedding calls from **~200ms → ~1ms**
- Built a Health Status API aggregating real-time status across **16 service dependencies** (Kafka, Flyte, Azure OpenAI, Azure AI Search, Redis, Blob Storage)
- Owned database + Blob Storage design for a vendor ingestion system used by **100+ engineers**; built the migration runbook now used as team standard (1M+ docs, zero data loss)


## Tech Stack

**Core** : 
<p>
<img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white"/>
<img src="https://img.shields.io/badge/PyTorch-EE4C2C?style=for-the-badge&logo=pytorch&logoColor=white"/>
<img src="https://img.shields.io/badge/LangChain-1C3C3C?style=for-the-badge&logo=langchain&logoColor=white"/>
<img src="https://img.shields.io/badge/LangGraph-1C3C3C?style=for-the-badge&logo=langgraph&logoColor=white"/>
</p>

**GenAI**
<p>
<img src="https://img.shields.io/badge/RAG-4B8BBE?style=for-the-badge&logoColor=white"/>
<img src="https://img.shields.io/badge/LLM%20Evaluation-4B8BBE?style=for-the-badge&logoColor=white"/>
<img src="https://img.shields.io/badge/Azure%20OpenAI-0078D4?style=for-the-badge&logo=microsoftazure&logoColor=white"/>
<img src="https://img.shields.io/badge/Elasticsearch-005571?style=for-the-badge&logo=elasticsearch&logoColor=white"/>
</p>

**Infra & Data**
<p>
<img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white"/>
<img src="https://img.shields.io/badge/Apache%20Kafka-231F20?style=for-the-badge&logo=apachekafka&logoColor=white"/>
<img src="https://img.shields.io/badge/Flyte-4300FA?style=for-the-badge&logo=flyte&logoColor=white"/>
<img src="https://img.shields.io/badge/Redis-FF4438?style=for-the-badge&logo=redis&logoColor=white"/>
<img src="https://img.shields.io/badge/Azure%20Blob%20Storage-0078D4?style=for-the-badge&logo=microsoftazure&logoColor=white"/>
</p>

**Serving**
<p>
<img src="https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white"/>
<img src="https://img.shields.io/badge/ONNX-005CED?style=for-the-badge&logo=onnx&logoColor=white"/>
<img src="https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white"/>
</p>

## Featured Work

### [Multi-Source GTM Intelligence Engine](https://github.com/SoubhikSinha/Multi-Source-GTM-Search-Engine)
Built a fully async, multi-agent research system (Query Strategy → Execution → Evaluator → Refiner → Synthesis) that autonomously investigates companies across news, web, and company sites — sustaining **80+ concurrent searches** via semaphore-controlled `asyncio`/`aiohttp`, with GPT-4o query planning and a confidence-scoring loop that auto-refines low-confidence results. Exposed via FastAPI batch and SSE streaming endpoints.

### [RAG-ElasticSearch-OpenLLM](https://github.com/SoubhikSinha/RAG-ElasticSearch-OpenLLM)
Built a hybrid retrieval RAG system from scratch — sparse (BM25, ELSER) + dense vector search combined via Reciprocal Rank Fusion — to understand the core mechanics behind LLM-assistant products (retrieval, grounding, memory). Benchmarked retrieval quality, latency, and ranking across Elasticsearch, LlamaIndex, LangChain (FAISS/Chroma), and MongoDB Vector Search using automated `pytest` evaluation.

### [Chest Disease Detection — DenseNet-ViT Hybrid](https://github.com/SoubhikSinha/Chest-Disease-Detection-Using-Custom-DenseNet-ViT-Architecture)
Designed a lightweight multi-task DenseNet-121–Vision Transformer hybrid with three task-specific heads, classifying pneumonia, tuberculosis, and lung cancer from chest X-ray/CT images across **11K+ medical images**. Full pipeline (CLAHE preprocessing, augmentation, training, eval) with a deployed interactive demo on Hugging Face Spaces. *MS capstone, Computer Vision & Image Processing — reference project, not actively maintained.*

## Currently
Deepening GenAI infrastructure at production scale — read/write data layers, observability, and inference cost/latency tradeoffs for systems beyond the single-model call.
