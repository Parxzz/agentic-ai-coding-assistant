# Agentic AI Coding Assistant

An **AI-powered coding assistant** that converts natural language project ideas into structured development plans and automatically generates project files.

This project demonstrates how **agent-based AI workflows** can automate parts of the software development process using modern LLM frameworks.

---

## Features

- Convert natural language prompts into structured project plans
- Multi-agent workflow for planning and code generation
- Automatic creation of project files
- Structured AI outputs using schema validation
- Secure environment variable management
- Modular architecture for easy extension

---

## Tech Stack

- Python
- LangChain
- LangGraph
- Groq LLM
- Pydantic
- python-dotenv

---

## Project Architecture

The system follows an **agentic workflow**:

User Prompt  
↓  
Planner Agent (creates structured project plan)  
↓  
Coder Agent (generates code for each file)  
↓  
Tool Execution (writes files to disk)  
↓  
Generated Project Files

Agents communicate through **state management and structured outputs** to ensure reliable code generation.

---

## Project Structure

```
agentic-ai-coding-assistant
│
├── agent
│   ├── graph.py
│   ├── tools.py
│
├── main.py
├── pyproject.toml
├── .env.example
└── README.md
```

---

## Installation

Clone the repository

```bash
git clone https://github.com/yourusername/agentic-ai-coding-assistant.git
cd agentic-ai-coding-assistant
```

Create a virtual environment

```bash
python -m venv .venv
```

Activate environment

Windows:

```bash
.venv\Scripts\activate
```

Install dependencies

```bash
pip install -r requirements.txt
```

---

## Environment Setup

Create a `.env` file and add your Groq API key:

```
GROQ_API_KEY=your_api_key_here
```

---

## Running the Project

Run the application:

```bash
python main.py
```

Enter a project prompt when requested, for example:

```
create a digital clock application
```

The system will generate a structured plan and create project files accordingly.

---

## Example Output

Example prompt:

```
create a simple digital clock
```

Generated files:

```
clock.py
time.py
alarm.py
```

---

## Key Concepts Demonstrated

- Agentic AI workflows
- LLM orchestration
- Structured outputs using schemas
- Tool-based execution
- State-driven agent pipelines

---

## Future Improvements

- Add a web interface using FastAPI
- Support multiple programming languages
- Add project templates
- Integrate GitHub auto-commit
- Enable real-time code execution

---

## Author

Paras Soni

---

## License

This project is for educational and learning purposes.
