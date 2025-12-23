## Agentic Workflow Patterns

Large Language Models (LLMs) have transformed how we tackle complex tasks, enabling the creation of agents that operate autonomously. Unlike AI agents that function without a predefined sequence of steps, agentic workflows leverage LLMs within structured, task-oriented processes. To design effective LLM workflows, it's crucial to understand key patterns. In this tutorial, we'll explore four essential workflow patterns: Prompt Chaining, Orchestrator-Workers, Evaluator-Optimizer, and Parallelization.


# Agentic Workflow Patterns

[![GitHub stars](https://img.shields.io/github/stars/mohamedaadhil96/agentic-workflow-patterns?style=social)](https://github.com/mohamedaadhil96/agentic-workflow-patterns/stargazers)
[![GitHub forks](https://img.shields.io/github/forks/mohamedaadhil96/agentic-workflow-patterns?style=social)](https://github.com/mohamedaadhil96/agentic-workflow-patterns/forks)
[![GitHub license](https://img.shields.io/github/license/mohamedaadhil96/agentic-workflow-patterns)](https://github.com/mohamedaadhil96/agentic-workflow-patterns/blob/main/LICENSE)

A curated collection of design patterns for building **agentic AI workflows** with Large Language Models (LLMs).

This repository explores proven patterns like prompt chaining, tool calling, planning, reflection, routing, multi-agent collaboration, and more. Each pattern includes:
- Clear explanations
- Visual diagrams
- Code examples in popular frameworks (LangChain, LangGraph, AutoGen, with Groq for fast inference)

**Status**: Early stage — Prompt Chaining implemented; others coming soon. Contributions welcome!

## Table of Contents

- [Introduction](#introduction)
- [Key Patterns](#key-patterns)
- [Installation](#installation)
- [Contributing](#contributing)
- [License](#license)

## Introduction

Large Language Models (LLMs) have transformed how we tackle complex tasks, enabling the creation of agents that operate autonomously. Unlike traditional AI agents that may lack predefined structure, **agentic workflows** leverage LLMs within structured, task-oriented processes.

To design effective and scalable LLM applications, it's crucial to understand recurring design patterns. This repository serves as a practical guide and reference for building robust agentic systems.

## Key Patterns

### 1. Prompt Chaining
**Description**: Breaks down a complex task into a sequence of simpler prompts, where the output of one prompt feeds into the next. Ideal for step-by-step reasoning, data transformation, or multi-stage generation.

**Use Cases**: Content generation pipelines, research summarization, code refactoring.

```mermaid
graph LR
    A[User Input] --> B[Prompt 1: Extract Key Facts]
    B --> C[Output 1]
    C --> D[Prompt 2: Analyze Implications]
    D --> E[Output 2]
    E --> F[Prompt 3: Generate Final Response]
    F --> G[Final Output]
