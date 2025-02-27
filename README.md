# Stock Market Analyser: End-to-End Pipeline

## Overview
This project is a real-time stock market data analysis pipeline using Apache Kafka, AWS services, and Python. It collects, processes, and analyzes stock market data to provide real-time insights.

## Tech Stack
- **Apache Kafka**: Real-time data streaming
- **AWS Glue (Crawler & Catalog)**: Data transformation and cataloging
- **AWS Athena**: SQL-based querying and analytics
- **Python**: Data processing and analysis
- **SQL**: Querying stock data for insights

## Architecture
1. **Data Ingestion**:
   - Stock market data is streamed in real-time using Apache Kafka.
   - Producers publish data to Kafka topics.
   
2. **Data Processing & Storage**:
   - Data is stored in AWS S3.
   - AWS Glue Crawler scans and catalogs data.

3. **Data Analysis**:
   - AWS Athena is used for querying structured data using SQL.
   - Python is used for additional data processing and visualization.

4. **Insights & Reporting**:
   - Processed data is used to generate insights into stock trends and movements.

## Installation & Setup
### Prerequisites:
- AWS Account with S3, Glue, and Athena access
- Apache Kafka installed and running
- Python (3.x) with necessary dependencies

### Steps:
1. **Set up Kafka**:
   - Install and start Kafka.
   - Create required topics for stock data.
   
2. **Run Kafka Producer**:
   - Write a producer script to fetch real-time stock data and publish to Kafka.
   
3. **Consume Data & Store in AWS S3**:
   - Create a Kafka consumer to consume and store data in S3.

4. **AWS Glue Crawler Setup**:
   - Configure Glue to crawl S3 bucket and create a table in AWS Glue Catalog.

5. **Query with Athena**:
   - Use Athena to analyze stock data using SQL.

6. **Process and Visualize with Python**:
   - Fetch queried data.
   - Use Pandas/Matplotlib for analysis and visualization.

## Usage
- Run the Kafka producer to start streaming data.
- Use AWS services to store and process the data.
- Query data in Athena and analyze it with Python.
- Generate insights and visualize trends.

## Future Enhancements
- Implement machine learning models for stock price prediction.
- Add alert mechanisms for significant market movements.
- Optimize real-time analytics for better performance.

## Author
Anmol Upadhyay

## License
This project is licensed under the MIT Open License.

