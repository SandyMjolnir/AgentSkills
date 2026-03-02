# AgentSkills

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
[![GitHub Stars](https://img.shields.io/github/stars/SandyMjolnir/AgentSkills?style=social)](https://github.com/SandyMjolnir/AgentSkills/stargazers)
[![GitHub Issues](https://img.shields.io/github/issues/SandyMjolnir/AgentSkills)](https://github.com/SandyMjolnir/AgentSkills/issues)

> A curated collection of modular, reusable skills for AI agents — designed to be composable, extensible, and easy to integrate.

---

## Table of Contents

- [Overview](#overview)
- [Features](#features)
- [Getting Started](#getting-started)
  - [Prerequisites](#prerequisites)
  - [Installation](#installation)
- [Usage](#usage)
- [Project Structure](#project-structure)
- [Contributing](#contributing)
- [License](#license)

---

## Overview

**AgentSkills** is an open-source repository that provides a growing library of well-defined skills for autonomous AI agents. Each skill is designed to be:

- **Self-contained** – minimal external dependencies per skill.
- **Composable** – skills can be chained or combined to build complex agent workflows.
- **Documented** – every skill ships with a clear description, inputs, outputs, and usage examples.

Whether you are building a personal assistant, a code-generation bot, a research agent, or any other AI-powered application, AgentSkills gives you a solid foundation to start from.

---

## Features

- 📦 **Modular skill library** – add only the skills you need.
- 🔌 **Framework agnostic** – works alongside popular agent frameworks (LangChain, AutoGen, CrewAI, etc.).
- 📝 **Consistent skill interface** – every skill follows a standard contract for inputs and outputs.
- 🧪 **Tested** – each skill includes unit tests to ensure reliability.
- 🚀 **Extensible** – contribute new skills or fork the project to build your own private collection.

---

## Getting Started

### Prerequisites

- Python 3.10 or higher (or the relevant runtime for your chosen skill set)
- `pip` (Python package manager)
- An API key for your preferred LLM provider (e.g., OpenAI, Azure OpenAI, Anthropic) if you plan to use LLM-dependent skills

### Installation

```bash
# Clone the repository
git clone https://github.com/SandyMjolnir/AgentSkills.git
cd AgentSkills

# (Recommended) Create and activate a virtual environment
python -m venv .venv
source .venv/bin/activate   # On Windows: .venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt
```

---

## Usage

```python
from agent_skills import SomeSkill

skill = SomeSkill()
result = skill.run(input="your input here")
print(result)
```

> **Note:** Replace `SomeSkill` with the name of the skill you want to use. Refer to the individual skill documentation under the `skills/` directory for detailed examples.

---

## Project Structure

```
AgentSkills/
├── skills/               # Individual skill modules
│   ├── __init__.py
│   └── <skill_name>/
│       ├── __init__.py
│       ├── skill.py      # Skill implementation
│       ├── README.md     # Skill-level documentation
│       └── tests/        # Unit tests for this skill
├── examples/             # End-to-end usage examples
├── docs/                 # Project-level documentation
├── requirements.txt      # Python dependencies
├── LICENSE
└── README.md
```

---

## Contributing

Contributions are welcome and appreciated! Here is how to get involved:

1. **Fork** the repository.
2. **Create** a feature branch: `git checkout -b feature/my-new-skill`.
3. **Implement** your skill following the existing conventions.
4. **Add tests** for your skill in the appropriate `tests/` directory.
5. **Commit** your changes with a descriptive message.
6. **Open a Pull Request** against the `main` branch and describe what your skill does.

For now, follow the conventions demonstrated in existing skills. A full `CONTRIBUTING.md` with detailed guidelines, code style requirements, and review process will be added soon.

---

## License

This project is licensed under the **MIT License** — see the [LICENSE](LICENSE) file for details.

---

<p align="center">Made with ❤️ by <a href="https://github.com/SandyMjolnir">SandyMjolnir</a></p>
