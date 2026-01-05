# 🚀 EDA Integration LLM Framework

An automated **Exploratory Data Analysis (EDA)** assistant powered by **Mistral AI**, **Ollama**, and **Gradio**. This framework allows you to perform deep data exploration using natural language queries in a 100% local and private environment.

## 🛠️ The Stack
- **LLM:** Mistral AI (7B)
- **Local Inference:** Ollama
- **Interface:** Gradio UI
- **Data Engine:** Pandas & Python

## ✨ Features
- **Privacy-First:** All data remains on your local machine; no cloud APIs required.
- **Semantic Understanding:** Automatically maps raw column names to human-readable descriptions.
- **Automated Insights:** Generate statistical summaries, correlation reports, and data quality checks through chat.
- **Interactive UI:** A clean, web-based dashboard for file uploads and real-time LLM interaction.

---

## 📊 Data Dictionary (Titanic Example)
The framework is optimized to understand the context of your variables. Below is the mapping used for the default Titanic dataset analysis:

| Variable | Description |
| :--- | :--- |
| **Survived** | Survival (0 = No, 1 = Yes) |
| **Pclass** | Ticket class (1 = 1st, 2 = 2nd, 3 = 3rd) |
| **Sex / Age** | Demographics of the passenger |
| **SibSp** | # of siblings / spouses aboard the Titanic |
| **Parch** | # of parents / children aboard the Titanic |
| **Ticket / Fare** | Ticket number and passenger fare |
| **Cabin** | Cabin number |
| **Embarked** | Port of Embarkation (C = Cherbourg, Q = Queenstown, S = Southampton) |

---

## ⚙️ Installation

### 1. Prerequisite: Ollama
Download and install [Ollama](https://ollama.ai/). Once installed, pull the Mistral model:
```bash
ollama pull mistral
