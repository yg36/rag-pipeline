# Advanced RAG Pipeline

A focused RAG engineering repo that explores retrieval quality, chunking strategies, query expansion, rank fusion, hybrid search, reranking, and multimodal retrieval patterns.

This repo is stronger than a basic chatbot because it breaks RAG into individual system components and experiments with the retrieval layer directly.

## What This Covers

- Document ingestion and retrieval pipelines
- Recursive, semantic, and agentic chunking approaches
- History-aware answer generation
- Multi-query retrieval for query expansion
- Hybrid search patterns
- Reciprocal Rank Fusion for combining ranked results
- Reranking experiments
- Multimodal RAG notebook exploration

## Repository Map

```text
1_ingestion_pipeline.py
2_retrieval_pipeline.py
3_answer_generation.py
4_history_aware_generation.py
5_recursive_character_text_spliiter.py
6_semantic_chunking.py
7_agentic_chunking.py
8_multi_modal_rag.ipynb
9_retrieval_methods.py
10_multi_query_retrieval.py
11_reciprocal_rank_fusion.py
12_hybrid_search.ipynb
13_reranker.ipynb
docs/
requirements.txt
```

## System Design

```text
Documents
  -> ingestion
  -> chunking strategy
  -> embeddings/vector store
  -> retrieval method
  -> optional query expansion
  -> optional fusion/reranking
  -> answer generation
```

## Tech Stack

Python, LangChain, FAISS/Chroma-style vector retrieval, OpenAI embeddings and chat models, notebooks for retrieval experiments.

## Run Locally

1. Install dependencies:

```bash
pip install -r requirements.txt
```

2. Create a `.env` file:

```bash
cp .env.example .env
```

3. Add your API key, then run individual pipeline files or notebooks depending on the retrieval experiment.

## Recruiter Notes

This repo is directly relevant to AI/ML engineer, LLM engineer, and applied RAG roles because it shows retrieval experimentation beyond a single prompt wrapper.

## Next Improvements

- Add a small benchmark dataset and query set
- Record retrieval metrics such as hit rate, MRR, and answer faithfulness checks
- Add before/after examples for reranking and RRF
