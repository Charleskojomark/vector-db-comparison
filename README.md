# Embeddings & Vector Database Comparison

This project demonstrates generating text embeddings using Hugging Face sentence-transformers and storing/querying them in vector databases: Milvus (local), Weaviate (local), and Pinecone (cloud, optional). It includes benchmarking indexing speed, query latency, and retrieval relevance.

## Project Structure

```

lab3-vector-db-comparison/
├── data/                 # Sample text corpus
├── embeddings/           # Saved embeddings
├── notebooks/            # Jupyter notebooks
├── src/                  # Python scripts
├── requirements.txt      # Dependencies
└── report.pdf            # Final lab report

````

## Setup

1. Create and activate a virtual environment:

```bash
python3 -m venv venv
source venv/bin/activate   # Windows: venv\Scripts\activate
````

2. Install dependencies:

```bash
pip install -r requirements.txt
```

3. (Optional) Start local Weaviate with Docker:

```bash
docker run -p 8080:8080 semitechnologies/weaviate
```

---

## Usage

1. Generate embeddings in `notebooks/01_generate_embeddings.ipynb`.
2. Insert embeddings into Milvus, Weaviate, or Pinecone.
3. Run queries and benchmark retrieval performance.
4. Record results and create the final report in `report.pdf`.

---

## Dependencies

* sentence-transformers
* torch
* numpy
* pandas
* scikit-learn
* matplotlib
* tqdm
* jupyter
* ipykernel
* pinecone
* weaviate-client
* pymilvus[milvus-lite]

