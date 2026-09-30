<h1 align="center">Hi, I'm Jean Gouttier 👋</h1>

<h3 align="center">
Applied AI Engineer · LLM · NLP · Automation · Backend Development
</h3>

<p align="center">
  <a href="https://linkedin.com/in/jeangouttier">
    <img src="https://img.shields.io/badge/LinkedIn-Jean%20Gouttier-0A66C2?style=flat-square&logo=linkedin&logoColor=white" />
  </a>
  <a href="mailto:gouttierjean@gmail.com">
    <img src="https://img.shields.io/badge/Email-gouttierjean%40gmail.com-EA4335?style=flat-square&logo=gmail&logoColor=white" />
  </a>
  <a href="https://portfolio-gouttier-jean.vercel.app/">
    <img src="https://img.shields.io/badge/Portfolio-Visit-111827?style=flat-square&logo=vercel&logoColor=white" />
  </a>
</p>

---

## About me

I build and ship applied AI systems: LLM integration, structured information extraction, computer vision models and data pipelines. Graduating from Epitech in September 2026 (MSc-level, AI specialisation) after nearly three years of apprenticeship in production environments.

My profile combines software development, internal tools, data processing and business process automation. I am currently building my skills around **LLMs**, **RAG**, **NLP** and AI-powered document analysis.

During my apprenticeship at **SUPINFO Paris**, I work on digitalization and automation projects involving educational planning, document generation, SQL databases, internal applications and technical documentation.

My goal is to build practical AI tools that solve real business problems and can be used by non-technical teams.

---

## Currently

**Looking for a permanent role (CDI) as an AI Engineer or Data Engineer
in the Paris area or remote.** Graduated from Epitech in September 2026.

* Building small, well-documented systems around LLMs: context
  management, structured outputs, failure handling.
* Deepening RAG, agent patterns and evaluation of AI systems.

---

## Selected projects

### Conversational chatbot with context management

A 200-line CLI chat over a local LLM. The interesting part was not the
model call, it was everything that breaks around it.

Three problems I hit and fixed: an inconsistent history when streaming
fails mid-response (the user message is stored, the answer never
arrives, and the next turn sends two consecutive user messages);
capping history by message count instead of tokens, which ignores what
actually fills the context window; and replacing truncation with
summarisation, which simply moved the growth problem into a system
message that no reduction step ever touched.

**Tech:** Python · Ollama · streaming · token budgeting
**Code:** [github.com/JinClaudius/PneumonIA](https://github.com/JinClaudius/AI-Chat)

---

### BagTrip — AI travel planning (team project, 5 people)

Final-year Epitech project where I acted as project lead on the AI side.
The system plans a full trip from a single prompt: destinations,
flights, accommodation, activities, packing list and budget.

I led the AI workstream and prototyped the orchestration in n8n, then
decided to drop it for a Python implementation once error handling and
testability became the priority. The final implementation was built by
two developers on the team.

**Architecture:** multi-agent pipeline over SSE streaming, ReAct
executor (the target model had no native function calling), embedding
based recommendation where the destination is locked server-side so the
model cannot invent one.

---

### PneumonIA — Medical image classification

Chest X-ray classification into three classes (Normal / Bacterial / Viral pneumonia),
evaluated on a 624-image test set.

**EfficientNet-B0 fine-tuned: 89% accuracy, 0.88 macro F1.** The most instructive part
was diagnosing a scratch CNN that reached 80% accuracy while never once predicting the
minority class — corrected through class weighting, LR scheduling and training-split-only
augmentation, bringing VIRAL F1 from 0.00 to 0.80. Predictions explained with Grad-CAM.

**Tech:** Python · PyTorch · scikit-learn · PCA · Grad-CAM · OpenCV
**Code:** [github.com/JinClaudius/PneumonIA](https://github.com/JinClaudius/PneumonIA)

---

### VerifDoc — AI document analysis API

Personal project in progress.

A FastAPI-based API designed to analyze academic certificates, detect the document type, extract key information and identify simple anomalies using structured JSON outputs and LLM-oriented prompting.

**Tech:** Python · FastAPI · LLM · JSON · Git

---

### Travel Order Resolver — NLP / Information extraction

Academic NLP project focused on interpreting French travel requests.

The goal is to extract departure and destination locations, detect invalid requests, handle ambiguous formulations and prepare route search logic using SNCF data.

**Tech:** Python · NLP · Entity extraction · SNCF data · Evaluation metrics

---


### Internal tools & automation

During my apprenticeship at SUPINFO Paris, I worked on several internal tools and automation workflows:

* Educational planning automation with **Excel/VBA**
* Document generation with **Word, Excel and PowerShell**
* SQL Server database analysis and exploitation
* Internal tools using **C#/WPF**, **React**, **Node.js** and **PostgreSQL**
* Technical documentation and process reliability improvement
* Teaching C and C++ programming to 2nd and 3rd-year students

---

## Tech stack

### AI & Data

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square\&logo=python\&logoColor=white)
![LLM](https://img.shields.io/badge/LLM-111827?style=flat-square)
![RAG](https://img.shields.io/badge/RAG-2563EB?style=flat-square)
![NLP](https://img.shields.io/badge/NLP-1D4ED8?style=flat-square)
![pandas](https://img.shields.io/badge/pandas-150458?style=flat-square\&logo=pandas\&logoColor=white)
![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white)

### Backend & APIs

![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square\&logo=fastapi\&logoColor=white)
![Node.js](https://img.shields.io/badge/Node.js-339933?style=flat-square\&logo=node.js\&logoColor=white)
![Express](https://img.shields.io/badge/Express-000000?style=flat-square\&logo=express\&logoColor=white)
![C Sharp](https://img.shields.io/badge/C%23-512BD4?style=flat-square\&logo=csharp\&logoColor=white)
![WPF](https://img.shields.io/badge/WPF-512BD4?style=flat-square)

### Frontend

![React](https://img.shields.io/badge/React-61DAFB?style=flat-square\&logo=react\&logoColor=111827)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square\&logo=typescript\&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square\&logo=javascript\&logoColor=111827)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat-square\&logo=html5\&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat-square\&logo=css3\&logoColor=white)

### Databases & tools

![SQL Server](https://img.shields.io/badge/SQL%20Server-CC2927?style=flat-square\&logo=microsoftsqlserver\&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square\&logo=postgresql\&logoColor=white)
![Supabase](https://img.shields.io/badge/Supabase-3FCF8E?style=flat-square\&logo=supabase\&logoColor=111827)
![Git](https://img.shields.io/badge/Git-F05032?style=flat-square\&logo=git\&logoColor=white)
![GitHub](https://img.shields.io/badge/GitHub-181717?style=flat-square\&logo=github\&logoColor=white)
![Postman](https://img.shields.io/badge/Postman-FF6C37?style=flat-square\&logo=postman\&logoColor=white)
![PowerShell](https://img.shields.io/badge/PowerShell-5391FE?style=flat-square\&logo=powershell\&logoColor=white)

---

## Contact

* Email: **[gouttierjean@gmail.com](mailto:gouttierjean@gmail.com)**
* Portfolio: [portfolio-gouttier-jean.vercel.app](https://portfolio-gouttier-jean.vercel.app/)
* LinkedIn: [linkedin.com/in/jeangouttier](https://linkedin.com/in/jeangouttier)

---

<p align="center">
Thanks for visiting my GitHub profile.
</p>
