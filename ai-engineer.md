# AI Engineer – Technical Interview Questions

At Capco, we’re building autonomous AI systems that integrate multi‑modal LLMs and agentic workflows for the financial services industry. This role demands a strong blend of AI/ML engineering, software development, and MLOps.

Below you’ll find the topics and example questions we may ask during your technical interview. Use them to guide your preparation.

---

## Core Topics

### 1. LLMs & Multi‑Modal Models
- How do you choose between fine‑tuning, RAG, and prompt engineering for a given business problem?
- Explain how multi‑modal models (text + image + audio) are integrated. What challenges arise in latency and performance?
- Describe techniques to reduce hallucination in LLM outputs for regulated financial environments.
- How would you evaluate an LLM used for financial document summarisation? Which metrics and test data would you use?

### 2. Agentic Systems & Frameworks
- What is an “agentic workflow”? How would you design an agent that can query multiple APIs and decide which tool to use?
- Compare LangChain, LlamaIndex, and a custom framework. When would you use each?
- How do you implement memory and state management in a conversational AI agent?
- How would you design an approval or human‑in‑the‑loop mechanism around an action‑taking agent in a bank?

### 3. MLOps & Production Deployment
- Walk me through a production‑grade ML pipeline for a generative AI service – from data ingestion to inference.
- How do you monitor drift, bias, and performance in a live LLM system? Mention tools like Langfuse or Langsmith.
- What’s your experience with cloud‑native AI deployment (e.g., AWS SageMaker, Azure ML, or Kubernetes + KServe)?
- How would you design CI/CD for a GenAI service where both prompts and models change over time?

### 4. Python & Backend Engineering
- You need to serve a fine‑tuned LLM with strict latency requirements (<100ms). How do you structure the API and optimise inference?
- How do you handle asynchronous tasks (e.g., long‑running fine‑tuning jobs) in a FastAPI or Django application?
- Write a simple decorator that logs execution time and token usage for any LLM call.
- How would you design a rate‑limited, multi‑tenant API for a GenAI service?

### 5. RAG, Evaluation & Observability
- What metrics would you collect for a RAG pipeline? How would you alert on degradation?
- Describe a strategy for A/B testing two different prompt templates in production.
- How do you scale a vector database (e.g., Pinecone, Weaviate, or pgvector) as the number of embeddings grows to millions?
- How would you measure and reduce hallucinations on a bank‑specific corpus (e.g., policies, product docs)?

### 6. Enterprise Integration, Governance & Risk
- How would you mitigate bias and hallucinations when deploying a GenAI solution for a tier‑1 bank?
- Explain the Model Context Protocol (MCP) and its relevance to agentic systems.
- What governance steps would you introduce before allowing an LLM to execute actions on live financial data?
- How would you design auditability and traceability (who asked what, which model responded, which tools were called) for an AI system in production?

---

## Sample Coding / System Design Exercise

> *You will be given a small problem statement during the interview – here’s an example of what to expect:*

**Task:**  
Build a REST endpoint that accepts a user query, retrieves relevant context from a provided set of PDF documents (using RAG), and returns an answer from an LLM. The solution must include:
- Document chunking & embedding
- A simple similarity search
- A prompt that includes the retrieved context
- A way to log the query, context, and answer for observability

**Expected discussion points:**  
- Choice of embedding model and vector store  
- Handling document updates without rebuilding everything  
- Latency optimisation (cache, streaming, batching)  
- How you would test for hallucination on this specific data  
- How to secure the endpoint and protect sensitive financial data  

---

## Additional Experience We Value

- Experience with **LangChain**, **LlamaIndex**, or similar agentic frameworks  
- Familiarity with **Langfuse**, **Langsmith**, or **OpenTelemetry** for LLM observability  
- Understanding of **model fine‑tuning techniques** (LoRA, QLoRA, PEFT)  
- Hands‑on experience with **Kubernetes**, **KServe**, or similar for model deployment  
- Contributions to open‑source AI projects or a strong GitHub portfolio  

---

## How You’ll Be Assessed

- **Depth of knowledge** in the topics above, not just buzzwords  
- **Clean, maintainable code** (Python) and thoughtful API design  
- **Ability to reason about trade‑offs** (cost, latency, accuracy, safety)  
- **System thinking** – how your solutions fit into enterprise architectures  
- **Communication** – explaining complex AI concepts to both technical and non‑technical stakeholders  

Good luck! We’re excited to see how you approach modern AI engineering.
