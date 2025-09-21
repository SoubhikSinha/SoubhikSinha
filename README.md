# Playing Around with  `Langchain`

<p align="center">
  <img src="https://registry.npmmirror.com/@lobehub/icons-static-png/latest/files/dark/langchain-color.png" alt="LangChain" height="100"/>&nbsp;&nbsp;
	<img src="https://github.com/SoubhikSinha/SoubhikSinha/blob/main/extras/Screenshot%202025-09-19%20at%2018.23.09.png" alt="LangServe" height="60"/>&nbsp;&nbsp;
  <img src="https://registry.npmmirror.com/@lobehub/icons-static-png/latest/files/dark/langsmith-color.png" alt="LangSmith" height="100"/>
</p>
<br>

<p align="center">
  <img src="https://img.shields.io/badge/Python-3.12+-blue.svg" />
  <img src="https://img.shields.io/badge/LangChain-0.3.x-green.svg" />
  <img src="https://img.shields.io/badge/LangServe-0.3.x-brightgreen.svg" />
  <img src="https://img.shields.io/badge/FastAPI-0.115+-teal.svg" />
  <img src="https://img.shields.io/badge/Streamlit-1.49+-red.svg" />
  <img src="https://img.shields.io/badge/Ollama-0.5.x-orange.svg" />
  <img src="https://img.shields.io/badge/LangSmith-Latest-lightgrey.svg" />
</p>
<br>

## About this Repo

This repository is a practical playground for experimenting with **LangChain-powered chatbots**, built on **FastAPI** and integrating both **OpenAI GPT models** and a locally hosted **LLaMA 3.2 via Ollama** for hybrid inference. It leverages **LangServe** to expose modular routes accessible via RESTful APIs or an interactive **Streamlit interface**, making it flexible for both prototyping and production-style workflows. Core features include **prompt templates, chains, and parsers** for conversational flow management, **hybrid model switching** between cloud and local inference, **LangSmith integration** for tracing and debugging, and reproducible environments through `.env` and `requirements.txt`. Serving as both a **learning resource** and a **starter kit** for **RAG pipelines, prompt engineering, and LLM experimentation**, this project is inspired by the tutorials and guidance of [**Krish Naik**](https://github.com/krishnaik06).
<br>
<br>

## How to Play Around ?
### **1. Create a Virtual Environment**
Navigate to the project root and create a Conda virtual environment (Python 3.12):
```bash
conda create --prefix ./venv python=3.12 -y
```

### **2. Activate the Conda Environment**
Activate the newly created environment:
```bash
conda activate venv/
```

### **3. Install Dependencies**
Install all the required libraries from `requirements.txt`:
```bash
pip install -r requirements.txt
```

### **4. Set Up API Keys and Project Name**
Create a `.env` file in the root directory and add your credentials:
```bash
OPENAI_API_KEY="your_openai_api_key_here"
LANGCHAIN_API_KEY="your_langsmith_api_key_here"
LANGCHAIN_PROJECT="ChatBotOpenAIProject"
```
-   Get your OpenAI key from [OpenAI Platform](https://platform.openai.com/).
-   Get your LangSmith key from [LangSmith](https://www.langchain.com/langsmith).

### **5. Download Ollama and Models**
Install [Ollama](https://ollama.com/) and pull the LLaMA 3.2 model (or any other you want to experiment with):
```bash
ollama run llama3.2:1b
```

### **6. Run the Application**
Start the Streamlit application:
-   **Using OpenAI (cloud-based):**
	```bash
	streamlit run chatbot/app.py
	```
- **Using Ollama (local LLM):**
	```bash
	streamlit run chatbot/local_llama.py
	```

### **7. Run the FastAPI Backend (Swagger UI)**
If you want to explore the API endpoints via Swagger:
```bash
python api/app.py
```
Then open any browser and go to:
```bash
http://localhost:8000/docs
```
⚠️ **Note:** The latest pydantic and langserve libraries may not be fully compatible and could throw errors. If that happens, you can still test APIs at:
-   http://localhost:8000/essay/playground/
-   http://localhost:8000/poem/playground/

### **8. Run the Streamlit Client (API Frontend)**
You can also launch a **Streamlit client app** that consumes the FastAPI backend:
```bash
streamlit run api/client.py
```

### **9. Play Around 🚀**
Experiment with both **OpenAI** and **Ollama** modes, test out the **FastAPI routes**, monitor your interactions in **LangSmith**, and enjoy building with **LangChain + Streamlit + FastAPI**!
