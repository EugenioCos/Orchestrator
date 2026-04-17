# Orchestrator project

This project was developed in January 2026 following experimentation with 'Codex' and 'OpenClaw'.  
Below is an explanation of the project's objective and the milestones achieved.

## Premise

In April 2025, I invested in a computer equipped with a capable graphics card to run artificial intelligence models locally, avoiding the need to expose my data to services such as 'Gemini', 'ChatGPT', 'DeepSeek', etc.  

When coding tools like 'Codex', 'Claude', 'OpenClaw', etc. were released, I immediately realized they are not designed to work with the local AI models my graphics card can support.  

At that point, I asked myself:  

- The models I run locally work perfectly—why do these coding tools yield poor results?  

The answers I arrived at were:  

- The capabilities required of an AI agent exceed those needed for standard conversational use, which I was accustomed to.  

- These tools were built for worldwide deployment, not for specific local setups, and primarily target clients willing to invest in high-performance resources and models.

## Objective

This project aimed to explore the following questions:  

- By stripping commercial tools down to minimal functionality, can acceptable results be achieved using local models?  

- Is orchestration truly so complex and resource-intensive that it inherently demands high-performance models?

## Results Obtained

After one/two week of development, initial results were achieved:  

- Step-level orchestration is straightforward; high-performance models are not required. 

- The true critical challenges identified were:  

    - Context management and agent coordination.  

    - Reliable tool usage.  

- Acceptable results are achievable even with 12B-parameter models.

### What is meant by "acceptable results" in this project?

During testing, I implemented workflows requesting code review for:  

- Documentation  

- Modification  

- Review and correction  

- Adding new features that do not require complex integration with existing code  

### What does the code of this project consist of?

The core idea is to define development flows (non-linear, graph-structured) where steps can be specified either via predefined messages or through automated orchestration.  

The system comprises two modules:  

- **"IA" (AI)**: The application core. It interfaces with the provider (Ollama) and manages full orchestration. 

- **"OrchestratorClient"**: The interface that loads workflows and manages the agents' working environment.  

Advantages of this two-module architecture:  

- The workspace can reside on a device without the AI provider installed, requiring only Python and the GitPython library.  

- Logic is cleanly separated.  

- Adding new components (e.g., a web interface) is simplified.

### Usage Documentation

- [Server documentation](./IA/README.md)  

- [Client documentation](./OrchestratorClient/README.md)  

## Contact me for more info

I have discontinued this project having achieved its objectives and exhausted the available time. For any questions or requests, please do not hesitate to reach out.  

[Portfolio with contact module](https://www.ceugenio.org)