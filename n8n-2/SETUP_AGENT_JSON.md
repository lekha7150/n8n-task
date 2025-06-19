# Quickstart Guide: Advanced Q&A Agent with Pinecone, Groq, and Hugging Face (n8n)

Welcome! This guide will walk you through setting up your AI-powered Q&A Agent using the provided `agent.json` workflow in n8n. This agent leverages Pinecone for vector storage, Groq for chat generation, and Hugging Face for embeddings.

---

## 1. What You Need
- **n8n** (latest version, self-hosted or cloud)
- **Pinecone** account and index
- **Groq** API credentials
- **Hugging Face** API key
- (Optional) Any other n8n integrations you wish to add

---

## 2. Preparation Steps

### a. Pinecone Setup
- Register at [Pinecone](https://www.pinecone.io/).
- Create an index (e.g., `qa-bot`) and note your API key and environment.

### b. Groq & Hugging Face
- Obtain your Groq API key from your Groq dashboard.
- Get a Hugging Face API key from [Hugging Face](https://huggingface.co/settings/tokens).

### c. n8n Credentials
- In n8n, add credentials for Pinecone, Groq, and Hugging Face under **Credentials**.

---

## 3. Importing the Workflow
1. Open n8n and go to **Workflows**.
2. Click **Import** and select your `agent.json` file.
3. Review the imported nodes and connections.

---

## 4. Configuration Checklist
- **Pinecone Vector Store Node**: Set your Pinecone index name and namespace (e.g., `qa-bot`, `IOS`).
- **Groq Chat Model Node(s)**: Ensure your Groq credentials are selected.
- **Hugging Face Embeddings Node**: Choose your Hugging Face model and credentials.
- **System Message**: Edit the system prompt in the agent node if you want to customize the agent's behavior.

---

## 5. How It Works
- The workflow listens for chat messages.
- It retrieves relevant context from Pinecone using Hugging Face embeddings.
- The Groq model generates a response, using both retrieved context and conversation memory.

---

## 6. Testing Your Agent
- Trigger the workflow by sending a chat message (via webhook or UI).
- Check the response for accuracy and context.
- Adjust parameters or prompts as needed for your use case.

---

## 7. Troubleshooting
- **No Response?** Double-check your API keys and node credentials.
- **Irrelevant Answers?** Refine your Pinecone namespace or system prompt.
- **Errors in n8n?** Review node logs for credential or configuration issues.

---

## 8. Customization Ideas
- Add more tools or data sources as needed.
- Tweak the system message for a different agent persona.
- Integrate with other n8n workflows for notifications or logging.

---

## 9. Example Prompts
- "What is Retrieval-Augmented Generation (RAG)?"
- "Summarize the last conversation."
- "What information is stored in the vector database?"

---

Happy automating! For advanced customization, refer to the n8n and Pinecone documentation. 