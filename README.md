
# Elasticsearch

This project explores different information retrieval strategies — `lexical`, `semantic`, `hybrid`, and `creative` — using `Elasticsearch`, applied to a fact-checking news dataset.

## PROJECT DESCRIPTION

This project was developed during an academic lab with the goal of experimenting with different search mechanisms inside and outside of `Elasticsearch`. We use a dataset from Lupa, a Brazilian fact-checking agency, containing verification texts related to news.

The main focus is to retrieve relevant analysis texts from Lupa using different search approaches.

## TASKS

### 1. Query Design

Each team received two predefined queries (`QF1` and `QF2`) and had to design two additional queries (`QP1` and `QP2`) inspired by the dataset. Queries must be written as natural language questions or statements.

## 2. Search Implementations

- `Lexical Search (BM25)` — using ElasticSearch.

- `Semantic Search` — using precomputed sentence embeddings.

- `Hybrid Search` — combining lexical and semantic results.

- `Creative Search` — a custom, team-defined strategy used in the final competition.

In addition, various data `pre-processing` techniques were tested to improve performance, and results were manually annotated with relevance scores.

### Relevance levels:

- `0`: Not Relevant
- `1`: Somewhat Relevant
- `2`: Highly Relevant

At least 10 results per query were annotated.

## 3. Evaluation with New Queries

Three new queries (`QA1, QA2, QA3`) were provided to all teams. The previously submitted code was re-executed without changes to evaluate the performance of each search method on unseen queries.

## SETUP

- Docker + Docker Compose

- Python 3.12

- Recommended: virtual environment (venv)

## TOOLS USED

- ElasticSearch (with BM25 ranking)

- Kibana (for visualization and debugging)

- Jupyter Notebook

- Sentence Embeddings (for semantic search)

## HOW TO RUN

### 1. Clone the repository

```bash
git clone https://github.com/paolamoura/elasticsearch.git
cd elasticsearch
```

### 2. Create a virtual environment

```bash
python3.12 -m venv venv
```

### 3. Activate the virtual environment

- On `Linux/macOS`:
```bash
source venv/bin/activate
```

- On `Windows`:
```bash
venv\Scripts\activate
```

### 4. Install dependencies

```bash
pip install -r requirements.txt
```

### 5. Start ElasticSearch and Kibana

```bash
docker-compose up -d
```

### 6. Start the Jupyter Notebook

```bash
jupyter notebook
```

Access the notebook via the link shown in the terminal.

