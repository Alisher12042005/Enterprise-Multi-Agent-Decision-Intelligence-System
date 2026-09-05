# Enterprise Decision Intelligence System

An API-first Decision Intelligence platform that leverages machine learning models and data processing pipelines to deliver automated predictive analytics for enterprise datasets.

📌 Project Overview
The Enterprise Decision Intelligence System processes raw enterprise and financial datasets to generate predictive insights for investment and operational decision-making.

Built using a modular microservices architecture, the platform provides:
- Real-time machine learning model inference
- RESTful APIs for prediction services
- Scalable asynchronous batch processing
- Interactive data visualization dashboards
- Containerized development and deployment

💡 Key Features

🔮 Predictive Analytics
Implements multiple machine learning approaches to analyze enterprise data and forecast outcomes:
- Decision Trees & Random Forests
- Scikit-Learn-based ML pipelines
- Neural Networks (PyTorch)

⚡ RESTful API Backend
High-performance asynchronous APIs built with FastAPI for low-latency model inference and data processing.

🔄 Asynchronous Processing
Uses Celery and Redis to handle background jobs and large-scale batch prediction workloads without blocking API requests.

📊 Interactive Dashboard
A modern web dashboard built with Next.js, React, and Tailwind CSS for data ingestion, prediction monitoring, and decision-support insights.

🐳 Containerized Deployment
Uses Docker Compose to provide reproducible development and deployment environments with support for scalable cloud infrastructure.

🏗️ System Architecture

                    ┌──────────────────────┐
                    │    Next.js Dashboard │
                    │   React + Tailwind   │
                    └──────────┬───────────┘
                               │
                               ▼
                    ┌──────────────────────┐
                    │      FastAPI API     │
                    │   RESTful Endpoints  │
                    └──────────┬───────────┘
                               │
              ┌────────────────┼────────────────┐
              │                │                │
              ▼                ▼                ▼
       ┌─────────────┐  ┌─────────────┐  ┌─────────────┐
       │ ML Inference│  │ Data Layer  │  │ Task Queue  │
       │ Pipelines   │  │ PostgreSQL  │  │ Celery      │
       │             │  │ MongoDB     │  │ Redis       │
       └─────────────┘  └─────────────┘  └─────────────┘

🛠️ Technology Stack
- Languages: Python 3.9+, TypeScript
- Machine Learning: Scikit-Learn, PyTorch
- Data Processing: Pandas, NumPy
- Backend: FastAPI, SQLAlchemy
- Databases & Caching: PostgreSQL, MongoDB, Redis, Celery
- Frontend: Next.js 14, React, Tailwind CSS
- DevOps & Cloud: Docker, Docker Compose, AWS

📄 License
This project is distributed under the Apache License 2.0.
