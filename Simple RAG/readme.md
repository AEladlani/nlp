# Local LLM + RAG Example

This project demonstrates how to use local large language models (LLMs) with Retrieval-Augmented Generation (RAG) to answer questions from PDF documents. The workflow allows for precise, controlled answers, suitable for research or document analysis.

PDF Source

Document: Sample Research Report

URL: Sample Research Report PDF

Description: A research report containing multiple sections of structured text, which can be queried using RAG.

# 1️⃣ Local DeepSeek Model

Model: DeepSeek-R1-Distill-Llama-8B-Q4_0.gguf

Usage: Loaded locally in the notebook to generate text completions.

RAG Integration: Text is split into chunks, embedded using a semantic embedding model, and indexed with FAISS. Queries retrieve the most relevant chunks, which are then passed to the LLM for accurate answers.

Output Control: The model can be prompted to output highly structured answers, such as only the exact names, dates, or lists, without unnecessary explanation.

# 2️⃣ HuggingFace Qwen Model (Torch-based)

Model: Qwen/Qwen2.5-3B-Instruct

Features: GPU-compatible, supports 4-bit quantization for faster inference with reduced memory footprint.

RAG Workflow: Similar to DeepSeek, but using the HuggingFace Transformers framework for tokenization, embedding, and LLM inference.

Use Case: Ideal for notebooks with GPU access where faster responses are desired, while still providing structured outputs.

# 3️⃣ Retrieval-Augmented Generation (RAG) Workflow

Text Extraction: Load and extract text from PDF pages.

Text Chunking: Split text into semantically meaningful chunks while respecting sentence boundaries.

Embedding: Encode chunks using a sentence transformer for semantic similarity.

Indexing: Store embeddings in a FAISS vector index to enable fast retrieval.

Querying: Retrieve top relevant chunks for a user query.

LLM Completion: Feed retrieved context into the LLM to generate controlled, accurate answers.

# 4️⃣ Key Benefits

Works completely offline with local LLMs.

RAG ensures accurate, context-based answers from large documents.

Supports structured output, like Python lists, dictionaries, names, dates, or other controlled formats.

Can use either CPU or GPU, with Torch models leveraging quantization for efficiency.

Fully reproducible workflow for research, document analysis, or educational purposes.
