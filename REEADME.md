# 🚀 PySpark Stateless Kafka Streaming

A real-time data streaming pipeline built using **PySpark Structured Streaming** and **Apache Kafka**. This project demonstrates how to consume streaming data from Kafka, process it in a **stateless manner**, and efficiently output results for downstream systems.

---

## 📌 Project Overview

This repository showcases a **stateless streaming architecture**, where each batch of incoming data is processed independently without maintaining state across batches.

### 🔹 Key Features
- Real-time data ingestion from Kafka
- Stateless transformations using PySpark
- Structured Streaming pipeline
- Scalable and fault-tolerant design
- Easy to extend for production-grade pipelines

---

## 🏗️ Architecture

Kafka Producer → Kafka Topic → PySpark Structured Streaming → Output Sink


### 🔹 Flow Explanation
1. Data is produced into a Kafka topic  
2. PySpark reads the stream using `readStream`  
3. Data is transformed (stateless processing)  
4. Results are written to output (console/file/database)

---

## ⚙️ Tech Stack

- 🐍 Python  
- ⚡ PySpark (Structured Streaming)  
- 📨 Apache Kafka  
- ☁️ Cloud Storage / Data Lake (optional)

---

## 📂 Project Structure

pyspark_stateless_kafka_streaming/
│── producer/ # Kafka producer scripts
│── consumer/ # PySpark streaming jobs
│── requirements.txt # Python dependencies
│── README.md # Project documentation


---

## 🚀 Getting Started

### 🔹 Prerequisites

Make sure you have installed:
- Python 3.x  
- Apache Spark  
- Apache Kafka  
- Java (required for Spark)

---

### 🔹 Install Dependencies

```bash
pip install -r requirements.txt

🔹 Run Producer

python producer/producer.py

🔹 Run PySpark Consumer

spark-submit consumer/streaming_job.py