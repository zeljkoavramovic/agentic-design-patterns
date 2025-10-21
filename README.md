# Agentic Design Patterns

This repository contains an interactive, single-file tutorial on 21 essential agentic design patterns for building intelligent AI systems.



## Overview

The included `index.html` file is a self-contained web page that provides a comprehensive guide to various patterns used in modern AI development. It's designed to make complex architectural concepts accessible through simple visual representations, detailed explanations, and real-world examples.

### Online Use
Open https://zeljkoavramovic.github.io/agentic-design-patterns/ in your browser

### Offline Use
Simply download the `index.html` file and open it in any modern web browser. No internet connection is required after the initial download.



## Pattern Relationships

The following diagram illustrates how different agentic patterns often connect and rely on each other. This provides a high-level view of the ecosystem.

```mermaid
graph LR
    subgraph "Core Patterns"
        P1("Prompt Chaining")
        P2("Routing")
        P3("Parallelization")
        P4("Reflection")
        P5("Tool Use")
    end
    subgraph "Advanced Patterns"
        P6("Planning")
        P7("Multi-Agent Collaboration")
        P8("Memory Management")
        P9("Learning and Adaptation")
        P10("MCP")
    end
    subgraph "System Patterns"
        P11("Goal Setting & Monitoring")
        P12("Exception Handling & Recovery")
        P13("Human-in-the-Loop")
        P14("Knowledge Retrieval RAG")
        P15("Inter-Agent Communication")
    end
    subgraph "Optimization & Strategic"
        P16("Resource-Aware Optimization")
        P17("Reasoning Techniques")
        P18("Guardrails & Safety")
        P19("Evaluation & Monitoring")
        P20("Prioritization")
        P21("Exploration & Discovery")
    end
    
    P7 -- "requires" --> P15
    P7 -. "uses" .-> P6
    P7 -. "uses" .-> P8
    P6 -- "can be composed of" --> P1
    P6 -- "often requires" --> P5
    P14 -- "is a form of" --> P5
    P2 -- "is used by" --> P16
    P4 -- "is a form of" --> P19
    P9 -- "is enabled by" --> P13
    P13 -- "is triggered by" --> P18
    P13 -- "is triggered by" --> P12
    P17 -- "can be improved by" --> P4
    P21 -- "is a form of" --> P6
    P1 -- "often needs" --> P12
```



## Patterns Included

The tutorial covers the following 21 patterns, grouped into categories:

### Core Patterns
- Prompt Chaining
- Routing
- Parallelization
- Reflection
- Tool Use

### Advanced Patterns
- Planning
- Multi-Agent Collaboration
- Memory Management
- Learning and Adaptation
- Model Context Protocol (MCP)

### System Patterns
- Goal Setting & Monitoring
- Exception Handling & Recovery
- Human-in-the-Loop
- Knowledge Retrieval (RAG)
- Inter-Agent Communication

### Optimization Patterns
- Resource-Aware Optimization
- Reasoning Techniques
- Guardrails & Safety
- Evaluation & Monitoring

### Strategic Patterns
- Prioritization
- Exploration & Discovery



## Credits

The patterns, diagrams, and explanations are sourced from the excellent work done by Prompt Advisers. For more information and to view the original source files, please visit their GitHub repository:

[https://github.com/promptadvisers/agentic-design-patterns-docs](https://github.com/promptadvisers/agentic-design-patterns-docs)

For those who want to dig much deeper, their work is based on a book from Antonio Gulli:

https://www.amazon.com/Agentic-Design-Patterns-Hands-Intelligent/dp/3032014018
