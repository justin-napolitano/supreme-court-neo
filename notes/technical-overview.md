---
slug: github-supreme-court-neo-note-technical-overview
id: github-supreme-court-neo-note-technical-overview
title: supreme-court-neo
repo: justin-napolitano/supreme-court-neo
githubUrl: https://github.com/justin-napolitano/supreme-court-neo
generatedAt: '2025-11-24T18:47:33.924Z'
source: github-auto
summary: >-
  This repository provides a Python project that integrates a Neo4j graph
  database with a Flask REST API. It allows you to manage graph data with
  features like node creation, querying, and CSV/GraphML imports.
tags: []
seoPrimaryKeyword: ''
seoSecondaryKeywords: []
seoOptimized: false
topicFamily: null
topicFamilyConfidence: null
kind: note
entryLayout: note
showInProjects: false
showInNotes: true
showInWriting: false
showInLogs: false
---

This repository provides a Python project that integrates a Neo4j graph database with a Flask REST API. It allows you to manage graph data with features like node creation, querying, and CSV/GraphML imports.

## Key Features
- Flask-based REST API for Neo4j.
- Utilities for data ingestion from CSV and GraphML.
- Data models defined with Neomodel.
- Docker Compose setup for easier local development.

## Quick Start

### Prerequisites
- Docker & Docker Compose.
- Python 3.

### Installation
Clone the repo and navigate to the directory:

```bash
git clone https://github.com/justin-napolitano/supreme-court-neo.git
cd supreme-court-neo/neo4jAPI
```

Install dependencies:

```bash
pip install -r requirements.txt
```

### Running the App
Start everything up with:

```bash
docker-compose -f docker-compose.dev.yml up --build
```

The API will be live at `http://localhost:5000`.

## Gotchas
- Placeholder credentials should be secured for production.
