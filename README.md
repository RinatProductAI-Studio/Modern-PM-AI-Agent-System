# Modern PM AI Agent System (Proof of Concept)

This repository demonstrates how a modern, AI‑native Product Manager can design and deliver a multi‑agent system that automates core PM workflows such as risk detection, schedule awareness, planning alignment, and executive reporting.

The goal is not to build a production system.  
The goal is to provide a clear, simple, working example of how AI agents can support PM work — and how a PM can lead such a project from concept to prototype.

This project is part of a portfolio to demonstrate AI‑driven PM capabilities for resumes, LinkedIn, and interviews.

---

## 1. Purpose of This Project

This project aims to:

- Demonstrate modern PM thinking and AI literacy  
- Show how AI agents can automate PM workflows  
- Provide a working proof‑of‑concept **Risk Agent**  
- Document a simple multi‑agent architecture  
- Serve as a live demo during interviews  
- Showcase PM leadership in AI transformation  

---

## 2. What This Project Includes (Alpha Version)

### ✅ Working Components

**Risk Agent (fully implemented in proof‑of‑concept mode)**  
- Detects risks from text  
- Classifies risks  
- Scores risks (severity + hybrid probability)  
- Tracks risks in a simple list  
- Produces summaries  
- Proposes actions (requires human approval)  

### 🟦 Defined but Not Implemented (Stubs)

- Schedule Agent  
- Planning Agent  
- Collaboration Agent  
- Daily Summary Agent  

### 📘 Documentation

- Architecture explanation  
- Agent definitions  
- Example inputs and outputs  
- Project structure  

### 📂 Data Storage

- `risks.json` (simple list of risks)  
- JSON = a simple text format for storing structured data  

---

## 3. Why This Project Matters

Modern PM roles increasingly require:

- Understanding of AI agents  
- Ability to automate workflows  
- Ability to design agentic systems  
- Ability to collaborate with AI tools  
- Ability to build small prototypes  
- Ability to explain architecture clearly  

This project demonstrates all of these skills in a practical, accessible way.

---

## 4. Architecture Overview

Below is a simple ASCII diagram:
+----------------------+
|    Daily Summary     |
|        Agent         |
+----------+-----------+
^
|
+------------------+------------------+
|                                     |
+-------+--------+                    +--------+--------+
|   Risk Agent   | <---- signals ---- | Schedule Agent  |
+-------+--------+                    +--------+--------+
|                                     |
|                                     |
v                                     v
+-------+--------+                    +--------+--------+
| Collaboration  |                    |   Planning      |
|     Agent      |                    |     Agent       |
+----------------+                    +-----------------+

**Risk Agent = the central reasoning engine.**  
Other agents support it.

---

## 5. Risk Agent (Full Implementation)

The Risk Agent includes:

### **Risk Intake Engine**
Listens for signals from text, summaries, or other agents.

### **Risk Structuring Engine**
Creates structured risk entries with:
- Title  
- Description  
- Category  
- Impact type  
- Severity  
- State  
- Owner  

### **Probability Engine (Hybrid Model)**
Two inputs:
- **ProbabilityOwner** (from questionnaire)  
- **ProbabilitySystem** (from schedule analysis)  

Final probability = the higher of the two.

### **State Machine**
Risk lifecycle:
1. Signal detected  
2. Needs validation  
3. Confirmed  
4. Mitigation in progress  
5. Closed  

### **Action Proposal Engine**
Suggests actions but never executes without human approval.

---

## 6. Project Structure

modern-pm-ai-agents/
│
├── agents/
│   ├── risk_agent.md
│   ├── schedule_agent_stub.md
│   ├── planning_agent_stub.md
│   ├── collaboration_agent_stub.md
│   └── summary_agent.md
│
├── data/
│   └── risks.json
│
├── examples/
│   ├── example_input.md
│   └── example_output.md
│
└── README.md


---

## 7. How to Use This Project

1. Open the **Risk Agent** file.  
2. Review how the agent works.  
3. Open the example input file.  
4. Copy the sample text.  
5. Paste it into an AI assistant (Copilot or Claude).  
6. The agent will:
   - Detect risks  
   - Classify them  
   - Score them  
   - Produce a summary  
7. Copy the output into `example_output.md`.  
8. Use this project as a demo in interviews.  

---

## 8. Future Roadmap

### **Beta**
- Simulated schedule analysis  
- Simulated questionnaires  
- Compound risk detection  
- PM identity accounts  
- Demo video  

### **Final**
- Optional Jira integration  
- Optional Slack integration  
- Optional website  
- Case study  
- Full multi‑agent orchestration  

---

## 9. License
This project is open for learning, portfolio use, and demonstration.



