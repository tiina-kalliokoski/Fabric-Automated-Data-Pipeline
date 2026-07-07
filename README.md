## Fabric End-to-End Data Pipeline

This repository demonstrates an end-to-end Microsoft Fabric Data Engineering solution built using the Medallion Architecture. The pipeline automates data ingestion, transformation, and aggregation through Bronze, Silver, and Gold layers, orchestrated by a Microsoft Fabric Data Pipeline.

### Solution Flow

Source CSV → Bronze Load → Silver Transform → Gold Aggregations → Semantic Model Refresh

### Key Capabilities

- Microsoft Fabric Lakehouse architecture
- PySpark notebook-based data processing
- Automated pipeline orchestration
- Medallion (Bronze/Silver/Gold) data design
- Semantic Model integration and refresh
- Pipeline monitoring and operationalization
- GitHub-based project documentation

### Pipeline Parameters

The solution uses dynamic pipeline parameters to improve reusability, monitoring, and auditability across the entire data processing workflow.

### Parameters

#### Parameter | Description 

- RunTimestamp | Captures the execution timestamp of each pipeline run
- Environment | Identifies the target environment (DEV, TEST, PROD)

#### Implementation

The parameters are defined at the pipeline level and passed to all notebook activities:

- 01_Bronze_Load
- 02_Silver_Transform
- 03_Gold_Aggregations

The notebooks are designed to support both pipeline execution and standalone development execution through fallback default values.

## Some screenshots 

End-to-end pipeline
<img width="1198" height="631" alt="end-to-end-pipeline" src="https://github.com/user-attachments/assets/facd9803-56fa-4fdd-9b2c-33080fbf5f84" />

Monitoring Hub
<img width="1642" height="875" alt="monitoring" src="https://github.com/user-attachments/assets/5255256b-8f65-4c2b-b45d-4a64fb9df894" />


This project was created to demonstrate practical Data Engineering skills, Data Factory orchestration, and Microsoft Fabric best practices while preparing for the DP-700: Fabric Data Engineer Associate certification.
