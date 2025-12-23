## Prompt Chaining - Agentic Workflow Design Pattern

Prompt Chaining is a foundational design pattern in agentic AI workflows. It breaks down complex tasks into a sequence of smaller, interconnected prompts, where the output of one large language model (LLM) call becomes the input for the next.

This approach enables structured, step-by-step reasoning and improves reliability, controllability, and performance compared to handling everything in a single large prompt.

### How It Works
In prompt chaining:

1. A complex goal decomposes into logical subtasks.
2. Each subtask is handled by a specialized prompt.
3. Outputs are passed sequentially (often formatted as structured data like JSON for easy parsing).
4. The chain continues until the final result is produced.

This mimics a pipeline or assembly line, allowing focused processing at each stage. It evolved from techniques like Chain-of-Thought prompting but emphasizes modular, sequential execution.

