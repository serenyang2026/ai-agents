# Building Agents from Scratch

This repo documents my hands-on journey learning to build AI agents — 
starting from raw Python (no frameworks) to using LangGraph, and applying 
the concepts to real-world-inspired scenarios.

## Projects
|#| Project |Concepts |Status|API Required|
|-|---------|---------|------|------------|
|1|[Unit Converter Agent](agent01_unit_converter_agent.ipynb)|Hand-built ReAct loop, regex-based action parsing|✅|open-ai-api|
|2|[Finance Assistant](agent02_finance_assistant.ipynb)|LangGraph, @tool decorator, official tool calling, bind_tools, multi-step tool chaining|✅|open-ai-api，exchange-rate-api|
|3|[IT Helpdesk RAG](agent03_rag01_it_helpdesk.ipynb)|Local embeddings (sentence-transformers, all-MiniLM-L6-v2), cosine similarity, top-k retrieval, grounded prompting with "I don't know" fallback and source citation|✅|open-ai-api|
|4|[Book Q&A RAG](agent04_rag02_courage_to_be_disliked.ipynb)|PDF text extraction (pypdf), data quality check, fixed-size chunking with overlap, page-level metadata, batch embedding, page-cited answers, data path stored in Colab Secrets|✅|open-ai-api|
| 5 | [Finance Assistant with Self-Reflection](agent05_finance_assistant_reflection.ipynb) | Self-reflection pattern: generator–reviewer loop in LangGraph, reflector node with structured output (Pydantic), conditional routing on review verdict, max-revision cap, reviewer feedback injected back as a message | ✅ | open-ai-api, exchange-rate-api |
| 6 | [Language Learning Multi-Agent](agent06_language_practicing_multi-agent.ipynb) | Supervisor pattern (hierarchical delegation), routing via structured output with `Literal`, conditional edges, 4 specialist agents built from one prompt-template factory, runtime-configurable target language / explanation language / level (Colab form), scoped context per agent, short-term memory with checkpointer + thread_id, filtering thinking blocks from responses | ✅ | anthropic-api |
