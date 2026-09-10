
<h1 align="center">Soubhik Sinha</h1> <h3 align="center">AI Engineer — Agentic Voice AI, RAG & Production GenAI Infrastructure</h3> <p align="center"> <a href="https://www.linkedin.com/in/sinhasoubhik/">LinkedIn</a> • <a href="mailto:work.soubhiksinha@gmail.com">Email</a> • <a href="https://github.com/SoubhikSinha">GitHub</a> </p> <p align="center"> I build the layer under the model call — the data, the guardrails, and the systems that fail quietly if you get them wrong. </p>

----------

## About

AI Engineer at Hexaware, working on the infrastructure and safety layer underneath a production agentic voice AI assistant — not the model calls themselves, but the retrieval, guardrails, and data systems that sit around them and have to hold up under real load.

I care about one specific intersection: agentic systems useful enough to ship, and infrastructure disciplined enough that useful never comes at the cost of safe. In practice, that's meant building dual-LLM guardrails that catch prompt-injection before it reaches a tool call, a real-time PII redaction pipeline that scrubs sensitive data out of every recorded call, and a database routing layer that keeps read-heavy traffic off the write path without anyone noticing.

Before voice AI, I was the sole database owner for a knowledge-ingestion platform used across a 100+ engineer org — which is where I learned that most "AI failures" are actually data-layer failures wearing a model's name.

## Currently

Building agentic voice AI infrastructure at production scale — real-time data/state layers, LLM guardrails, and PII-safe systems that hold up when the model call is the easy part.

## Featured Work

### [RAG-ElasticSearch-OpenLLM](https://github.com/SoubhikSinha/RAG-ElasticSearch-OpenLLM)

Hybrid retrieval RAG system combining sparse (BM25, ELSER) and dense vector search via Reciprocal Rank Fusion, built to understand what actually happens inside a RAG pipeline — retrieval, grounding, citations. Runs four independently selectable retrieval modes over a live Elasticsearch index and cuts hallucinated answers by 40% against a non-RAG baseline.

### [Multi-Source GTM Intelligence Engine](https://github.com/SoubhikSinha/Multi-Source-GTM-Search-Engine)

Fully async, multi-agent research system (Strategy → Execution → Evaluator → Refiner → Synthesis) that autonomously investigates companies across news, web, and company sites, sustaining 80+ concurrent searches with a confidence-scoring loop that auto-refines weak results.

### [LLM From Scratch (GPT, PyTorch)](https://github.com/SoubhikSinha/LLM-from-scratch-using-Python)

Wanted to know what's actually happening inside a language model before trusting one in production. Built a transformer-based GPT from scratch — from a bi-gram baseline up through the full architecture in _Attention Is All You Need_ — trained on OpenWebText and shipped as both a CLI chatbot and a Gradio app.

### [Chest Disease Detection — DenseNet-ViT Hybrid](https://github.com/SoubhikSinha/Chest-Disease-Detection-Using-Custom-DenseNet-ViT-Architecture)

Multi-task DenseNet-ViT hybrid trained from scratch, with three heads classifying pneumonia, tuberculosis, and lung cancer from chest X-ray/CT images. Deployed live on Hugging Face Spaces.

## Tech Stack

<p align="center">
	<img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white"/>														
	<img src="https://img.shields.io/badge/PyTorch-EE4C2C?style=for-the-badge&logo=pytorch&logoColor=white"/> 
	<img src="https://img.shields.io/badge/LangChain-1C3C3C?style=for-the-badge&logo=langchain&logoColor=white"/> 
	<img src="https://img.shields.io/badge/LangGraph-1C3C3C?style=for-the-badge&logo=langgraph&logoColor=white"/> 
<br> 
<img src="https://img.shields.io/badge/LiveKit-1FD5F9?style=for-the-badge&logo=livekit&logoColor=black"/>
<img src="https://img.shields.io/badge/Deepgram-CE2029?style=for-the-badge&logo=deepgram&logoColor=white"/>
<img src="https://img.shields.io/badge/Presidio-0078D4?style=for-the-badge&logoColor=white"/>
<br> 
	<img src="https://img.shields.io/badge/Elasticsearch-005571?style=for-the-badge&logo=elasticsearch&logoColor=white"/> 
	<img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white"/> 
	<img src="https://img.shields.io/badge/Apache%20Kafka-231F20?style=for-the-badge&logo=apachekafka&logoColor=white"/> 
	<img src="https://img.shields.io/badge/Redis-DC382D?style=for-the-badge&logo=redis&logoColor=white"/> <br> 
	<img src="https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white"/> 
	<img src="https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white"/> <br> 
	<img src="https://img.shields.io/badge/Microsoft%20Azure-0078D4?style=for-the-badge&logo=microsoftazure&logoColor=white"/> 
	<img src="https://img.shields.io/badge/OpenAI-412991?style=for-the-badge&logo=openai&logoColor=white"/> 
	<img src="https://img.shields.io/badge/HuggingFace-FFD21E?style=for-the-badge&logo=huggingface&logoColor=black"/> 
</p>

---
<p align="left"><i>Open to conversations about that harder-scale problem—where useful and safe are genuinely in tension, not resolved by default. </i></p>
