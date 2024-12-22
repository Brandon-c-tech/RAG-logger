# RAG Logger

RAG Logger is an open-source logging tool designed specifically for Retrieval-Augmented Generation (RAG) applications. It serves as a lightweight, open-source alternative to LangSmith, focusing on RAG-specific logging needs.

## Features

- 📊 **Comprehensive RAG Pipeline Logging**
  - Query tracking
  - Retrieval results logging (text & images)
  - LLM interaction recording
  - Step-by-step performance monitoring

- 💾 **Structured Storage**
  - JSON-based log format
  - Daily log organization
  - Automatic file management
  - Metadata enrichment
 
## Log Structure
···json
{
    "timestamp": "2024-03-20 10:00:00",
    "query": "user query",
    "total_time": 1.23,
    "steps": {
        "retrieval": {
            "name": "retrieval",
            "start_time": 1234567890.0,
            "end_time": 1234567891.0,
            "duration": 1.0,
            "metadata": {}
        }
    },
    "retrieval_results": {
        "text": {
            "total_docs": 100,
            "retrieved_docs": [],
            "metadata": {}
        }
    },
    "llm_input": "...",
    "llm_output": "...",
    "messages": []
}
···
