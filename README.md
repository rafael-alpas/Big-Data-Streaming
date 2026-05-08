# Big Data Streaming Pipeline: Kafka-Spark-Cassandra
Built a distributed streaming system featuring a producer-consumer architecture to process and store high-velocity data for a school requirement.

## 📌 Project Overview
This project demonstrates a real-time data engineering pipeline. It simulates a high-velocity data source (Producer) that streams messages through **Apache Kafka**, processes them via **Apache Spark Structured Streaming**, and persists the final state into an **Apache Cassandra** NoSQL database.

*Note: The source code is restricted due to MAPUA University academic integrity requirements. This repository serves as a technical showcase and documentation of the architecture.*

### 📺 Technical Walkthrough
Click the thumbnail below to watch the pipeline in action, including terminal logs showing real-time data ingestion and database persistence.

[![Big Data Pipeline Demo](https://img.youtube.com/vi/8j5vpFwmRn0wh8ST/0.jpg)](https://youtu.be/vA0sU4RtFNQ)
## 🏗️ Architecture
1. **Data Producer:** A Python-based script generating simulated high-velocity event data.
2. **Message Broker:** **Apache Kafka** manages the message queues and ensures fault-tolerant data streaming.
3. **Stream Processing:** **Apache Spark** consumes the Kafka topics, performs real-time transformations, and handles data windowing.
4. **Sink/Storage:** **Apache Cassandra** stores the processed data for low-latency querying.

## 🚀 Key Learning Outcomes
- **Distributed Systems:** Managing communication between multiple services using Docker.
- **Data Consistency:** Ensuring "exactly-once" or "at-least-once" delivery semantics within Kafka.
- **NoSQL Modeling:** Designing Cassandra tables optimized for write-heavy streaming workloads.

## 🛠️ Tech Stack
![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)
![Apache Kafka](https://img.shields.io/badge/Apache%20Kafka-000?style=for-the-badge&logo=apachekafka)
![Apache Spark](https://img.shields.io/badge/Apache%20Spark-E25A1C?style=for-the-badge&logo=apachespark&logoColor=white)
![Apache Cassandra](https://img.shields.io/badge/cassandra-%231287B1.svg?style=for-the-badge&logo=apache-cassandra&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)
