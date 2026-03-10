# UMKC Smart Campus AI Pipeline

A production-ready data science capstone project that incorporates data ingestion, feature generation, retrieval augmentation, and AI evaluation metrics.

## Overview
This repository contains a Streamlit-based AI assistant for UMKC, powered by Snowflake and Groq LLMs. It has been hardened for production environments, featuring configuration management, automated data ingress, and structured logging.

## Core Modules
- **`app/`**: Contains the Streamlit frontend.
- **`core/`**: Centralized non-UI business logic:
    - **`features/`**: Feature store and versioning logic.
    - **`modeling/`**: AI evaluation and metric logging.
    - **`ingestion/`**: Automated CSV-to-Snowflake ingress pipeline.
    - **`config.py`**: Central YAML parameter loader.
    - **`logger.py`**: Structured Python logging utility.
- **`agent/`**: The system runner and tool definitions for the Groq LLM logic processing.

## Quick Start
1. Ensure Python 3.9+ is installed.
2. Review the detailed directions in [SETUP.md](SETUP.md).
3. Review execution commands in [RUN.md](RUN.md).

Run the application:
```bash
# Mac / Linux
bash scripts/run.sh

# Windows
scripts\run.bat
```
