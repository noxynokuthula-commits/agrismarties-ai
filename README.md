AgriSmarties AI – Agricultural Intelligence Agent
Project Overview
AgriSmarties AI is an AI-powered agricultural intelligence system built using n8n automation workflows, Gemini embeddings, and a vector database. The system helps farmers identify crop issues, generate actionable recommendations, and produces structured agricultural reports for decision-making and government monitoring.
It combines conversational AI with real-time data storage and retrieval to support smarter farming and agricultural reporting.
Problem It Solves
Farmers often struggle with:
Delayed access to agricultural advice
Lack of structured reporting on crop issues
No centralized system for tracking pest or disease outbreaks
Limited connection between farmer queries and government monitoring systems
AgriSmarties AI solves this by turning farmer questions into structured intelligence data in real time.
Key Features
AI-powered farming assistant using retrieval-augmented generation (RAG)
Vector-based knowledge search for accurate agricultural responses
Automated classification of crop issues (pests, disease, irrigation, soil)
Structured reporting system for government monitoring
Risk detection and severity scoring (low, medium, high)
Real-time data logging for analytics and dashboards
Scalable workflow-based architecture using n8n
Tech Stack
n8n (workflow automation)
Gemini Embeddings API
Vector Database (Supabase / Pinecone / Qdrant)
Google Sheets (data logging & MVP dashboard)
Looker Studio (reporting layer)
Webhooks (API integration layer)
AI Agent (LLM orchestration)
System Architecture
Farmer Query → n8n Webhook → AI Agent → Vector Database Retrieval → Response Generation → Data Structuring → Storage → Government Dashboard
Workflows
1. AI Chat Workflow
Receives farmer questions via webhook
Sends query to AI Agent
Retrieves relevant agricultural data from vector database
Generates contextual farming advice
Returns response to user
2. Data Ingestion Workflow
Collects agricultural knowledge (crops, pests, soil data)
Splits and processes text into chunks
Generates embeddings using Gemini
Stores embeddings in vector database
3. Reporting Workflow
Extracts structured insights from farmer interactions
Logs crop issues, severity, and location data
Stores data in Google Sheets or database
Feeds into dashboard tools for visualization
4. Alert System Workflow (Optional)
Detects high-severity agricultural risks
Sends notifications via email or messaging systems
Flags urgent agricultural issues for response teams
Example Use Case
Farmer Input:
“My maize leaves are turning yellow and drying out”
AI Output:
Likely issue: Nutrient deficiency or pest infestation
Recommended action: Apply nitrogen-rich fertilizer and inspect for pests
Severity: Medium
Logged into government monitoring system for regional tracking
Data Output Structure
Each interaction is stored as:
Crop type
Problem category
Severity level
Farmer query
AI recommendation
Region (if provided)
Timestamp
Business & Government Value
Enables real-time agricultural monitoring
Supports early detection of crop diseases and pest outbreaks
Provides structured data for policy and resource allocation
Improves decision-making for agricultural departments
Scalable across regions and countries
How to Run
Import n8n workflows from /workflows folder
Configure environment variables (API keys, vector DB)
Activate ingestion workflow first
Activate chat workflow second
Test using webhook endpoint
Project Status
✔ Core AI agent completed
✔ Embedding-based knowledge system active
✔ Data ingestion pipeline functional
✔ Reporting structure implemented
⏳ Dashboard UI integration (next phase)Future Improvements
WhatsApp integration for farmers
Advanced crop disease prediction model
Satellite data integration
Mobile-friendly farmer assistant app
Full government analytics dashboard
Author
AgriSmarties AI Project – AI Automation Engineering Portfolio Project
Notes
This project demonstrates practical implementation of:
AI agent design
Retrieval-augmented generation (RAG)
Workflow automation
Data structuring for real-world systems
Scalable AI architecture for agriculture
