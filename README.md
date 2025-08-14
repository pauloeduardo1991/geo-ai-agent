<p align="center">
  <a href="https://brightdata.com/">
    <img src="https://mintlify.s3.us-west-1.amazonaws.com/brightdata/logo/light.svg" width="300" alt="Bright Data Logo">
  </a>
</p>

<div align="center">
  <img src="https://img.shields.io/badge/python-3.10+-blue"/>
  <img src="https://img.shields.io/badge/License-MIT-blue"/>
</div>

---

# 🚀 GEO AI Crew

GEO Agent Crew with [CrewAI](https://crewai.com) automates AI-driven website content audits. Enter a URL, and the system crawls the site (with URL filtering), extracts H1s, generates and summarizes related queries using Gemini with Google Search, fetches Google AI Overviews via [Bright Data SERP API](https://brightdata.com/products/serp-api), compares results, and outputs actionable page-level optimization suggestions.

---

## 🛠️ Installation

Ensure you have **Python >=3.10 <3.14** installed on your system.  
This project uses [UV](https://docs.astral.sh/uv/) for dependency management and package handling, offering a seamless setup and execution experience.

First, if you haven't already, install uv:

```bash
pip install uv
```

Next, navigate to your project directory and install the dependencies:

```bash
uv pip install -r requirements.txt
```

*(Optional) Lock the dependencies and install them by using the CLI command:*

```bash
crewai install
```

---

### ⚙️ Customizing

**🔑 Add your `GOOGLE_API_KEY` into the `.env` file**

- 🧑‍💻 Modify `src/ai_content_optimization_agent/config/agents.yaml` to define your agents
- 📋 Modify `src/ai_content_optimization_agent/config/tasks.yaml` to define your tasks
- 🛠️ Modify `src/ai_content_optimization_agent/crew.py` to add your own logic, tools and specific args
- ⚡ Modify `src/ai_content_optimization_agent/main.py` to add custom inputs for your agents and tasks

---

## ▶️ Running the Project

To kickstart your crew of AI agents and begin task execution, run this from the root folder of your project:

```bash
$ crewai run
```

This command initializes the ai-content-optimization-agent Crew, assembling the agents and assigning them tasks as defined in your configuration.

☑️ This example, unmodified, will run the create a `report.md` file with the output of a research on LLMs in the root folder.

---

## 🤖 Understanding Your Crew

The ai-content-optimization-agent Crew is composed of multiple AI agents, each with unique roles, goals, and tools. These agents collaborate on a series of tasks, defined in `config/tasks.yaml`, leveraging their collective skills to achieve complex objectives. The `config/agents.yaml` file outlines the capabilities and configurations of each agent in your crew.

---

## 💬 Support

For support, questions, or feedback regarding the AiContentOptimizationAgent Crew or crewAI:

- ☀️ Visit Bright Data's [SERP API docs](https://docs.brightdata.com/scraping-automation/serp-api/introduction)
- 📖 Visit CrewAI's [documentation](https://docs.crewai.com)
- 🐙 Reach out to CrewAI through the [GitHub repository](https://github.com/joaomdmoura/crewai)
- 💬 [Join Discord](https://discord.com/invite/X4JWnZnxPb)
- 💡 [Chat with CrewAI's docs](https://chatg.pt/DWjSBZn)

---

✨ Let's create wonders together with the power and simplicity of Bright Data & crewAI.



