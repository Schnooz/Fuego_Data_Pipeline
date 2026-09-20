# News Pulse Data Pipeline

Data preprocessing pipeline for the SteelHacks 2026 project participating in Xtract and Nemotron tracks. 

## Overview

This notebook retrieves news article metadata from the GDELT Global Knowledge Graph
and prepares article data for downstream analysis and LLM processing.

The pipeline:

1. Queries GDELT data using Google BigQuery
2. Filters articles by geographic location and publication date
3. Extracts article titles and metadata
4. Uses Trafilatura to retrieve and extract main article text
5. Filters out articles that cannot be successfully extracted or contain fewer than 300 words
6. Removes duplicate articles
7. Filters the dataset to English-language articles
8. Splits the resulting dataset by publication date
9. Exports daily datasets as JSON

## Technologies

- Python
- Pandas
- Google BigQuery
- GDELT
- Trafilatura

## Project

Developed as part of SteelHacks 2026.

## AI Assistance

ChatGPT (OpenAI) was used as a coding assistant during development, primarily
for debugging, explaining Python/Pandas concepts, and refining data-processing
functions.
