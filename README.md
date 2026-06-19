# NexusAI-Platform 🤖💼
> **Autonomous AI Agent Marketplace with Advanced RAG Production Pipeline**

<div align="center">
  

  <video src="https://github.com/user-attachments/assets/687bb050-ba3f-49c7-bf98-3a06a1b4eb6e" width="100%" autoplay loop muted playsinline>
  </video>

</div>



NexusAI is a professional, high-performance landing page and autonomous sales ecosystem designed for deploying and selling specialized AI Agents (Support, Analyst, and Custom Ops). The architecture bridges a modern, user-friendly frontend directly to an enterprise-grade Retrieval-Augmented Generation (RAG) chatbot backend driven by n8n.

---

## ⚡ Key Highlights
* **Conversion-Oriented UI:** A high-end, responsive dark-themed landing page customized with optimized container layouts for premium readability and structural balance.
* **Production n8n Backed:** Seamless live integration with a full local workflow via webhooks.
* **Context-Aware Sales RAG:** Powered by vector-embedded knowledge bases to ensure autonomous, hallucination-free business conversions.

---

## 📂 Repository Architecture & Core Components

### 1. `index.html` (The Landing Page)
The standalone frontend interface built with modern, optimized CSS. It includes custom layout containers with wide margins/paddings (`max-width: 1280px`) designed specifically to look flawless on both Ultra-Wide monitors and mobile devices. It natively injects the asynchronous n8n chat widget configuration, complete with custom CSS overrides for perfect float overlay (`z-index: 9999`) and deep theme-matching colors.

### 2. `Ai Agent for Agent Sales Website with RAG.json` (The Backend Workflow)
The complete production-ready n8n workflow export. This file contains the architecture for:
* Webhook trigger management for real-time frontend chat sync.
* Advanced orchestration using LangChain / n8n AI components.
* Vector Store memory retrieval using **Gemini Dense Embeddings** (optimized natively for 768-dimension semantic lookups).

### 3. `MyWebsiteDetailsForRAG_DB.txt` (The Knowledge Base)
A meticulously structured markdown data sheet acting as the core knowledge repository for the RAG database. It features detailed system prompts, operational constraints, product portfolios, pricing structures, and an extensive, multi-tier FAQ pipeline. 

---

## 🧠 The RAG Pipeline & Intelligent Context Matching

The core intelligence of this platform relies on the ingestion of `MyWebsiteDetailsForRAG_DB.txt` into our Vector Database. 

When a visitor interacts with the chat bubble on `index.html`, the n8n RAG engine matches the user's semantic intent against the embedded text coordinates. As a result, the chatbot dynamically synthesizes answers using a mix of **its own generative intelligence** and **strict contextual data boundaries** outlined in the knowledge base.

### 🎥 Demo & Workflow Verification
We have included a full recorded demonstration video in this repository. In this demo, you can watch the entire workflow live:
1. Posing highly specific customer queries regarding pricing tiers, security protocols, and CRM integration scopes.
2. The RAG engine instantly fetching and parsing text clusters from `MyWebsiteDetailsForRAG_DB.txt`.
3. The chatbot generating precise, business-compliant, and high-converting answers natively on the web interface.

---

## 🚀 Quick Start Guide

1. **Deploy Frontend:** Open `index.html` locally or host it on any web server.
2. **Import Workflow:** Open your n8n instance, click **Import from File**, and upload `Ai Agent for Agent Sales Website with RAG.json`.
3. **Seed Vector Store:** Load `MyWebsiteDetailsForRAG_DB.txt` into your n8n-connected Vector Store Document Loader (e.g., Qdrant, Pinecone, or Chroma) using Gemini Embeddings (3072 Dimensions).
4. **Active & Connect:** Update the Webhook URL parameter inside the `index.html` widget configuration to match your live n8n node, and activate the workflow.
