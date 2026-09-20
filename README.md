# Fuego_Data_Pipeline

Data preprocessing pipeline for the SteelHacks 2026 project participating in Xtract and Nemotron tracks. 

## Overview

This notebook retrieves news article metadata from the GDELT Global Knowledge Graph
and prepares article data for downstream analysis and LLM processing.

The pipeline:

1. Queries GDELT data using BigQuery
2. Filters articles by geographic location and publication date
3. Extracts article titles and metadata
4. Uses Trafilatura to retrieve and extract main article text
5. Filters articles based on successful extraction and minimum word count
6. Splits the resulting dataset by publication date
7. Exports daily datasets as JSON

## Technologies

- Python
- Pandas
- Google BigQuery
- GDELT
- Trafilatura

## Project

Developed as part of SteelHacks 2026.
