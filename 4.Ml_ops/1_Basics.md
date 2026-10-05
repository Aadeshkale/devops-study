## AI ML Notes

##  1. What is AI and ML?

* **AI:** is a technology that enables machines to process information, recognize patterns, make decisions, and perform tasks that normally require human intelligence, with minimal or no direct human intervention.

* **MI:**  is a part of AI that allows computers to learn from data, identify patterns, and use what they learn to generate outputs, make predictions, or make decisions without being explicitly programmed for every task.

* AI is the broader concept of enabling machines to perform intelligent tasks, while ML is a subset of AI that enables machines to learn from data and improve their output.
In simple terms: AI is the goal, and ML is one way to achieve it.

---


##  2. What is Gen AI and ML?
* GenAI is a type of AI that creates new content such as text, images, videos, audio, or code.
* Traditional AI mainly analyzes data and makes predictions or decisions, while GenAI creates new content.
---

## 3. What is Deep Learning?

Deep Learning is a part of Machine Learning that uses neural networks with multiple layers to learn complex patterns from large amounts of data and generate predictions or outputs.

Example:
A deep learning model can learn from thousands of images and recognize whether a new image contains a cat or dog.

---
## 3. Supervised, Unsupervised, and Reinforcement Learning

* **Supervised Learning:** The model **learns from data with correct answers** and uses it to predict new results.
  *Example: Identifying whether an email is spam or not.*

* **Unsupervised Learning:** The model **learns from data without answers** and finds patterns or groups by itself.
  *Example: Grouping customers based on their behavior.*

* **Reinforcement Learning:** The model **learns by trying actions and getting rewards or penalties**.
  *Example: A robot learning which path to take.*

---
## 4. Pre-tuned vs. fine-tuned models  

* **Pre-tuned:** These models are already trained on big datasets for general purposes
  *Example: Foundation models like Gemma, Llama.*
* **Fine-tuned:** These models are trained on particular datasets for specific purposes
  *Example: Foundation models like Qwen Coder, DeepSeek-V3, Llama.*

---
## 5. What is an AI agent, Agentic AI 
* An AI agent is a software system that takes actions on your behalf. It uses an AI/ML model as its brain to understand, reason, and decide, and uses external tools, APIs, or systems to execute those actions and achieve a goal.
* Agentic AI is an autonomous AI system that can reason, plan, make decisions, use tools, and perform multiple steps to achieve a goal. It can also coordinate multiple AI agents for complex tasks when needed.

* AI Agent vs Agentic AI
  | **AI Agent** | **Agentic AI** |
  |---|---|
  | An **AI system that performs a task** | An **AI system that works autonomously toward a goal** |
  | Understands, reasons, uses tools, and takes actions | Plans, reasons, makes decisions, and takes **multiple actions** |
  | Usually focused on a specific task | Usually handles **complex, multi-step tasks** |
  | Example: “Check my email and summarize it.” | Example: “Monitor my emails, identify important requests, decide what needs to be done, and complete the tasks.” |

---
## Explain MCP server, Tools, skills 
* MCP Server: **MCP** is a standard followed by AI systems/Agents to communicate with other/external systems. **MCP Server**: A server that implements MCP and exposes those capabilities to an AI client.   
* **Tools**: A set of Callable functions/actions performed by AI systems/Agents. 
* **Skills**: A set of instructions/procedures/policies to teach AI systems on how to teach an AI System/agent how to perform a particular task.

  **Example:** A Cost Calculator Agent uses MCP tools to retrieve cost and usage data from external systems, while Skills define the instructions and workflow for how the agent should calculate, analyze, and present the results.

```text
                    Cost Calculator Agent
                            |
              ┌─────────────┴─────────────┐
              │                           │
           Skills                      MCP Server
              │                           │
     ┌────────┴────────┐          ┌───────┴────────┐
     │                 │          │                │
Calculation Skill   Presentation   Tool           Tool
                    Skill          │                │
     │                 │       get_pricing()     get_usage()
     │                 │          │                │
     │                 │          └───────┬────────┘
     │                 │                  ↓
     │                 │          Cost Data / APIs
     │                 │                  │
     └─────────────────┼──────────────────┘
                       ↓
                Agent processes
                & calculates
                       │
                       ↓
                  Final Result
                       │
                       ↓
                     User 
```
  
