# Multi-Agent Financial Trading System using Crew AI

## 📝 Project Overview
This project is a **Local Trading Research Assistant** built using **Crew AI**, a framework for creating autonomous multi-agent systems. The system leverages multiple AI agents, each specialized in a specific domain of financial trading:
- 🧑‍💼 **Data Analyst Agent:** Monitors and analyzes market data in real-time.  
- 📊 **Trading Strategy Developer:** Designs trading strategies based on market insights.  
- 💡 **Trade Advisor:** Provides execution recommendations for trading strategies.  
- ⚖️ **Risk Advisor:** Evaluates and advises on trading risks.  

The agents collaborate to fetch market data, analyze trends, formulate strategies, recommend execution, and assess risks, providing a **comprehensive financial trading insight**.

---

## 🚀 Key Features
- **Local LLM Integration:** Uses a locally hosted Llama model for fast and private inference.  
- **Multi-Agent Coordination:** Crew AI manages task delegation among agents.  
- **Financial Trading Insights:** Generates actionable trading recommendations.  
- **Streamlit Interface:** Interactive UI for running analyses and displaying results.

---

## 🤔 How Crew AI Works
1. **Task Assignment:** Each agent is assigned tasks based on their role.  
2. **Tool Utilization:** Agents can use tools like web scrapers or search APIs to gather data.  
3. **Delegation & Collaboration:** Agents can delegate subtasks to other agents if required.  
4. **Task Completion:** Agents generate outputs for their tasks.  
5. **Aggregation:** Crew AI combines results from all agents into a final output.

**Crew AI Workflow Image:**

![App Screenshot](crewAI_workflow.png)

---

## 🏗️ Project Architecture
The system consists of four main modules:
1. **app.py** – Streamlit interface, triggers the Crew AI process.
2. **crew_agents.py** – Defines the multi-agent team and their capabilities.
3. **tasks.py** – Assigns tasks to agents and defines expected outputs.
4. **local_llm.py** – Loads and runs the local LLM for generating insights.

![App Screenshot](financial_trading_architecture.png)
---

## ⚙️ Installation
1. **Clone the Repository:**
```bash
git clone https://github.com/ritvika-talreja/multi-agent-financial-trading.git
cd multi-agent-financial-trading
```
2. **Create a Virtual Environment and Activate it:**
```bash 
python -m venv .venv
# Linux/Mac
source .venv/bin/activate
# Windows
.venv\Scripts\activate
```
3. **Install Dependencies:**
```bash
pip install -r requirements.txt
```
4. **Update Model Path in app.py:**
```bash
MODEL_PATH = r"path\to\your\model.gguf"
```   




