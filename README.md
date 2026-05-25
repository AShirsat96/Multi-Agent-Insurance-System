# Multi-Agent Insurance Support System

**An intelligent, multi-agent conversational AI system built with LangGraph to automate insurance support workflows.**

This project implements a sophisticated agentic architecture designed to handle customer inquiries, process claims documentation, and interact with a structured database, all while maintaining conversation context and agent state.

## Overview

Moving beyond simple LLM chatbots, this system utilizes **LangGraph** to define a stateful, multi-agent workflow. It decomposes complex support tasks into specialized agents (e.g., Triage, Claims Analysis, Billing, Database Query) that collaborate to resolve user issues effectively.

## Key Features

* **Multi-Agent Orchestration:** Uses a Supervisor-Agent pattern to route tasks efficiently to specialized sub-agents.
* **Stateful Conversations:** Leverages LangGraph to maintain context across multi-turn interactions.
* **RAG & Database Integration:** Uses ChromaDB for policy lookups and SQLite for structured data querying.
* **Guard rails for infinite loops:** The supervisor logic includes escalation protocols to prevent routing errors.
* **Modular Design:** Specialized agents (Billing, Claims, General Help) can be updated or added independently.

## Workflow Architecture

The system uses a Supervisor-Agent pattern to route tasks efficiently.

## Tech Stack

* **Language:** Python
* **Orchestration:** LangGraph (LangChain)
* **AI/LLM:** OpenAI
* **Database:** SQLite & ChromaDB

## Project Structure

```text
multi-agent-system/
├── multi-agent_system_no_phoenix.ipynb  # Main multi-agent system
├── requirements.txt                     # Python dependencies
├── enhanced_workflow.mmd                # Mermaid workflow diagram
├── chroma_db/                           # Vector database storage
├── insurance_support.db                 # SQLite database
└── README.md

```

## Setup & Installation

1. **Clone the repository:**
```bash
git clone https://github.com/AShirsat96/Multi-Agent-Insurance-System.git
cd Multi-Agent-Insurance-System

```


2. **Install dependencies:**
```bash
pip install -r requirements.txt

```


3. **Configure environment variables:**
Create a `.env` file in the root directory (do not commit this file!):
```env
OPENAI_API_KEY=your_key_here

```



---

## 📄 License

This project is open-source and available under the MIT License.

---

*Built with ❤️ using LangGraph, OpenAI, and ChromaDB*
