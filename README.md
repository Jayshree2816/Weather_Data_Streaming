# Weather_Data_Streaming

In this project, we leverage Azure Event Hub and Databricks to build a real-time weather data streaming pipeline. The solution ingests high-frequency data from IoT sensors, including temperature, humidity, and wind speed, into Azure Event Hub. From there, Databricks processes and analyzes the streaming data to derive meaningful insights, such as weather trends, anomaly detection, and forecasting.

This project showcases the power of cloud-based data engineering by integrating scalable event-driven architectures with big data analytics. The processed insights are visualized using interactive dashboards, enabling data-driven decision-making for weather monitoring and forecasting applications.

This process involves:
	•	Fetching real-time weather data from a public API.
	•	Storing the raw data in Azure Data Lake.
	•	Processing and analyzing the data using Databricks.
	•	Streaming data into Azure Event Hub for further processing.

## Architecture
- **Weather API**: Fetches real-time weather data.
- **Databricks**: Processes and transforms the data.
- **Azure Data Lake**: Stores raw weather data.
- **Azure Event Hub**: Streams processed data for real-time analytics.


### 1. Set Up Databricks
- Create a Databricks workspace on Azure.
- Install necessary libraries:
  ```python
  %pip install requests azure-eventhub pyspark