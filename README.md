
<h1 align="center">Soubhik Sinha</h1> <h3 align="center">AI Engineer — Agentic Voice AI, RAG & Production GenAI Infrastructure</h3> <p align="center"> <a href="https://www.linkedin.com/in/sinhasoubhik/">LinkedIn</a> • <a href="mailto:work.soubhiksinha@gmail.com">Email</a> • <a href="https://github.com/SoubhikSinha">GitHub</a> </p> <p align="center"> Building the infrastructure and safety layer under a production GenAI platform — from an agentic voice AI assistant to a PostgreSQL routing layer offloading <b>60–70% of read traffic</b> at scale. </p>

----------

## About

AI Engineer at Hexaware, owning the infrastructure and safety layer under a production GenAI platform — not the LLM calls themselves, but everything that has to work correctly, safely, and fast around them.

-   Architecting an **agentic voice AI assistant** end to end — direct-pgvector retrieval, Redis-backed session state, Kafka-surface eventing — holding **sub-1.3s** end-to-end latency under multi-tenant load
-   Built a **dual-LLM guardrail architecture** (FSM-scoped tool allow-listing + independent verifier model) blocking prompt-injection and unauthorized tool execution at **~150ms** overhead
-   Built a **real-time PII audio-redaction pipeline** on LiveKit Cloud egress — ASR-timestamp-mapped FFmpeg tone-masking — achieving **98% redaction recall** across SSN/card/phone/email on every recorded call
-   Architected a PostgreSQL read/write routing layer with automatic SQL safety classification, cutting replica read load by **60–70%** while preserving write consistency
-   Built a caching layer that took repeat embedding calls from **~200ms → ~1ms**, adopted platform-wide
-   Built a Health Status API aggregating real-time status across **16 service dependencies** (Kafka, Flyte, Azure OpenAI, Azure AI Search, Redis, Blob Storage)
-   Owned database + Blob Storage design for a vendor ingestion system used by **100+ engineers**; built the migration runbook now used as team standard (1M+ docs, zero data loss)

## Tech Stack

<p align="center"> <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white"/> <img src="https://img.shields.io/badge/PyTorch-EE4C2C?style=for-the-badge&logo=pytorch&logoColor=white"/> <img src="https://img.shields.io/badge/LangChain-1C3C3C?style=for-the-badge&logo=langchain&logoColor=white"/> <img src="https://img.shields.io/badge/LangGraph-1C3C3C?style=for-the-badge&logo=langgraph&logoColor=white"/> <br> <img src="https://img.shields.io/badge/LiveKit-FF3B3B?style=for-the-badge&logoColor=white"/> <img src="https://img.shields.io/badge/Voice%20AI-000000?style=for-the-badge&logoColor=white"/> <img src="https://img.shields.io/badge/Agentic%20Systems-000000?style=for-the-badge&logoColor=white"/> <br> <img src="https://img.shields.io/badge/Elasticsearch-005571?style=for-the-badge&logo=elasticsearch&logoColor=white"/> <img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white"/> <img src="https://img.shields.io/badge/Apache%20Kafka-231F20?style=for-the-badge&logo=apachekafka&logoColor=white"/> <img src="https://img.shields.io/badge/Redis-DC382D?style=for-the-badge&logo=redis&logoColor=white"/> <br> <img src="https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white"/> <img src="https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white"/> <br> <img src="https://img.shields.io/badge/Microsoft%20Azure-0078D4?style=for-the-badge&logo=microsoftazure&logoColor=white"/> <img src="https://img.shields.io/badge/OpenAI-412991?style=for-the-badge&logo=openai&logoColor=white"/> <img src="https://img.shields.io/badge/HuggingFace-FFD21E?style=for-the-badge&logo=huggingface&logoColor=black"/> </p>

## Featured Work

### [RAG-ElasticSearch-OpenLLM](https://github.com/SoubhikSinha/RAG-ElasticSearch-OpenLLM)

Built a hybrid retrieval RAG system from scratch — sparse (BM25, ELSER) + dense vector search combined via Reciprocal Rank Fusion — to understand the core mechanics behind LLM-assistant products (retrieval, grounding, memory). Benchmarked retrieval quality, latency, and ranking across Elasticsearch, LlamaIndex, LangChain (FAISS/Chroma), and MongoDB Vector Search using automated `pytest` evaluation.

### [Multi-Source GTM Intelligence Engine](https://github.com/SoubhikSinha/Multi-Source-GTM-Search-Engine)

Built a fully async, multi-agent research system (Query Strategy → Execution → Evaluator → Refiner → Synthesis) that autonomously investigates companies across news, web, and company sites — sustaining **80+ concurrent searches** via semaphore-controlled `asyncio`/`aiohttp`, with GPT-4o query planning and a confidence-scoring loop that auto-refines low-confidence results. Exposed via FastAPI batch and SSE streaming endpoints.

### [Chest Disease Detection — DenseNet-ViT Hybrid](https://github.com/SoubhikSinha/Chest-Disease-Detection-Using-Custom-DenseNet-ViT-Architecture)

Designed a lightweight multi-task DenseNet-121–Vision Transformer hybrid with three task-specific heads, classifying pneumonia, tuberculosis, and lung cancer from chest X-ray/CT images across **11K+ medical images**. Full pipeline (CLAHE preprocessing, augmentation, training, eval) with a deployed interactive demo on Hugging Face Spaces. _MS capstone, Computer Vision & Image Processing — reference project, not actively maintained._

## Currently

Building agentic voice AI infrastructure at production scale — real-time data/state layers, LLM guardrails, and PII-safe systems that hold up when the model call is the easy part.
