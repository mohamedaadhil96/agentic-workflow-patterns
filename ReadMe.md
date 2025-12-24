
# Agentic Workflow Patterns

[![GitHub stars](https://img.shields.io/github/stars/mohamedaadhil96/agentic-workflow-patterns?style=social)](https://github.com/mohamedaadhil96/agentic-workflow-patterns/stargazers)
[![GitHub forks](https://img.shields.io/github/forks/mohamedaadhil96/agentic-workflow-patterns?style=social)](https://github.com/mohamedaadhil96/agentic-workflow-patterns/forks)


Large Language Models (LLMs) have revolutionized how we approach complex problem-solving, enabling the creation of sophisticated AI agents that can operate autonomously or semi-autonomously. However, building robust, scalable, and maintainable agentic systems requires understanding fundamental design patterns.

Agentic workflows leverage LLMs within structured, task-oriented processes, combining the power of generative AI with proven software engineering principles. This repository serves as both a learning resource and a practical reference for developers building real-world LLM applications.

This repository explores proven patterns like prompt chaining, tool calling, planning, reflection, routing, multi-agent collaboration, and more. Each pattern includes:
- Clear explanations
- Visual diagrams
- Code examples in popular frameworks (LangChain, LangGraph, AutoGen, with Groq for fast inference)

**Status**: Early stage — Prompt Chaining implemented; others coming soon. Contributions welcome!

## Table of Contents

- [Introduction](#introduction)
- [Key Patterns](#key-patterns)

## Introduction

Large Language Models (LLMs) have transformed how we tackle complex tasks, enabling the creation of agents that operate autonomously. Unlike traditional AI agents that may lack predefined structure, **agentic workflows** leverage LLMs within structured, task-oriented processes.

To design effective and scalable LLM applications, it's crucial to understand recurring design patterns. This repository serves as a practical guide and reference for building robust agentic systems.

## Key Patterns

### 1. Prompt Chaining

![Prompt Chaining Workflow](https://github.com/mohamedaadhil96/agentic-workflow-patterns/blob/d5dea7811db450f144427593421cdc89257fcb1c/Prompt%20Chaining/prompt_chain_diagram.png)

**Description**: Prompt Chaining is a foundational design pattern in agentic AI workflows. It breaks down complex tasks into a sequence of smaller, interconnected prompts, where the output of one large language model (LLM) call becomes the input for the next.

This approach enables structured, step-by-step reasoning and improves reliability, controllability, and performance compared to handling everything in a single large prompt.

### How It Works
In prompt chaining:

1. A complex goal decomposes into logical subtasks.
2. Each subtask is handled by a specialized prompt.
3. Outputs are passed sequentially (often formatted as structured data like JSON for easy parsing).
4. The chain continues until the final result is produced.

This mimics a pipeline or assembly line, allowing focused processing at each stage. It evolved from techniques like Chain-of-Thought prompting but emphasizes modular, sequential execution.

**NOTE**: This Breaks down a complex task into a sequence of simpler prompts, where the output of one prompt feeds into the next. Ideal for step-by-step reasoning, data transformation, or multi-stage generation.

**Use Cases**: Content generation pipelines, research summarization, code refactoring.

### 2. Agentic Workflow Design Pattern - Prompt Chaining

![Agentic Workflow](D:\Aadhil-Codes\Agentic_design_Patterns\Routing\routing_agent.png)

**Description**:The Routing Agentic Workflow Design Pattern is a foundational design pattern in agentic AI systems. It enables intelligent classification of user inputs and dynamic delegation to specialized agents, tools, prompts, or sub workflows.

#### How It Works
A central "router" component typically powered by a large language model (LLM) analyzes the incoming query to determine its intent, category, complexity, or type. Based on this classification, it routes the task to the most appropriate specialized handler. This creates separation of concerns, allowing each downstream component to be optimized for specific tasks without compromising overall system performance.

**Use Cases**: Customer Support Systems processes, Multi-Domain Question Answering, Cost/Performance Balancing



## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

