# 🇮🇳 BharatShield  
### AI-Driven Strategic Simulation Platform (DBMS-Oriented Project)

---

## 📌 Overview
**BharatShield** is an AI-assisted strategic simulation platform designed to model **geopolitical, policy, and crisis-response scenarios** in a safe, abstract, and academic environment.

The project is primarily designed as a **Database Management Systems (DBMS) application**, focusing on:
- Structured data modeling
- Scenario storage and retrieval
- Decision–outcome relationships
- Analytics over historical simulation data

While India-focused by default, the system architecture is **country-agnostic**.

---

## 🎯 Problem Statement
Strategic simulations involve large volumes of interconnected data such as:
- Countries and regions
- Scenarios and constraints
- Decisions and outcomes
- Media narratives and public sentiment

Traditional static databases fail to:
- Represent complex relationships
- Track multi-stage decision flows
- Support analytical queries on simulated outcomes

---

## 💡 Solution
BharatShield implements a **well-structured relational database system** combined with an AI reasoning layer to:

- Store geopolitical entities and scenarios
- Track user decisions and their consequences
- Maintain historical simulation runs
- Enable analytical queries and comparisons
- Generate AI-assisted narrative insights based on stored data

The emphasis is on **data modeling, normalization, relationships, and queries**, aligned with DBMS concepts.

---

## 🧠 Core Modules

### 1️⃣ Scenario Management
- Create and manage scenarios
- Associate countries, constraints, and risk factors
- Store scenario metadata in normalized tables

### 2️⃣ Decision Tracking
- Record policy-level decisions taken by users
- Maintain decision timelines
- Link decisions to scenarios and simulation runs

### 3️⃣ Outcome & Impact Storage
Each decision produces multiple outcomes stored across dimensions:
- Stability index
- Economic impact
- Diplomatic impact
- Media sentiment
- Public response

### 4️⃣ Media & Narrative Records
- AI-generated headlines and summaries
- Stored as structured narrative data
- Queryable for trend and sentiment analysis

### 5️⃣ Analytics & Query Engine
Supports DBMS-focused queries such as:
- Comparing outcomes across scenarios
- Tracking decision effectiveness
- Aggregating sentiment over time
- Identifying high-risk policy patterns

---

## 🗄️ Database Design (High-Level)

### Key Entities
- `Country`
- `Scenario`
- `Simulation_Run`
- `Decision`
- `Outcome`
- `Media_Narrative`
- `Public_Sentiment`

### Relationships
- One country → many scenarios  
- One scenario → many simulation runs  
- One simulation run → many decisions  
- One decision → multiple outcomes  
- One simulation run → multiple media narratives  

---

## 🧩 Tech Stack

- **Frontend:** Flutter / React  
- **Backend:** Node.js + Express  
- **Database:** MySQL  
- **AI Layer:**  
  - Scenario reasoning (LLM-based)
  - Sentiment classification
  - Probabilistic outcome generation  

---

## 🛡️ Ethical & Academic Scope
BharatShield is:

- ❌ NOT a military command system  
- ❌ NOT an operational or tactical planner  
- ❌ NOT connected to real-time or classified data  

It is:
- ✅ Abstract and academic  
- ✅ Designed for learning DBMS concepts  
- ✅ Focused on data modeling and analysis  

All simulations are **hypothetical**.

---

## 📐 System Architecture

```mermaid
flowchart TD

A[User Interface<br/>(Web / App)] --> B[Backend API<br/>(Node.js + Express)]

B --> C[Scenario Service]
B --> D[Decision Service]
B --> E[Analytics Service]

C --> F[(MySQL Database)]
D --> F
E --> F

B --> G[AI Reasoning Layer]
G --> B

F --> H[Reports & Visualizations]
