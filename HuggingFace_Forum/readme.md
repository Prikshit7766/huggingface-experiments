# Semantic Search with FAISS

This document provides a brief overview of preparing a dataset by scraping data from the Hugging Face forum and implementing semantic search using FAISS.

## 1. Dataset Preparation (`prepare_dataset.ipynb`)

This notebook focuses on:
- **Web Scraping**: Scraping discussion posts, replies, and metadata from different categories on the Hugging Face forum.
- **Data Storage**: Saving the scraped data into JSON files for further processing.

## 2. Semantic Search with FAISS (`Semantic_Search_FAISS.ipynb`)

Using the prepared dataset, this notebook implements:
- **Data Loading**: Loading the pre-scraped JSON dataset.
- **Embedding Generation**: Creating embeddings for forum posts using a model from `SentenceTransformer` or Hugging Face.
- **FAISS Indexing**: Indexing embeddings in FAISS for fast similarity-based searches.
- **Querying**: Executing a semantic search by converting a query to an embedding and retrieving the most similar entries.

---