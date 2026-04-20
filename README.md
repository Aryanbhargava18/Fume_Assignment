# Fume Pipeline Assignment

This repository contains my submission for the Fume parsing and data extraction assignment. It includes an automated pipeline for conversation transcription analysis, LLM-based data extraction, and a dynamic frontend dashboard for visualizing client metrics.

## Architecture

- **`pipeline/`**: The core python backend pipeline. Handles reading transcripts, chunking, parsing speaker turns, and calling the LLM extraction logic.
- **`docs/`**: A frontend web dashboard built with HTML, CSS (dark mode/glassmorphism), and vanilla JS to visualize the output of the pipeline (Client risk, metrics, etc.).
- **`scripts/`**: Auditing and verification scripts to ensure schema validation and hallucination-free outputs.

## Getting Started

1. Install dependencies:
   ```bash
   pip install -r pipeline/requirements.txt
   ```
2. Run the extraction pipeline:
   ```bash
   python pipeline/run_pipeline.py
   ```
3. Run audits to verify the generated data:
   ```bash
   python scripts/audit.py
   ```
4. To view the dashboard, open `docs/index.html` in your browser.

## Documentation

Full architectural specifications, schema requirements, and hallucination scenarios can be found in the `docs_zip/` folder.
