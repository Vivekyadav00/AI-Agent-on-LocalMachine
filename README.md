# 🤖 DevOps AI Agent – CrewAI + LLaMA 3.1 + Ollama

This is a **local AI agent project** built using [CrewAI](https://github.com/joaomdmoura/crewAI), powered by the [LLaMA 3.1](https://ollama.com/library/llama3) large language model running via [Ollama](https://ollama.com/). The agent is designed to assist with DevOps-related tasks — all running securely and privately on your local machine.

---

## 🛠️ Prerequisites

- Python 3.8 or newer
- [Ollama](https://ollama.com/) installed and running
- LLaMA 3.1 model pulled locally
- CrewAI CLI installed via pip

---

## 🚀 Setup Instructions

### 1. Check Python Version

```bash
python3 --version
```
Make sure it's Python 3.8 or later.

### 2. Create and Activate Virtual Environment

```bash
python3 -m venv crew
source crew/bin/activate
```

### 3. Install CrewAI CLI

```bash
pip install crewai
```

### 4. Install Ollama

```bash
curl -fsSL https://ollama.com/install.sh | sh
```

Start the Ollama service:

```bash
ollama serve
```

### 5. Pull the LLaMA 3.1 Model

```bash
ollama pull llama3
```

### 6. Create a New CrewAI Project

```bash
crewai create devops-ai-project
cd devops-ai-project
```

### 7. Install Project Dependencies

```bash
crewai install
```

### 8. Run the Agent

```bash
crewai run
```

## 📁 Project Structure

```
devops-ai-project/
├── agents/
│   └── devops_expert.py
├── tasks/
│   └── automate_infra.py
├── main.py
├── requirements.txt
└── README.md
```

## 🧠 What This Project Does

- Runs an LLM-powered AI agent completely offline
- Designed for DevOps workflows like infra automation, cloud scripting, YAML generation, etc.
- Uses CrewAI's modular agent-task architecture
- LLM backend powered by LLaMA 3.1 via Ollama

## 🔐 100% Private & Local

No API keys, no internet calls, no cloud processing. All prompt data and LLM outputs stay on your machine.

## 📌 Example Use Cases (Ideas)

- Generate Terraform modules
- Suggest Azure/AWS CLI commands
- Explain Kubernetes configurations
- Build CI/CD pipeline templates

## 🛣️ Roadmap Ideas

- [ ] Integrate command-line output parsing
- [ ] Create multiple DevOps role-based agents (SRE, Infra, Security)
- [ ] Add GitHub Actions or Jenkins YAML generator
- [ ] Add file input/output support

## 🙌 Credits

- [CrewAI](https://github.com/joaomdmoura/crewAI)
- [Ollama](https://ollama.com/)
- Meta's LLaMA 3.1

Give this project a ⭐ if it inspires you. PRs and ideas are welcome!
