# Q&A Agent Workflow for n8n

Welcome to the Q&A Agent Workflow! This project enables you to deploy an advanced AI-powered question-answering agent in n8n, leveraging Pinecone for vector storage, Groq for language generation, and Hugging Face for embeddings.

---

## 🚀 What is This?
This workflow (see `agent.json`) lets you build a conversational agent that can:
- Answer user queries with context-aware, fact-based responses
- Retrieve relevant information from a Pinecone vector database
- Use state-of-the-art language models (Groq) and embeddings (Hugging Face)
- Maintain conversation memory for coherent multi-turn interactions

---

## ✨ Features
- **Retrieval-Augmented Generation (RAG)** for accurate answers
- Modular n8n nodes for easy customization
- Integration with Pinecone, Groq, and Hugging Face APIs
- Configurable system prompt and memory window

---

## 🛠️ Setup
1. **Install n8n** (self-hosted or cloud)
2. **Add Credentials** for Pinecone, Groq, and Hugging Face in n8n
3. **Import the Workflow**: Go to n8n > Workflows > Import > Select `agent.json`
4. **Configure Nodes**:
   - Set your Pinecone index/namespace
   - Select your API credentials in each relevant node
   - (Optional) Edit the system prompt for your agent
5. **Activate the Workflow**

For detailed setup, see `SETUP_AGENT_JSON.md`.

---

## 💬 Usage
- Trigger the workflow by sending a chat message (via webhook or UI)
- The agent will respond with a contextually relevant answer
- Review and adjust parameters as needed for your use case

---

## 🧩 Customization
- Add new data sources or tools by inserting more n8n nodes
- Change the embedding model or LLM as desired
- Refine the system prompt for different agent personalities

---

## 📚 Documentation
- **Setup Guide:** `SETUP_AGENT_JSON.md`
- **Technical Details:** `TECHNICAL_AGENT_JSON.md`

---

## 🤝 Contributing
Pull requests and suggestions are welcome! Feel free to fork and adapt for your own use cases.

---

## 📄 License
This project is provided as-is for educational and prototyping purposes. Please review third-party service terms for production use. 
