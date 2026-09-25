<img src="https://user-images.githubusercontent.com/74038190/225813708-98b745f2-7d22-48cf-9150-083f1b00d6c9.gif" alt="Header Animation">

<h1 align="center">Hi, I'm Abhinav Shakya 👋</h1>
<h3 align="center">AI/ML Engineer · Agentic AI · RAG · Computer Vision</h3>

<p align="center">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=22&pause=1000&color=38BDF8&center=true&vCenter=true&width=800&lines=Multi-agent+systems+with+guardrails;RAG+%26+ranking+pipelines;Computer+vision+that+ships" alt="Typing SVG" />
</p>

<p align="center">
  <a href="mailto:abhinavshakya063@gmail.com"><img src="https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white" /></a>
  <a href="https://www.linkedin.com/in/abhinav-shakya-a6ab28244"><img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" /></a>
  <a href="https://huggingface.co/Abhii2005"><img src="https://img.shields.io/badge/Hugging%20Face-FFD21E?style=for-the-badge&logo=huggingface&logoColor=black" /></a>
  <a href="https://github.com/abhinav-123457"><img src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white" /></a>
</p>

---

## 🧑‍💻 About Me

```python
abhinav = {
    "education"  : "B.Tech CSE (AI & ML), SRM Institute of Science and Technology — graduating May 2027",
    "location"   : "Delhi-NCR, India",
    "focus"      : ["Agentic AI systems", "RAG + retrieval pipelines", "Computer vision"],
    "experience" : ["AI/ML Intern @ Extion Infotech", "Edge AI / Drone work @ Canopy Puffs"],
    "looking_for": "AI Engineer / ML Engineer / LLM Engineer internships and roles",
}
```

I like building **complete systems**, not notebooks: data in, model or agent in the middle, a working app at the end.

---

## 🚀 Featured Projects

### 💸 AI Revenue Recovery Agent — Agentic AI for a B2B fintech

- Finds revenue that is slipping away: **abandoned checkouts, failed subscription/mandate charges, overdue B2B invoices, degraded payment routes.**
- **4 specialist LLM agents** diagnose *why* each event happened using a ReAct loop with **read-only tools** (the LLM can look things up, never act).
- Every action passes a **policy gate → independent critic agent → human review** (if flagged) before anything can move money.
- **Real payment execution:** creates actual Cashfree sandbox payment links, and an HMAC-verified webhook updates the ledger when a real payment lands.
- Next.js dashboard shows a recovery ledger and a full decision trace for every event. Every step is audited.

