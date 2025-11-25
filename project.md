---
slug: github-supreme-court-neo
id: github-supreme-court-neo
title: Integrating Neo4j with Flask for Graph Data Management
repo: justin-napolitano/supreme-court-neo
githubUrl: https://github.com/justin-napolitano/supreme-court-neo
generatedAt: '2025-11-24T21:36:32.824Z'
source: github-auto
summary: >-
  Explore a Python project that combines Neo4j with Flask for managing graph data through a REST API
  and data ingestion pipelines.
tags:
  - flask
  - neo4j
  - docker
  - pyspark
  - neomodel
  - rest api
  - data ingestion
seoPrimaryKeyword: flask neo4j integration
seoSecondaryKeywords:
  - python graph database
  - docker compose setup
  - neo4j data models
  - csv data ingestion
  - flask rest api
  - data pipeline automation
seoOptimized: true
topicFamily: datascience
topicFamilyConfidence: 0.9
kind: project
entryLayout: project
showInProjects: true
showInNotes: false
showInWriting: false
showInLogs: false
---

A Python-based project integrating Neo4j graph database functionalities with Flask REST API endpoints and data ingestion pipelines. It provides tools for managing graph data, including node creation, querying, and CSV/GraphML data uploads.

---

## Features

- REST API server built with Flask for Neo4j interactions.
- Neo4j connection and query management classes.
- Data ingestion utilities for CSV and GraphML files into Neo4j.
- Neo4j data models defined using Neomodel.
- Docker Compose setup for local development with Neo4j and Flask.

## Tech Stack

- Python 3
- Flask
- Neo4j (Graph Database)
- Neomodel (Object Graph Mapper for Neo4j)
- Docker & Docker Compose
- PySpark (for some data processing)

## Getting Started

### Prerequisites

- Docker and Docker Compose installed
- Python 3 environment

### Installation

Clone the repository:

```bash
git clone https://github.com/justin-napolitano/supreme-court-neo.git
cd supreme-court-neo/neo4jAPI
```

Install Python dependencies (assuming a virtual environment):

```bash
pip install -r requirements.txt
```

### Running the Application

To start the Flask REST API and Neo4j database using Docker Compose:

```bash
docker-compose -f docker-compose.dev.yml up --build
```

The Flask app will be available at `http://localhost:5000`.

### Usage

- Access the root endpoint `/` for a basic health check.
- Use `/init_neo_driver` to initialize the Neo4j driver and run a test query.

## Project Structure

```
neo4jAPI/
├── rest.py               # Flask REST API server
├── neo4j_connect.py      # Neo4j connection and query wrapper
├── neo_native_apy.py     # Neo4j driver wrapper with sample queries
├── NeoNodes.py           # Neomodel node definitions
├── docker-compose.dev.yml# Docker Compose config for dev
├── clean_loc_data.py     # Utility for file listing
├── upload_csv_to_neo.py  # Data ingestion pipeline for CSV
├── csv_to_neo.py         # CSV data upload functions
├── graphml_to_neo.py     # GraphML import utility
├── neo4j_connect_2.py    # Alternative Neo4j connection class
├── neo4jClasses.py       # Neo4j Aura and Sandbox API classes
├── neoModelAPI.py        # Neomodel API wrapper
├── stack_graph.py        # Cypher queries and graph processing logic
└── test_data/            # Sample test data
```

## Future Work / Roadmap

- Add comprehensive documentation and usage examples.
- Implement more robust error handling and logging.
- Extend REST API with additional endpoints for CRUD operations on graph nodes.
- Integrate authentication and security for API access.
- Automate data pipeline workflows for scalable ingestion.
- Add unit and integration tests.

---

*Note: Some credentials and connection details are placeholders or hardcoded for development and should be secured or parameterized for production.*


