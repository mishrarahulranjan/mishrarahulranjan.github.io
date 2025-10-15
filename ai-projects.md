---
layout: default
title: AI & Machine Learning Projects
permalink: /ai-projects/
description: A portfolio of practical AI/ML projects focusing on finance, e-commerce, and software architecture applications.
---

# 🤖 AI & Machine Learning Portfolio

This page showcases projects where I have applied my expertise in software architecture and data engineering to build production-grade AI and Machine Learning solutions. 
The focus is on **impact**, **scalability**, and **responsible deployment**.

## Featured Project 1: Real-Time Fraud Detection System (Finance)

### **Stack & Technologies**
* **Core ML:** Isolation Forest, One-Class SVM
* **Data Pipeline:** Apache Kafka (Event Sourcing), Kafka Streams/KSQL
* **Serving:** Python (Flask/FastAPI), Java API, Kubernetes
* **Data Store:** Redis (Feature Store)

### **Overview**
Designed and implemented a low-latency fraud detection pipeline to score millions of financial transactions per day. The system operates entirely on a streaming architecture, enabling sub-millisecond decision-making.

### **Key Contributions**
* **Architecture:** Migrated from a nightly batch process to a **real-time event-driven architecture (EDA)**, reducing fraud exposure time from 24 hours to under 500ms.
* **MLOps:** Developed a repeatable CI/CD pipeline for model training, versioning (MLflow), and A/B testing in a production Kubernetes environment.
* **Resilience:** Implemented backpressure handling and failover strategies in Kafka to ensure zero data loss during peak trading volumes.

## Featured Project 2: Personalized Product Recommendation Engine (E-commerce)

### **Stack & Technologies**
* **Core ML:** Collaborative Filtering (ALS), Deep Learning (TensorFlow Recommenders)
* **Data Pipeline:** Spark (ETL/Model Training), Delta Lake
* **Serving:** Go microservice, gRPC API
* **Cloud:** Google Cloud Platform (GCP - Vertex AI, Cloud Storage)

### **Overview**
Built a recommendation service that provides personalized product suggestions across the e-commerce platform (homepage, product pages, cart). The model updates daily based on user behavior, inventory changes, and sales data.

### **Key Contributions**
* **Scalability:** Implemented a **vector database** to handle billions of embedding lookups, ensuring high throughput for the API under heavy load.
* **Data Governance:** Established a clean, versioned **Feature Store** (using Delta Lake) to ensure consistency between training and serving data, mitigating data drift.
* **Performance:** The serving microservice was written in Go to maintain extremely low latency (P95 < 20ms) under a high volume of requests.

## Ongoing Initiatives & Research

| Initiative | Objective | Current Status | Technologies |
| :--- | :--- | :--- | :--- |
| **LLM RAG Integration** | Securely grounding internal Large Language Models with private enterprise data. | Active Development | Spring AI, PostgreSQL/pgvector, Azure OpenAI |
| **Code Structure to Markdown** | Automating project documentation and context generation for AI coding assistants. | Proof-of-Concept (POC) | Python, GitHub Copilot Instructions, Markdown |
| **Time Series Forecasting** | Predicting server load and resource usage for automated capacity planning. | In Testing | Prophet, ARIMA, Prometheus Metrics |

***

### Technologies and Concepts

I believe in building AI systems that are not just accurate, but **maintainable, auditable, and scalable**. My work heavily leverages:

* **MLOps Tools:** MLflow, Kubeflow, Prometheus, Grafana
* **Architecture Patterns:** Event-Driven Architecture (EDA), Microservices, Feature Stores
