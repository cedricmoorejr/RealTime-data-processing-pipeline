# Stock Data Real-Time

Stock Data Real-Time is a project that performs real-time analysis of stock market data using Apache Kafka, Apache Spark, PostgreSQL, and RShiny. The project streams stock market data from various sources, such as financial APIs or data providers, through Apache Kafka. It then applies machine learning-based analysis using Spark MLlib to extract valuable insights and patterns from the streaming data. The processed data is stored in a PostgreSQL database for further querying, analysis, and integration with other systems. Additionally, it provides a mechanism to notify an RShiny application to update the visualization.

## Table of Contents

- [Description](#description)
- [Overview](#overview)
- [Prerequisites](#prerequisites)
- [Getting Started](#getting-started)
  - [Installation](#installation)
  - [Kafka Configuration](#kafka-configuration)
  - [PostgreSQL Configuration](#postgresql-configuration)
  - [RShiny Configuration](#rshiny-configuration)
  - [Spark Configuration](#spark-configuration)
- [Usage](#usage)
- [Contact](#contact)
- [License](#license)

## Description

The Stock Data Real-Time project aims to provide a comprehensive solution for real-time stock market analysis, enabling users to gain deeper insights and make informed decisions in the fast-paced financial markets. By leveraging the power of Apache Kafka, the project ensures the seamless and efficient ingestion of stock market data from multiple sources. This includes real-time market prices, trade volumes, news sentiment scores, and other relevant metrics.

Apache Spark and Spark MLlib are utilized to perform advanced analysis and modeling on the streaming data. With Spark's powerful distributed computing capabilities, the project can handle large-scale datasets and perform complex calculations in real-time. The machine learning algorithms in MLlib enable the identification of patterns, trends, and anomalies in the stock market data, providing valuable predictions and forecasts.

The processed data is stored in a PostgreSQL database, which serves as a centralized repository for historical and real-time stock market information. This enables users to query the data, generate custom reports, and perform further analysis using SQL or other data analytics tools. The PostgreSQL database also facilitates seamless integration with other systems, such as business intelligence platforms or custom applications.

To enhance the user experience and enable intuitive visualization of real-time stock market trends, Stock Data Real-Time integrates with an RShiny application. RShiny provides a dynamic and interactive interface to explore the streaming data through various visualizations, including line plots, bar charts, candlestick charts, and heatmaps. Users can customize the visualizations, apply filters, and interactively analyze the stock market data to gain valuable insights.

The Stock Data Real-Time project is highly configurable and can be adapted to different stock markets, asset classes, or specific data requirements. It provides a solid foundation for building real-time financial analytics applications, algorithmic trading systems, or data-driven investment platforms.


## Overview

The project performs the following steps:
1. Consume stock market data from a Kafka topic.
2. Create a streaming DataFrame from Kafka using Apache Spark.
3. Perform real-time analysis on the streaming data using Spark MLlib.
4. Store the analyzed data in PostgreSQL.
5. Notify an RShiny application to update the visualization.

## Prerequisites

Before running the project, make sure you have the following software installed:

- Java Development Kit (JDK) version X or higher: [Download JDK](https://www.oracle.com/java/technologies/javase-jdkX-downloads.html)
- Apache Kafka version X or higher: [Download Kafka](https://kafka.apache.org/downloads)
- Apache Spark version X or higher: [Download Spark](https://spark.apache.org/downloads.html)
- PostgreSQL database: [Download PostgreSQL](https://www.postgresql.org/download/)
- R and required packages: `shiny`, `DBI`, `ggplot2`

## Getting Started

To get started with the project, follow these steps:

### Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/your-username/stock-data-realtime.git
   ```

2. Update the project configuration:

   - Open the `RealTimeStockMarketAnalysis.java` file.
   - Modify the Kafka configuration, PostgreSQL configuration, and RShiny configuration according to your environment. Update the variables `bootstrapServers`, `topic`, `dbHost`, `dbPort`, `dbName`, `dbUser`, `dbPassword`, `rshinyHost`, and `rshinyPort` with your specific values.

3. Build the project:

   - Open a terminal.
   - Navigate to the project directory.
   - Build the project using Gradle or your preferred

 build tool:

     ```bash
     gradle build
     ```

4. Start Kafka, Spark, and PostgreSQL:

   - Follow the respective documentation to start Kafka, Spark, and PostgreSQL in your environment.


### Kafka Configuration

- Set the `bootstrapServers` variable to the Kafka bootstrap servers' address.
- Set the `topic` variable to the desired Kafka topic name.

### PostgreSQL Configuration

- Set the `dbHost`, `dbPort`, `dbName`, `dbUser`, and `dbPassword` variables according to your PostgreSQL database configuration.

### RShiny Configuration

- Set the `rshinyHost` variable to the RShiny application's host address.
- Set the `rshinyPort` variable to the RShiny application's port number.

### Spark Configuration

- Configure SparkSession settings as needed in the `main` method.

## Usage

1. Start Apache Kafka and create a Kafka topic.
2. Start PostgreSQL and create a database.
3. Run the `RealTimeStockMarketAnalysis` class in the project.
4. Launch the RShiny application to visualize the stock market data.

## Contact

For any inquiries or questions, please contact [cedricmoorejunior](mailto:Cedric.MooreJr@outlook.com).

## License

This project is licensed under the [MIT License](LICENSE.txt).


