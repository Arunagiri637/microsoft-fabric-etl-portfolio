# Microsoft Fabric ETL Pipeline for eCommerce

## Overview
End-to-end ETL project in Microsoft Fabric: Ingests eCommerce CSV data, stores in Lakehouse, transforms/validates with PySpark Notebooks, orchestrates via Pipelines, and serves insights in Power BI.

## Assets Included
- **Data**: Original CSV + exported Lakehouse tables (CSV).
- **Dataflow Gen2**: Ingestion logic (.flow JSON).
- **Notebooks**: Transformation and validation (PySpark .ipynb).
- **Pipeline**: Orchestration (.json).
- **Screenshots**: Visual proof of runs and dashboards.

## How to Replicate
1. Create a Fabric workspace with capacity.
2. Import .flow, .ipynb, .json assets.
3. Upload data.csv to Dataflow > Run Pipeline.
4. Open .pbix in Power BI Desktop.

## Architecture
![Diagram](./docs/architecture.png)

## Screenshots
![Pipeline Run](./screenshots/pipeline-run.png)
![Dashboard](./screenshots/powerbi-dashboard.png)

## Tech Stack
- Ingestion: Dataflows Gen2 + On-Premises Gateway
- Storage: Lakehouse (Delta tables)
- Transformation: PySpark Notebooks
- Orchestration: Pipelines
- Serving: Power BI

## Learnings
- Handled local file ingestion securely.
- Ensured data quality with assertions.
- Built for scalability in Fabric capacity.

Dataset source: Kaggle eCommerce sample.