`LangGraph` `FastAPI` `Next.js` `TypeScript` `Gemini` `Cashfree API`
&nbsp;→ [Repo](https://github.com/abhinav-123457/Revenue_Recovery_Agent)

---

### 🎯 Quiet Disasters Ranker — Candidate ranking for 100K profiles
**Redrob AI Candidate Ranking Hackathon · Team Quiet Disasters**

- Ranks **100,000 candidates** for a Senior AI Engineer role and returns the top 100 with written reasoning for each pick.
- **Two-phase design:** heavy precompute runs offline (Kaggle), fast ranking runs locally.
- **Retrieval:** `BAAI/bge-small-en-v1.5` bi-encoder + FAISS for search, then `ms-marco-MiniLM-L-12-v2` cross-encoder to re-rank.
- **Scoring:** 7 weighted features — domain evidence, retrieval expertise, production deployment, vector DB experience, LLM-adjacent work, career progression, availability.
- Built-in **honeypot detection** and output validation.

`Python` `FAISS` `Sentence-Transformers` `Streamlit` `Hugging Face Spaces`
&nbsp;→ [Repo](https://github.com/abhinav-123457/quiet-disasters-ranker) · [Live demo](https://huggingface.co/spaces/Abhii2005/Quiet-Disasters-Ranker)

---

### 🔐 Enterprise RAG Assistant — Secure RAG with access control
**Enterprise RAG Intelligence Challenge**

- Answers questions across mixed company data: **PDFs, SQL/CSV tables, and JSON logs.**
- **Hybrid search:** dense (FAISS) + keyword (BM25), merged with Reciprocal Rank Fusion, then re-ranked by a cross-encoder.
- **Role-based access control** (department + clearance level) filters documents **before** the LLM sees them.
- Grounded answers with inline citations, a confidence score, refusal when the user isn't allowed or the data isn't there, and an audit trail.
- Runs fully on free tools: Groq for generation, local sentence-transformers for embeddings.

`Python` `FAISS` `BM25` `Sentence-Transformers` `Groq` `Streamlit`
&nbsp;→ [Repo](https://github.com/abhinav-123457/Interprise_RAG_Intelligence_Challange) · [Live demo](https://huggingface.co/spaces/Abhii2005/Interprise_RAG_Intelligence_Challange)

---

### 🪙 BTC Trading Env — RL environment for trading agents
**Grand Finalist · Meta PyTorch OpenEnv Hackathon**

- OpenEnv-compatible environment where an **LLM or RL agent acts as a Bitcoin portfolio manager.**
- **Market simulator:** price moves with market regimes (calm → volatile → crash → recovery) plus random flash crashes.
- **Matching engine** with bid-ask spread, slippage, and maker/taker fees.
- Agent sees prices, portfolio state, and indicators (SMA, RSI, MACD, volatility).
- **3 graded tasks** (easy → hard), scored on return, drawdown, and Sharpe ratio.
- Served over **HTTP and WebSocket** (FastAPI), packaged with Docker on Hugging Face Spaces.

`Python` `FastAPI` `OpenEnv` `Docker` `Reinforcement Learning`
&nbsp;→ [Repo](https://github.com/abhinav-123457/btc-trading-env)

---

### 🚨 Nexus — Crisis coordination app

- Takes an emergency from **SOS report to resolution**: guests raise an SOS, AI classifies type and severity, staff are auto-assigned, admins watch it live.
- **Role-based access** (Guest / Staff / Admin), dispatch queue, and retry queue for failed actions.
- **Works when the network doesn't:** offline queue with auto-sync, plus SLA watchdogs that escalate if no one is assigned or acknowledges in time.
- Staff push notifications through a **Cloudflare Worker relay** — runs fully on free tier.

`Flutter` `Dart` `Firebase Auth` `Firestore` `FCM` `Cloudflare Workers` `Gemini`
&nbsp;→ [Repo](https://github.com/abhinav-123457/Nexus)

---

## 🧩 More Builds

| Project | What it does | Stack |
|---|---|---|
| [**Weather Wiplash**](https://github.com/abhinav-123457/Weather_Wiplash) | F1 tyre predictor | Python |
| [**JARVIS**](https://github.com/abhinav-123457/Jarvis) | Telegram assistant + quant analyst: live market data, web research, voice notes, image reading, reminders, scheduled daily messages | n8n, Groq (Llama 3.3, Whisper), Notion, Yahoo Finance, Jina AI |
| [**InternHunt**](https://github.com/abhinav-123457/Internship-Hunt) · [live](https://intern-hunt-rwr4.vercel.app) | ATS resume scorer, internship matching, cover letter generator, and AI career chat for students | Next.js, TypeScript |
| [**POLLUX**](https://github.com/abhinav-123457/Pollux) | Multilingual AI guide to Indian elections with offline support *(Google Cloud hackathon)* | React, TypeScript, Gemini, Firebase |
| [**VenueIQ**](https://github.com/abhinav-123457/Venue-IQ) | Stadium crowd-density maps and AI wayfinding for large venues | Next.js, TypeScript, Gemini, Google Maps |


<details>
<summary><b>📁 Early projects</b></summary>
<br>

| Project | What it does | Stack |
|---|---|---|
| [**Cover Letter Generator**](https://github.com/abhinav-123457/infosys-coverletter) | Resume-aware cover letters matched to a job description | React, TypeScript, Vite |
| [**CYPHER**](https://github.com/abhinav-123457/CYPHER) | Coding chatbot with Google sign-in and code highlighting | React, Gemini API, Firebase |
| [**Diabetes Prediction**](https://github.com/abhinav-123457/Diabetes-Prediction-System) | Predicts diabetes risk from health data (Pima dataset) | scikit-learn, Flask |
| [**Sentiment Analysis Tool**](https://github.com/abhinav-123457/Sentiment-Analysis-Tool) | Classifies text as positive/negative with Naive Bayes | Python, NLTK |
| [**Stable Diffusion Image Generator**](https://github.com/abhinav-123457/stable-diffusion-image-generator) | Text-to-image generation with Stable Diffusion | PyTorch, Diffusers |

</details>

---

## 🛠️ Tech Stack

**Languages**
<p>
  <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" />
  <img src="https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white" />
  <img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black" />
  <img src="https://img.shields.io/badge/Dart-0175C2?style=for-the-badge&logo=dart&logoColor=white" />
</p>

**ML, LLMs & Agents**
<p>
  <img src="https://img.shields.io/badge/PyTorch-EE4C2C?style=for-the-badge&logo=pytorch&logoColor=white" />
  <img src="https://img.shields.io/badge/LangGraph-1C3C3C?style=for-the-badge&logo=langchain&logoColor=white" />
  <img src="https://img.shields.io/badge/Hugging%20Face-FFD21E?style=for-the-badge&logo=huggingface&logoColor=black" />
  <img src="https://img.shields.io/badge/FAISS-0467DF?style=for-the-badge&logo=meta&logoColor=white" />
  <img src="https://img.shields.io/badge/Ultralytics%20YOLO-111F68?style=for-the-badge&logo=ultralytics&logoColor=white" />
  <img src="https://img.shields.io/badge/OpenCV-5C3EE8?style=for-the-badge&logo=opencv&logoColor=white" />
  <img src="https://img.shields.io/badge/scikit--learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white" />
  <img src="https://img.shields.io/badge/Gemini-8E75B2?style=for-the-badge&logo=googlegemini&logoColor=white" />
  <img src="https://img.shields.io/badge/Groq-F55036?style=for-the-badge&logoColor=white" />
  <img src="https://img.shields.io/badge/n8n-EA4B71?style=for-the-badge&logo=n8n&logoColor=white" />
</p>

**Backend & Frontend**
<p>
  <img src="https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white" />
  <img src="https://img.shields.io/badge/Flask-000000?style=for-the-badge&logo=flask&logoColor=white" />
  <img src="https://img.shields.io/badge/Next.js-000000?style=for-the-badge&logo=nextdotjs&logoColor=white" />
  <img src="https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB" />
  <img src="https://img.shields.io/badge/Flutter-02569B?style=for-the-badge&logo=flutter&logoColor=white" />
  <img src="https://img.shields.io/badge/Streamlit-FF4B4B?style=for-the-badge&logo=streamlit&logoColor=white" />
</p>

**Cloud & Tools**
<p>
  <img src="https://img.shields.io/badge/Firebase-FFCA28?style=for-the-badge&logo=firebase&logoColor=black" />
  <img src="https://img.shields.io/badge/Cloudflare%20Workers-F38020?style=for-the-badge&logo=cloudflare&logoColor=white" />
  <img src="https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white" />
  <img src="https://img.shields.io/badge/Vercel-000000?style=for-the-badge&logo=vercel&logoColor=white" />
  <img src="https://img.shields.io/badge/Kaggle-20BEFF?style=for-the-badge&logo=kaggle&logoColor=white" />
  <img src="https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white" />
</p>

---

## 🏆 Hackathons

- 🥇 **Grand Finalist** — Meta PyTorch OpenEnv Hackathon (BTC Trading Env)
- **Redrob AI Candidate Ranking Hackathon** — Quiet Disasters Ranker
- **Enterprise RAG Intelligence Challenge** — Enterprise RAG Assistant
- **Google Cloud Hackathon** — POLLUX

---

## 📊 GitHub Stats

<p align="center">
  <img src="https://streak-stats.demolab.com?user=abhinav-123457&theme=tokyonight&hide_border=true" height="160"/>
</p>

---

<p align="center"><b>Open to AI/ML internships and collaborations — reach out on email or LinkedIn.</b></p>
