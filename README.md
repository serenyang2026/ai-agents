# Building Agents from Scratch

This repo documents my hands-on journey learning to build AI agents — 
starting from raw Python (no frameworks) to using LangGraph, and applying 
the concepts to real-world-inspired scenarios.

## Projects
|#| Project |Concepts |Status|API Required|
|-|---------|---------|------|------------|
|1|[Unit Converter Agent](agent01_unit_converter_agent.ipynb)|Hand-built ReAct loop, regex-based action parsing|✅|open-ai-api|
|2|[Finance Assistant](agent02_finance_assistant.ipynb)|LangGraph, @tool decorator, official tool calling, bind_tools, multi-step tool chaining|✅|open-ai-api，exchange-rate-api|
|3|[IT Helpdesk RAG](rag01_it_helpdesk.ipynb)|Local embeddings (sentence-transformers, all-MiniLM-L6-v2), cosine similarity, top-k retrieval, grounded prompting with "I don't know" fallback and source citation|✅|open-ai-api|
|4|[Book Q&A RAG](rag02_courage_to_be_disliked.ipynb)|PDF text extraction (pypdf), data quality check, fixed-size chunking with overlap, page-level metadata, batch embedding, page-cited answers, data path stored in Colab Secrets|✅|open-ai-api|
