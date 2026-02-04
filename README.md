# 🚀 DeepResearch: Industrial-Grade Multi-Agent Research Platform

## 🌟 Overview
Deep-Research is an industrial-grade autonomous intelligence engine designed for deep-dive market synthesis. Moving beyond standard RAG patterns, the system implements a Multi-Agent Orchestration layer that mirrors the cognitive process of expert analysts. By leveraging an asynchronous OODA-loop (Observe-Orient-Decide-Act), it transforms raw, multi-source data into structured, high-fidelity research assets.

---
## 💡 Motivation & Inspiration
The genesis of Deep-Research stems from my professional background in Management Consulting and Financial IPO sectors. During my previous internships, I experienced firsthand that Desk Research—the meticulous process of gathering, verifying, and synthesizing multi-source intelligence—is a critical yet time-consuming bottleneck in high-stakes decision-making.

I recognized that the emergence of Large Language Models (LLMs) presents a transformative opportunity to improve these workflows. Since my prior professional consulting/financial IPO experiences were centered in the Chinese financial and consulting sectors, the current implementation is for the complex regulatory and industrial landscape of the Chinese market.

While the data sources are localized to specific industrial landscapes, the underlying architecture is entirely **market-agnostic**. The multi-agent orchestration framework, including RAG, data analysis, self-reflection and etc, is engineered to be seamlessly adapted for US industrial research, global market synthesis, or any other industrial context.

---
>## 💎 Core Value Proposition: Optimizing Industrial Research via Multi-Agent Automation

>### 1. Exponential Efficiency Gains
Traditional industrial research typically requires 3-5 days of manual labor for data collection and synthesis.  
**Deep-Research compresses this cycle in under 30 minutes**, enabling rapid decision-making without sacrificing depth.

>### 2. Collaborative Intelligence & Analytical Rigor
Orchestrated via a Multi-Agent ecosystem, the system simulates a high-level research team.  
By utilizing a specialized **Critic-in-the-loop mechanism**, it ensures that every report meets the standards of professional consulting and investment firms.

>### 3. Autonomous Synthesis & Multi-Modal Delivery
Beyond mere text summaries, the platform automates **Data Visualization and Professional Formatting**.  
It produces "Production-Ready" reports with structured layouts and insightful charts, ready for executive-level review.

---

## 📑 Table of Contents
- [🏗️ System Architecture](#system-architecture)

---

## 🏗️ System Architecture

The 4-Layer Implementation:

### 1. Presentation Layer (Frontend)
**Technology Stack**
| Category | Technology |
|:---|:---|
| **Core** | React 18, TypeScript, Zustand, Axios |
| **UI Framework** | Ant Design 5.x |
| **Visualization** | ECharts 5.x, Recharts |
| **Rendering** | react-markdown, rehype-highlight |

### 2. API & Gateway Layer
- **FastAPI + Modular Routing**: For scalable and maintainable backend orchestration.
- **Auth + Session Management**: Ensuring secure and stateful user research sessions.
- **SSE Streaming**: Providing real-time, transparent agentic reasoning updates.

### 3. Intelligence Orchestration Layer (🤖 Multi-Agent system)
Orchestrated via **LangGraph**, the system manages 6 specialized agents:
- **Architect**: Decomposes complex research queries into structured execution plans.
- **Scout**: Performs multi-source retrieval and web crawling.
- **Data Analyst**: Extracts structured entities and constructs domain-specific knowledge graphs.
- **CodeWizard**: Automates data visualization and chart generation.
- **LeadWriter**: Synthesizes multi-source intelligence into structured, professional reports.
- **CriticMaster**: Performs logical audits and quality control.

Supporting AI Services:
- **Text2SQL**: Empowers non-technical users to query complex industrial databases using natural language.
- **RAG**: Document parsing, vectorization and retrieval.

### 4. Data Layer
- **PostgreSQL**: Relational metadata and user session management.
- **Milvus**: High-performance vector storage for semantic retrieval.
- **Elasticsearch**: Full-text search for precise terminology matching.
- **Redis**: Real-time state management and short-term memory caching.
- **MinIO**: Object storage for original PDF reports and generated assets.

---

## 🛠️ Tech Stack & Key Innovations
- **Agentic Workflow**: Stateful OODA loop implementation.
- **Self-Healing Execution**: Autonomous Python sandbox that detects and fixes runtime errors during data analysis.
- **Source Tracing**: Every claim in the generated report is mapped back to its primary source in the vector/search layer.
- **Containerization**: Fully Dockerized deployment for environment consistency.

---

## 📂 Project Structure

```text
industry_information_assistant/
├── backend/
│   ├── app/
│   │   ├── api/          # API Routes
│   │   ├── core/         # Core Configurations
│   │   ├── models/       # Data Models
│   │   ├── service/      # Business Logic
│   │   └── app_main.py   # Application Entry Point
│   ├── docker-compose-base.yml
│   ├── requirements.txt
│   └── .env
├── frontend/
│   ├── src/
│   │   ├── api/          # API Integration
│   │   ├── components/   # UI Components
│   │   ├── pages/        # Application Pages
│   │   └── store/        # State Management
│   └── package.json
└── README.md
