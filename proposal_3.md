
# **Google Summer of Code 2025 Proposal: Gemini Web Agent Framework**  
**Author:** Samyak Sharma

---

## **Personal Information**
- **Name:** Samyak Sharma  
- **Email:** [sammi.bgas@gmail.com](mailto:sammi.bgas@gmail.com)  
- **GitHub:** [github.com/samyakshrma](https://github.com/samyakshrma)  
- **LinkedIn:** [linkedin.com/in/samyakshrma](https://linkedin.com/in/samyakshrma)

---

## **Synopsis**  
The goal of this project is to develop an open-source agent framework that leverages **Gemini 2.0**'s multimodal capabilities and function calling to autonomously perform web tasks such as browsing, form-filling, scraping, and interaction with modern web applications.

Inspired by tools like AutoGPT, Puppeteer, and LangGraph, the agent will combine LLM reasoning, DOM interaction, memory, and modular task planning. This will serve as a blueprint for future agents capable of interacting with any web environment through vision and tool-use.

---

## **Benefits to the Community**
Many current web automation tools require scripting or low-level control over browsers. This project will offer a declarative and high-level interface for building agents capable of understanding web environments visually and semantically.

Developers and researchers will be able to:
- Automate tedious web workflows.
- Test and prototype LLM agents in the browser.
- Extend the system with custom tools, memory modules, and planners.

This will lower the barrier for building intelligent agents and provide a testbed for multimodal reasoning research.

---

## **Deliverables**
1. **Web Environment Agent Core**
   - DOM parsing and screenshot extraction pipeline.
   - Vision + HTML encoder for input to Gemini.
   - Function-calling tools: navigation, click, fill, submit, scroll, etc.

2. **Task Planning via LangGraph-style Node Graphs**
   - Modular planner with pluggable nodes (tools, memory, evaluators).
   - Debug and trace agent decisions.

3. **Browser Automation API Layer**
   - Headless Chromium (Playwright or Puppeteer).
   - Visual state capture, page text, HTML, and bounding box generation.

4. **RAG + Toolformer-style Tool-Use Memory**
   - Store and retrieve past tool usage.
   - Reflect and modify tool calls using Gemini.

5. **Demos and Use Cases**
   - Form-filling bots, scraping agents, search + extract bots.
   - Agent that logs in and completes a workflow.

6. **Documentation and Tutorials**

---

## **Technical Details**

### **Architecture Overview**
- **Perception Layer:** Playwright extracts HTML, text, and a screenshot. These form Gemini’s context.
- **LLM Controller:** Gemini 1.5 Pro handles vision + function calls.
- **Tool Executor:** Executes actions via Playwright; handles failures.
- **Planner Engine:** LangGraph-style orchestrator routes outputs/tools/memory.
- **Memory and RAG:** Uses FAISS to retrieve prior steps for better reasoning.
- **Evaluator (Optional):** Scores or verifies task completion.

---

### **Tech Stack**
- **Languages:** Python, TypeScript  
- **Browser Automation:** Playwright or Puppeteer  
- **LLM Backend:** Gemini 1.5 Pro via Google AI Studio APIs  
- **Agent Framework:** LangGraph  
- **Visualization:** PyGraphviz / Mermaid.js  
- **Memory:** FAISS / ChromaDB  
- **Infrastructure:** Docker, SQLite/JSON  
- **Async Handling:** Python `asyncio`, WebSockets  

---

### **LLM Input Format Design**
- **Screenshot:** PNG of the browser viewport  
- **DOM Extract:** Clean HTML + visible text  
- **Task History:** List of previous steps  
- **User Objective:** Natural language input  

---

### **Security and Fault Tolerance**
- Tool validations for safe action execution.
- Try-except wrappers for resilient automation.
- Logging of every tool use and LLM decision.

---

### **Architecture Diagram**
![Architecture Diagram](Screenshot%20from%202025-04-08%2014-57-08.png)

---

## **Timeline**

| Week     | Milestone |
|----------|-----------|
| 1–2 | Research Gemini API and Playwright. Draft architecture. |
| 3–4 | Build screenshot + DOM converter. Design input format. |
| 5–6 | Develop toolset (click, scroll, fill). Integrate with Gemini. |
| 7–8 | Implement LangGraph-style planner. |
| 9–10 | Add memory and retrieval module. |
| 11–12 | Build and test use cases. |
| 13–14 | Finalize docs, polish, and create demo videos. |

---

## **Expected Size of Project**
**350 hours**

---

## **Skills Required**
- Python, TypeScript  
- FastAPI, Puppeteer, LangGraph  
- Gemini API and multimodal reasoning  
- Browser automation  
- Graph-based planning models  

---

## **Future Work**
- RLHF fine-tuning for agent actions.  
- Add speech input and TTS for voice agents.  
- Use in accessibility tools.

---

## **Why Me?**
I’m a CS undergrad (2022–2026) at Dayananda Sagar College of Engineering with a strong interest in AI and automation.

### **Projects and Experience**
- [**Code-Collab**](https://github.com/Samyakshrma/CodeCollab): Real-time collaborative coding via FastAPI + WebSockets + Redis.
- [**AI Assistant with Azure**](https://github.com/Samyakshrma/Voice_Assistant): Voice agent using FastAPI + Docker.
- [**MNIST From Scratch**](https://github.com/Samyakshrma/MNIST-NN-from-Scratch): DL framework in NumPy.
- **PDF QA + RAG Workflow:** LangChain + HuggingFace-powered QA.
- [**SCADA Topology (SIH 2024 Winner)**](https://www.linkedin.com/posts/samyakshrma_sih2024-winners-innovation-activity-7273965131846303744-AolN?utm_source=share&utm_medium=member_desktop&rcm=ACoAACqPzzUBjeMcFtE8RnPehts6E1RfCW--5K4):
  - EIGRP + SNMPv3 for secure monitoring
  - SSH setup for remote terminal
- [**Spam Detection**](https://github.com/Samyakshrma/sms-spam-detector): TF-IDF + Naive Bayes classifier with retraining pipeline.

### **Achievements**
- 🏆 **Winner** — Smart India Hackathon 2024  
- 🥈 **2nd Place** — Hack-O-Rama, Feb 2024  

With experience in LLMs, backend development, and browser automation, I’m confident in delivering this project successfully.
