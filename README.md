# ADK Basics - Simple ADK Multi-Tool Agent

A simple multi-tool AI agent built with **Google Agent Development Kit (ADK)**, **Groq Cloud**, and **LiteLLM**.

The agent can answer questions about **weather** and **current time** in a city, powered by **LLaMA 3.3 70B** — completely free, no Google API key required.

---

## 🛠️ Tech Stack

- [Google ADK](https://google.github.io/adk-docs/) - Agent Development Kit
- [Groq Cloud](https://console.groq.com) - Free LLM API
- [LiteLLM](https://docs.litellm.ai/) - Model integration bridge
- Python 3.10+

---

## ⚙️ Setup

### 1. Clone the repository
git clone https://github.com/Blimax7/ADK-Basics---simple-adk-multi-tool-agent.git
cd ADK-Basics---simple-adk-multi-tool-agent

### 2. Create and activate virtual environment
python -m venv .venv

# Windows CMD
.venv\Scripts\activate.bat

# Windows PowerShell
.venv\Scripts\Activate.ps1

# macOS/Linux
source .venv/bin/activate

### 3. Install dependencies
pip install google-adk litellm

### 4. Add your Groq API key
Create a `.env` file inside the `multi_tool_agent/` folder:
GROQ_API_KEY=your_actual_groq_api_key_here

Get your free API key at [console.groq.com](https://console.groq.com)

---

## 🚀 Run the Agent

adk web

Then open your browser at **http://localhost:8000** and select `multi_tool_agent` from the dropdown.

---

## 💬 Example Prompts

- `What is the weather in New York?`
- `What is the time in New York?`
- `What is the weather in Paris?`
- `What is the time in Paris?`

---

## 📁 Project Structure

ADK-Groq/
└── multi_tool_agent/
    ├── __init__.py   → Registers the agent package
    ├── agent.py      → Defines tools and the agent
    └── .env          → Stores your Groq API key (not uploaded)

---

## 📌 Notes

- `.env` is excluded from the repository via `.gitignore` to protect your API key
- Built-in ADK tools like `google_search` are not supported with third-party LLMs
- Only custom Python function tools work with Groq via LiteLLM
- `.env` is excluded from the repository via `.gitignore` to protect your API key
- Built-in ADK tools like `google_search` are not supported with third-party LLMs
- Only custom Python function tools work with Groq via LiteLLM
