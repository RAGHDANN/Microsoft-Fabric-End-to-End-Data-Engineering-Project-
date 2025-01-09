# Microsoft Fabric News Analytics Project

## Project Overview
This project implements an end-to-end data engineering solution using Microsoft Fabric to create a news analytics platform. The solution ingests news data from Bing News API, processes it using PySpark, performs sentiment analysis, and visualizes the results in a Power BI dashboard.

![Recording 2025-01-09 184142](https://github.com/user-attachments/assets/7c0e0bb2-b09a-447f-a4a4-214dda9e2c93)


## Architecture
The project utilizes several components within the Microsoft Fabric ecosystem:

1. **Data Ingestion**
   - Source: Bing News API
   - Tool: Data Factory (Microsoft Fabric)
   - Output: Raw JSON files in Lake Database

2. **Data Processing**
   - Tool: Synapse Data Engineering
   - Technology: PySpark
   - Process: JSON transformation to Delta tables
   - Features: Implements incremental load pattern

3. **Machine Learning**
   - Tool: Synapse Data Science
   - Technology: PySpark
   - Process: Sentiment analysis on news content
   - Model: Text Analytics pre-trained model

4. **Data Visualization**
   - Tool: Power BI
   - Output: Interactive news dashboard
   - Features: Real-time news monitoring

## Prerequisites
- Microsoft Fabric workspace
- Azure subscription
- Bing News API key
- Basic understanding of:
  - Data Engineering concepts
  - PySpark
  - Power BI
  - Delta Lake

## Project Structure
```
├── data_factory/
│   └── pipelines/
├── synapse/
│   ├── data_engineering/
│   │   └── pyspark_notebooks/
│   └── data_science/
│       └── sentiment_analysis_notebooks/
├── powerbi/
│   └── dashboards/
└── docs/
    └── images/
```

## Setup Instructions

### 1. Environment Setup
1. Configure Microsoft Fabric workspace
2. Set up Bing News API access
3. Create necessary Lake Database

### 2. Data Pipeline Configuration
1. Configure Data Factory connections
2. Import PySpark transformation notebooks
3. Configure incremental load parameters

### 3. Power BI Dashboard Setup
1. Import the provided Power BI template
2. Configure data source connections
3. Customize visualizations as needed

## Features
- Real-time news data ingestion
- Automated PySpark transformation pipeline
- PySpark-based sentiment analysis
- Interactive Power BI dashboard
- Incremental data load pattern
- End-to-end orchestration

## Technical Details

### Data Flow
1. Bing News API → Raw JSON files
2. JSON files → PySpark transformation → Structured Delta tables
3. Delta tables → PySpark sentiment analysis
4. Analyzed data → Power BI dashboard

### Technologies Used
- Microsoft Fabric
- Data Factory
- Synapse Data Engineering
- Synapse Data Science
- PySpark
- Delta Lake
- Power BI

## Contributing
Feel free to fork this repository and submit pull requests. For major changes, please open an issue first to discuss the proposed changes.

## License
[MIT](https://choosealicense.com/licenses/mit/)

## Acknowledgments
- Based on the tutorial by [Original Author Name]
- Microsoft Fabric documentation
- Bing News API documentation

## Contact
Your Name - [Your Email]

Project Link: [Your GitHub Repository URL]
