# Intelligent Multi-Agent Insurance Support System

Traditional customer service chatbots frustrate users with canned responses, while raw LLMs pose massive liability risks due to hallucinations in policy coverage and billing. This enterprise-grade AI application -  **Intelligent Multi-Agent Support System** solves this by establishing a LangGraph-orchestrated network of specialized agents.

The system leverages **LangGraph** to coordinate specialized AI agents, **OpenAI GPT** for intelligent responses, **ChromaDB** for semantic retrieval, **SQLite** for structured customer and policy information, and **Chainlit** to provide an interactive conversational interface.


# Value Proposition
In high-volume customer service operations, routine queries—like policy checks, premium due dates, and claim status checks—consume up to **70% of support resources**. Standard chatbots fall short because they cannot pull live transactions, while raw LLMs present major compliance risks due to financial hallucinations.

This project introduces an **Intelligent Agentic Mesh** that:
*   **Deflects Core Ticket Volumes**: Automatically handles structured lookup transactions and FAQs.
*   **Ensures Zero Hallucinations**: Grounded in SQLite schemas to retrieve exact billing and claim records.
*   **Reduces Average Handling Time**: Resolves common user issues in seconds with dynamic, multi-desk routing.
*   **Improves Operational Auditability**: Traced via OpenTelemetry to ensure security boundaries and response quality.

# Project Overview

Insurance companies receive a wide range of customer enquiries, including policy information, billing questions, payment history, and requests for human assistance. Traditional chatbots often struggle with conversations that require multiple reasoning steps or access to different information sources.

This project demonstrates how a **Multi-Agent AI architecture** can automate customer support by intelligently routing requests to specialized AI agents while maintaining conversational context.

The goal was to build a modular AI assistant capable of handling realistic insurance support workflows using modern Agentic AI techniques.

---

# Business Problem

Customer support representatives spend significant time responding to repetitive enquiries such as:

- Insurance policy questions
- Premium and billing enquiries
- Payment history requests
- Customer information lookup
- Escalation to human representatives

A traditional chatbot usually relies on a single reasoning process, making it difficult to handle different responsibilities effectively.

This project demonstrates how multiple specialized AI agents can collaborate to provide more accurate and maintainable customer support.

---

# Key Features

- Multi-Agent workflow using LangGraph
- OpenAI GPT-powered conversational responses
- Intelligent routing to specialized agents
- Customer policy support
- Billing and payment information retrieval
- Human escalation workflow
- Vector search using ChromaDB
- SQLite database integration
- Interactive conversational interface using Chainlit
- Modular architecture for future expansion

---

# Technology Stack

## Artificial Intelligence

- OpenAI GPT
- LangGraph
- Agentic AI

## Databases

- ChromaDB
- SQLite

## Data Processing

- Pandas
- NumPy
- Hugging Face Datasets

## Backend

- Python
- Chainlit

## Utilities

- python-dotenv
- tqdm

---

# Workflow

The application follows a multi-agent architecture coordinated by **LangGraph**.

1. The user submits an insurance-related question through the Chainlit interface.
2. LangGraph analyzes the request and routes it to the appropriate specialized agent.
3. The selected agent retrieves relevant information from SQLite or ChromaDB when required.
4. OpenAI GPT generates a context-aware response.
5. The final response is returned to the user while maintaining conversational context.

---

# Example Use Cases

## General Insurance Questions

The assistant answers general insurance-related questions using the LLM together with the retrieval pipeline.

<img width="1812" height="487" alt="general_insurance_question" src="https://github.com/user-attachments/assets/666b5db4-1998-41e8-a778-ce6cc1e8f3c0" />


---

## Billing Information Lookup

The Billing Agent retrieves premium information before generating a natural language response.

<img width="1827" height="412" alt="billing_query" src="https://github.com/user-attachments/assets/638b4cf0-24e7-4bba-9e83-0e2132ba1ca1" />


---

## Human Escalation

When a customer requests assistance from a human representative, the system detects the intent and routes the conversation accordingly.

<img width="1826" height="297" alt="human_escalation" src="https://github.com/user-attachments/assets/e30c3b57-accd-44cc-89ac-fd352cdf3dab" />


---

## Payment History Retrieval

The Billing Agent retrieves recent payment history and outstanding balances before generating a conversational response.

<img width="1827" height="522" alt="payment_history" src="https://github.com/user-attachments/assets/86fafb84-27f8-4cd2-bd12-3310074ddadd" />


---

# Repository Structure

```text
Multi-Agent-Insurance-System/

├── README.md
├── requirements.txt
├── .gitignore
├── LICENSE
├── multi_agent_insurance_support.ipynb
├── general_insurance_question.jpg
├── billing_query.jpg
├── human_escalation.jpg
└── payment_history.jpg
```

---

# Installation

Clone the repository.

```bash
git clone https://github.com/AShirsat96/Multi-Agent-Insurance-System.git
```

Install the required packages.

```bash
pip install -r requirements.txt
```

Create a `.env` file in the project root and add your OpenAI API key.

```text
OPENAI_API_KEY=your_openai_api_key
```

Run the notebook using Jupyter Notebook or JupyterLab.

---

# Skills Demonstrated

This project demonstrates practical experience with:

- Multi-Agent AI Systems
- Agent Orchestration using LangGraph
- Generative AI Applications
- OpenAI API Integration
- Retrieval-Augmented AI
- Vector Databases (ChromaDB)
- SQLite Database Integration
- Prompt Engineering
- Conversational AI
- Enterprise AI Workflow Design

---

# Future Improvements

- Refactor notebook into a modular Python application
- FastAPI backend
- Docker deployment
- User authentication
- AWS Bedrock integration
- Azure OpenAI integration
- Multi-language customer support
- Agent performance evaluation framework

---

# About the Author

**Aniket Shirsat**

AI Engineer | Data Scientist | Generative AI

- LinkedIn: https://www.linkedin.com/in/aniketshirsatsg/
- GitHub: https://github.com/AShirsat96
- Portfolio: https://aniketdshirsat.com

---

# License

This project is licensed under the MIT License - see the LICENSE file for details.

---

*Built with ❤️ using LangGraph, OpenAI, and ChromaDB*
