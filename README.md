# Building an Intelligent Multi-Agent Insurance Support System with LangGraph and RAG

![Multi-Agent System Architecture](https://img.shields.io/badge/AI-Multi--Agent%20System-blue) ![Python](https://img.shields.io/badge/Python-3.10%2B-green) ![LangGraph](https://img.shields.io/badge/LangGraph-Orchestration-orange)

Read full Medium Article Here: [Agentic AI Project: Build a multi-agent system with LangGraph](https://medium.com/towards-artificial-intelligence/agentic-ai-project-build-a-multi-agent-system-with-langgraph-and-open-ai-344ab768caac)

## Overview

This project walks through an end-to-end insurance support copilot that combines LangGraph, Retrieval-Augmented Generation (RAG), and structured data to resolve customer requests. The companion notebook (`multi-agent system.ipynb`) shows how to stand up the data stack, orchestrate specialized agents, and observe every hop with Phoenix tracing.

## What’s New in the Notebook

- **Phoenix-powered observability**: every agent function is wrapped with an OpenTelemetry span so you can replay decisions inside Arize Phoenix.
- **Clarification-aware supervisor**: the router uses OpenAI function calling to request missing context before delegating work.
- **Final answer agent**: conversations end with a summarizer that rewrites the last specialist message into a customer-ready response.
- **Guard rails for infinite loops**: the supervisor escalates to a human after three failed routing attempts.
- **Notebook testing**: This insurance support system demonstrates these principles in action, handling complex queries through intelligent routing, context management, and specialized processing.

The future of customer support isn't a single AI assistant—it's a **team** of specialized AI agents working together seamlessly.

---

## Contact & Resources

- **Repository**: [github.com/alphaiterations/multi-agent-system](https://github.com/alphaiterations/multi-agent-system)
- **LangGraph Docs**: [langchain-ai.github.io/langgraph](https://langchain-ai.github.io/langgraph/)
- **ChromaDB**: [docs.trychroma.com](https://docs.trychroma.com/)

---

## License

This project is open-source and available under the MIT License.

---

*Built with ❤️ using LangGraph, OpenAI, and ChromaDB*

---

## Appendix: Project Structure

```text
multi-agent-system/
├── agnetic-rag.ipynb              # RAG implementation notebook
├── multi-agent system.ipynb       # Main multi-agent system
├── requirements.txt               # Python dependencies
├── enhanced_workflow.mmd          # Mermaid workflow diagram
├── chroma_db/                     # Vector database storage
│   ├── chroma.sqlite3
│   └── 13cdf4c1-7894-4026-9ea8-46a4482514e0/
├── insurance_support.db           # SQLite database
├── insurance_agent.log            # Agent execution logs
└── README.md
