<div align="center">

```
██████╗ ██╗  ██╗ █████╗ ███╗   ██╗ █████╗ ███████╗██╗  ██╗██████╗ ███████╗███████╗
██╔══██╗██║  ██║██╔══██╗████╗  ██║██╔══██╗██╔════╝██║  ██║██╔══██╗██╔════╝██╔════╝
██║  ██║███████║███████║██╔██╗ ██║███████║███████╗███████║██████╔╝█████╗  █████╗  
██║  ██║██╔══██║██╔══██║██║╚██╗██║██╔══██║╚════██║██╔══██║██╔══██╗██╔══╝  ██╔══╝  
██████╔╝██║  ██║██║  ██║██║ ╚████║██║  ██║███████║██║  ██║██║  ██║███████╗███████╗
╚═════╝ ╚═╝  ╚═╝╚═╝  ╚═╝╚═╝  ╚═══╝╚═╝  ╚═╝╚══════╝╚═╝  ╚═╝╚═╝  ╚═╝╚══════╝╚══════╝
```

### *I translate human language into machine language. Fluently.*

[![Portfolio](https://img.shields.io/badge/Portfolio-000000?style=for-the-badge&logo=vercel&logoColor=white)](https://portfoliodhanashree.vercel.app/)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/dhanashree2311)
[![Medium](https://img.shields.io/badge/Medium-12100E?style=for-the-badge&logo=medium&logoColor=white)](https://medium.com/@dhanashreebansode416)
[![ISRO](https://img.shields.io/badge/Ex--ISRO_Intern-FF6B00?style=for-the-badge&logoColor=white)](#)
[![Best Paper](https://img.shields.io/badge/Best_Paper-ICRETETM_2024-gold?style=for-the-badge)](#)

</div>

---

<div align="center">

## `whoami`

</div>

```python
class Dhanashree:
    def __init__(self):
        self.name        = "Dhanashree Bansode"
        self.role        = "AI/ML Engineer (Graduating 2026)"
        self.location    = "Pune, India"
        self.gpa         = "8.95 / 10"
        self.ex          = ["ISRO-ISTRAC"]          # yes, THE space agency
        self.awards      = ["Best Paper — ICRETETM 2024"]
        self.shipped     = ["ISRO pipeline", "Smart AI Inbox", "TradeGuard", "Nyay AI"]
        self.philosophy  = "What works outside the notebook, not what looks good on a confusion matrix"

    def integrity_check(self) -> str:
        # Found a data leakage bug inflating accuracy by 20 points.
        # Reported it anyway.
        return "ship honest systems"

    def translate(self, human_problem: str) -> str:
        return "deployed AI that solves it 🚀"
```

---

## 🛰️ What I've Built

> Not side projects. **Deployed systems.** Real data, real users, real constraints.

---

### 🔴 ISRO-ISTRAC — Machine Learning Intern `Jan 2026 – Apr 2026`

**Spurious signal detection in Wind Profiler Radar IQ data.**
27,047 labeled samples. 3-stage pipeline. India's space programme.

```
Stage 1 → Spike Masking          (DC removal via mean subtraction + EMD)
Stage 2 → Narrowband Detection   (Doppler interpolation for vertical spike correction)
Stage 3 → Isolation Forest       (configurable contamination, horizontal RFI removal)
```

Shipped a Flask web app with real-time parameter tuning, beam-wise visualization, and cleaned `.dat` file export.
Letter of Recommendation from the **Deputy Director, ISRO-ISTRAC.**

---

### 📬 Smart AI Inbox — 4-Model ML Pipeline `[ Demo · Backend · Frontend ]`
`Python · FastAPI · XGBoost · Sentence-Transformers · Supabase/pgvector · React · Tailwind · Docker`

Production Gmail AI assistant. Every email scored 0-100. Surfaces what actually needs action.

| Model | Job |
|-------|-----|
| XGBoost importance scorer | Prioritises emails with surgical precision |
| Random Forest classifier | Labels with ensemble confidence |
| NER deadline extractor | Pulls dates out of email soup |
| K-Means clustering | Groups your inbox chaos into sense |

**The engineering details that matter:**
- Replaced 17 handcrafted keyword features with **384-dim sentence-transformer embeddings** (R² = 0.72 on 1,854 real emails)
- Weak supervision pipeline labeling **2,163 Enron emails** using 9 labeling functions
- 3-layer spam detection: Gmail category labels + List-Unsubscribe header + emoji rule
- Real-time XGBoost retraining on in-app user corrections
- Full Google OAuth2 web flow, Supabase session persistence, pgvector semantic search
- Found a 20-point accuracy inflation from data leakage. **Reported it honestly.**

---

### ⚖️ TradeGuard AI — Multi-Agent Compliance Monitor `[ Demo · GitHub ]`
`Python · FastAPI · React · Groq API (LLaMA 3.3 70B) · SQLite · SQLAlchemy`

3-agent LLM pipeline that catches financial crime and generates formal compliance reports.

```
Transaction Analyst → Compliance Mapper → Report Writer
```

**The engineering details that matter:**
- Per-agent `max_tokens` optimisation cut token consumption **63%** (6,000 → 2,200 tokens/pipeline)
- Cross-transaction fraud detection across **±5-min reversal windows** and **±60-sec same-IP windows**
- Human-in-the-loop as an **architectural constraint** — no auto-approve endpoint exists (by design)
- Exponential backoff retry (20s/40s/60s) + intermediate DB persistence so partial results survive agent failures

---

### 🎙️ Nyay AI — FIR in Your Language `[ Demo · GitHub ]`
`Python · FastAPI · React · Groq API (LLaMA 3.3 70B) · PostgreSQL · Vercel · Render`

**Because justice shouldn't require fluent English.**

Walk into a police station. Speak in Hindi, English, or Hinglish.
Nyay AI transcribes, identifies the right IPC sections, and files your FIR.

**The engineering details that matter:**
- Auto-identifies **14+ IPC sections** with confidence scoring from unstructured speech
- Reduced FIR filing time by **~80%**
- Fixed a silent multi-turn bug: replaced `str(result)` with `json.dumps(result, ensure_ascii=False)` in conversation history serialisation — injected explicit DB-extracted state into each LLM turn
- Language-enforcement fallback: Devanagari detection via Unicode regex + secondary Groq translation call when the model ignores English-mode instruction

---

### 🧪 Hinglish ML Tutor — LoRA Fine-Tuned LLM `[ Demo · GitHub ]`
`Unsloth · LoRA · LLaMA 3.2-1B-Instruct · HuggingFace · Google Colab T4`

Fine-tuned LLaMA 3.2-1B on **164 hand-crafted Hinglish + Marathlish ML Q&A pairs.**
Training loss: 2.5 → 1.0 in 100 steps. Free Colab T4. ~20 minutes. Zero cost.
Model is **live and public on Hugging Face.**

---

## 🧠 Stack

<div align="center">

**Gen AI & LLMs**

![LLaMA](https://img.shields.io/badge/LLaMA_3.x-black?style=flat-square)
![LoRA](https://img.shields.io/badge/LoRA_Fine--tuning-black?style=flat-square)
![Groq](https://img.shields.io/badge/Groq_API-F55036?style=flat-square)
![RAG](https://img.shields.io/badge/RAG-black?style=flat-square)
![pgvector](https://img.shields.io/badge/pgvector-336791?style=flat-square)
![HuggingFace](https://img.shields.io/badge/HuggingFace-FFD21E?style=flat-square&logoColor=black)

**ML**

![XGBoost](https://img.shields.io/badge/XGBoost-black?style=flat-square)
![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=flat-square)
![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square)
![Isolation Forest](https://img.shields.io/badge/Isolation_Forest-black?style=flat-square)
![K--Means](https://img.shields.io/badge/K--Means-black?style=flat-square)

**Backend & Deploy**

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square)
![Supabase](https://img.shields.io/badge/Supabase-3ECF8E?style=flat-square)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square)
![Vercel](https://img.shields.io/badge/Vercel-000000?style=flat-square)

</div>

---

## 📊 GitHub Stats

<div align="center">

![Dhanashree's GitHub Stats](https://github-readme-stats.vercel.app/api?username=dhanashree23112003&show_icons=true&theme=radical&hide_border=true&bg_color=0d1117&title_color=FF6B00&icon_color=FF6B00&text_color=ffffff)

![Top Languages](https://github-readme-stats.vercel.app/api/top-langs/?username=dhanashree23112003&layout=compact&theme=radical&hide_border=true&bg_color=0d1117&title_color=FF6B00&text_color=ffffff)

</div>

---

<div align="center">

## Open to Work

Actively looking for **junior AI/ML engineering roles.**
I ship deployed systems, I debug honestly, and I care about what the thing actually does in production.

[![LinkedIn](https://img.shields.io/badge/Let's_Talk-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/dhanashree2311)
[![Email](https://img.shields.io/badge/Email_Me-EA4335?style=for-the-badge&logo=gmail&logoColor=white)](mailto:dhanashree.professional@gmail.com)

---

*"I translate our language to machine's language using computer programming."*

*She means it.*

</div>
