# CursorRIPER Framework 

A comprehensive framework for AI-assisted software development in Cursor IDE that combines structured workflow with persistent memory.

## Overview

CursorRIPER provides a systematic approach to software development through five distinct operational modes:

1. **Research**: Information gathering and understanding existing code
2. **Innovate**: Brainstorming potential approaches and solutions
3. **Plan**: Creating detailed technical specifications
4. **Execute**: Implementing approved plans with precision
5. **Review**: Validating implementation against plans

This framework prevents unintended modifications while maintaining perfect continuity across coding sessions.

```mermaid
flowchart TD
    Start([Start]) --> Init{Project<br>Initialized?}
    Init -->|No| StartPhase[START Phase]
    Init -->|Yes| RIPER[RIPER Workflow]
    
    subgraph StartPhase[START Phase]
        S1[1. Requirements] --> S2[2. Technology]
        S2 --> S3[3. Architecture]
        S3 --> S4[4. Scaffolding]
        S4 --> S5[5. Environment]
        S5 --> S6[6. Memory Bank]
    end
    
    subgraph RIPER[RIPER Workflow]
        R[Research] --> I[Innovate]
        I --> P[Plan]
        P --> E[Execute]
        E --> Rev[Review]
        Rev -.-> R
    end
    
    StartPhase --> RIPER
```

## Features

- **Structured Workflow**: Clear separation of development phases
- **Memory Bank**: Persistent documentation across sessions
- **Project Intelligence**: Learning from patterns and preferences
- **State Management**: Explicit tracking of project phase and mode
- **Safe Initialization**: Guided setup with protection against re-initialization

## Getting Started

1. Copy the framework files to your project:
   ```bash
   cp -r src/.cursor your-project/.cursor
   ```

2. Initialize your project with:
   ```
   /start
   ```

3. Follow the START phase to set up your project structure and memory bank

4. Use the RIPER workflow for ongoing development

## Documentation

- [Setup Guide](docs/setup-guide.md)
- [START Phase Guide](docs/start-phase-guide.md)
- [RIPER Workflow Guide](docs/riper-workflow-guide.md)
- [Memory Bank Guide](docs/memory-bank-guide.md)
- [Custom Modes Guide](docs/custom-modes-guide.md)

## License

This project is licensed under the MIT License - see the LICENSE file for details.

---
The orginial RIPER framework is by: [robotlovehuman](https://github.com/robotlovehuman)

*The CursorRIPER Framework prevents coding disasters while maintaining perfect continuity across sessions.*
