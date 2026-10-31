# LLM Evaluation Pipeline

An automated evaluation pipeline for measuring the quality and reliability of Large Language Model (LLM) applications using structured test datasets and evaluation metrics.

## Overview

This project demonstrates how to evaluate LLM-powered systems systematically rather than relying only on subjective assessments.

The pipeline evaluates generated responses against reference data and provides measurable results to help identify quality issues and compare system performance.

## Key Features

- Automated LLM response evaluation.
- Structured evaluation datasets.
- Retrieval quality measurement.
- Recall@K evaluation.
- Baseline evaluation workflow.
- Deterministic mock answer adapter.
- Reproducible evaluation results.
- Automated test suite.

## Architecture

```text
       Evaluation Dataset
               |
               v
        Evaluation Pipeline
               |
               v
       LLM / Mock Adapter
               |
               v
       Generated Responses
               |
               v
        Evaluation Metrics
               |
               v
       Evaluation Report
```

## Technology Stack

- Python
- LLM evaluation workflows
- Retrieval evaluation
- Pytest
- Structured datasets

## Project Structure

```text
llm-evaluation-pipeline/
│
├── src/
├── data/
├── evaluation/
├── tests/
├── requirements.txt
├── README.md
└── .gitignore
```

*Refer to the repository for the exact folder structure.*

## Installation

```bash
git clone https://github.com/Chanikyaa/llm-evaluation-pipeline.git
cd llm-evaluation-pipeline

python -m venv .venv
```

Activate the environment:

**Windows**
```bash
.venv\Scripts\activate
```

**Linux/macOS**
```bash
source .venv/bin/activate
```

Install dependencies:

```bash
pip install -r requirements.txt
```

## Running the Evaluation

Use the evaluation entry point provided in the project source code to execute the benchmark against the included dataset.

Check the repository's CLI help or source instructions for the exact command.

## Evaluation Metrics

- Recall@K
- Retrieval quality
- Response evaluation against reference data

## Current Validation

- Automated tests: **9 passed**.
- The included fixture achieved **Recall@3 = 1.0**.
- The evaluation uses a deterministic mock answer adapter and a limited fixture dataset.

The fixture result demonstrates that the pipeline works on the included examples. It should not be interpreted as proof of general retrieval performance.

## Limitations

- Real LLM provider benchmarking has not been completed.
- Results depend on the included evaluation dataset.
- Mock responses do not establish real-world generation quality.

## Future Improvements

- Integrate multiple LLM providers.
- Add semantic similarity and groundedness metrics.
- Build evaluation dashboards.
- Add regression testing for prompt changes.
- Benchmark larger real-world datasets.

## Author

**Palli Chanikya Paidi Balaji**

B.Tech – VIT Chennai (2025)  
M.Tech CSE – AI & Data Science, Mahindra University (2026–2028)

GitHub: [@Chanikyaa](https://github.com/Chanikyaa)

---

*Part of an AI/ML Engineering Portfolio.*
