### Hi, I'm Sufian 👋

AI Engineer with a B.Sc. in Artificial Intelligence. I build LLM applications end to end: RAG, tool-calling agents, and the tests and evaluations that prove they work.

📍 Baton Rouge, LA · open to Austin, Dallas, San Francisco, New York, or remote

[![LinkedIn](https://img.shields.io/badge/LinkedIn-sufian--kanaan-0A66C2?logo=linkedin&logoColor=white)](https://www.linkedin.com/in/sufian-kanaan)
[![Live demo](https://img.shields.io/badge/Live_demo-AI_Car_Assistant-FFD21E?logo=huggingface&logoColor=black)](https://huggingface.co/spaces/ksufian/ai-car-assistant)

---

### 🚗 Featured: [AI Car Assistant](https://github.com/Sufiankanaan/ai-car-assistant) · [try it live](https://huggingface.co/spaces/ksufian/ai-car-assistant)

A LangGraph agent with conversation memory that answers car questions. For each question it decides whether to search a knowledge base (RAG over an FTC used-car guide) or run a fuel, loan, or total-cost calculator.

- **Agent:** LangGraph + Gemini API, memory per browser session, model retry and fallback when the API is busy
- **Number guard:** a middleware blocks a calculator call if the model invented a number the user never gave, and the agent asks for it instead
- **RAG:** PDF/Word ingestion, cleaned chunks with source ids, ChromaDB, and a relevance threshold (0.85) calibrated from measured distances
- **Evaluation:** 17-case golden set with tool and keyword checks, LLM-as-judge for faithfulness, Langfuse tracing
- **Engineering:** 16 pytest tests on every pull request with GitHub Actions; `main` is protected and deploys to Hugging Face only when tests pass
- **MCP:** the same calculators are exposed as an MCP server

| Metric | Before | Now |
|---|---|---|
| Golden set | 14/15 | 17/17 (2 multi-turn cases added) |
| Faithfulness (search answers) | 6/7 | 7/7 |

---

### 🧩 Other projects

| Project | What it shows | Stack |
|---|---|---|
| [llm-rag-system](https://github.com/Sufiankanaan/llm-rag-system) | RAG from scratch with cited sources and a retrieval-accuracy eval | Python · Ollama · ChromaDB |
| [llm-agent](https://github.com/Sufiankanaan/llm-agent) | Tool-calling loop with JSON-schema tools, error handling, logging | Python · Ollama |
| [Patient-Management-System-API](https://github.com/Sufiankanaan/Patient-Management-System-API) | ML model served through a REST API with full CRUD and validation | FastAPI · Pydantic v2 · scikit-learn · Docker |

---

### 🛠️ Toolbox

**LLM & GenAI:** RAG · AI agents · LangGraph · tool calling · embeddings · LLM evaluation (golden sets, LLM-as-judge) · Langfuse · MCP<br>
**Tools:** Gemini API · Ollama · ChromaDB · Gradio · Streamlit · Hugging Face Spaces · scikit-learn · pandas<br>
**Engineering:** Python · FastAPI · Pydantic · Docker · SQL · Git · GitHub Actions · pytest
