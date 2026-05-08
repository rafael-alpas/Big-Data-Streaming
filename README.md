# Big Data Streaming Pipeline: Kafka-Spark-Cassandra
Built a distributed streaming system featuring a producer-consumer architecture to process and store high-velocity data for a school requirement.

## 📌 Project Overview
This project demonstrates a real-time data engineering pipeline. It simulates a high-velocity data source (Producer) that streams messages through **Apache Kafka**, processes them via **Apache Spark Structured Streaming**, and persists the final state into an **Apache Cassandra** NoSQL database.

***Note:*** *This repository serves as a technical showcase and documentation of the architecture. The source code is passed as a major project at MAPUA University*

### 📺 Project Demo
> **[Click here to watch the demo on YouTube](https://youtu.be/vA0sU4RtFNQ)**

## 🏗️ Architecture
1. **Multi-Instance Producers:** Orchestrated ten simultaneous Python-based sensor scripts (sensor_01 through sensor_10) to generate high-velocity, JSON-formatted traffic event data.
2. **Distributed Message Broker:** Apache Kafka (orchestrated via Zookeeper) acts as the central bus, managing a dedicated topic (css182-grp-06) to decouple data generation from downstream consumption.
3. **Stream Processing:** Apache Spark Structured Streaming (via spark-shell) consumes the Kafka topics in real-time, handling data transformations and batch windowing.
4. **NoSQL Persistence:** Apache Cassandra serves as the storage sink. Data is persisted into a dedicated keyspace (p1_keyspace) and table (prod_storage) using an integration script that executes optimized Prepared Statements.

## 🚀 Key Learning Outcomes
- **Distributed System Orchestration:** Gained hands-on experience initializing and managing Zookeeper and Kafka brokers within a Linux environment to handle asynchronous data streams.
- **Real-Time Data Ingestion:** Successfully implemented a multi-producer architecture to simulate real-world data spikes, managing ten concurrent data streams into a single broker.
- **Structured Streaming & Transformations:** Developed proficiency in Spark SQL and DataFrames to process live Kafka streams, utilizing .readStream() and .writeStream() for real-time output.
- **NoSQL Schema Design:** Designed and managed Cassandra keyspaces using CQLSH, implementing specific Replication Factors and partition keys to ensure data availability and fault tolerance.
- **System Integration:** Built a robust data bridge between Kafka and Cassandra, mastering JSON deserialization and automated persistence for write-heavy streaming workloads.

## 🛠️ Tech Stack
![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)
![Apache Kafka](https://img.shields.io/badge/Apache%20Kafka-000?style=for-the-badge&logo=apachekafka)
![Apache Spark](https://img.shields.io/badge/Apache%20Spark-E25A1C?style=for-the-badge&logo=apachespark&logoColor=white)
![Apache Cassandra](https://img.shields.io/badge/cassandra-%231287B1.svg?style=for-the-badge&logo=apache-cassandra&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)
