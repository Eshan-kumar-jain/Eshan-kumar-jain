<div align="center">

# Eshan Kumar Jain

**AI Specialist & Business Data Analyst**

Agentic AI · Machine Learning · Data Analytics · Banking Systems

[![Portfolio](https://img.shields.io/badge/Portfolio-0F2B46?style=flat-square&logo=googlechrome&logoColor=white)](https://eshan-kumar-jain.github.io/My-Portfolio-Website)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=flat-square&logo=linkedin&logoColor=white)](https://linkedin.com/in/eshan-kumar-jain-a140921b6)
[![Email](https://img.shields.io/badge/Email-D14836?style=flat-square&logo=gmail&logoColor=white)](mailto:eshanjain552@gmail.com)
[![Zenodo](https://img.shields.io/badge/Published_Paper-1682D4?style=flat-square&logo=zenodo&logoColor=white)](https://zenodo.org/records/20754075)

</div>

---

I spent two years at **HDFC Bank** as a Business Data Analyst in Tech & Digital, running API
integration workstreams over ₹15 Cr+ of daily transaction value — requirement gathering, incident
triage, UAT, and the SQL analysis that found where processes were stalling.

I'm now finishing an **MSc in Data Science & Analytics at Maynooth University, Ireland** (on track
for 1st Class Honours), building LLM agents and self-supervised models. My background is a B.Tech
in Computer Science from **NIT Nagpur**.

The thread running through my work: most models that look good are measuring something other than
what you think. A 91% accuracy score on an 89/11 class split is reporting the class ratio. A 0.657
validation score can sit on top of a network that has collapsed onto the majority class. Finding
that gap — and closing it — is the part I care about.

<div align="center">

`Currently` &nbsp;·&nbsp; MSc thesis on self-supervised spectral classification &nbsp;·&nbsp; LangChain & RAG systems &nbsp;·&nbsp; Contributing to pandas & numpy-financial

</div>

---

## Featured Work

### 🔬 Ensemble of Lightweight CNNs and CLIP for Skin Disease Classification &nbsp;<sub>[`Published`](https://zenodo.org/records/20754075)</sub>

`PyTorch` `CLIP ViT-B/32` `MobileNetV2` `ShuffleNetV2` `Albumentations`

[Code](https://github.com/Eshan-kumar-jain/University-Final-year-project) · [Paper](https://zenodo.org/records/20754075)

Average ensemble across three architectures on 7-class HAM10000 dermoscopy data (10,015 images).
**Macro F1 0.6518 at 82.50% accuracy** — 8.6 points clear of the best single model.

- Adding the CLIP linear probe to a CNN-only ensemble was worth **+8.3% macro F1**, and the rare
  classes gained most — which is exactly where a screening tool carries its clinical value.
- Handled a 67% majority class through balanced class weighting and augmentation, selecting on
  macro F1 rather than accuracy throughout.
- Diagnosed VGG19's collapse onto the majority class (macro F1 0.1146 behind a 0.657 validation
  score) as batch-level metric accumulation, and rebuilt evaluation around per-class reporting.

### 🌌 Self-Supervised Region Mapping & Zero-Shot Spectral Classification &nbsp;<sub>`MSc Thesis`</sub>

`PyTorch` `CNNs` `Transformers` `Contrastive Learning`

[Code](https://github.com/Eshan-kumar-jain/Muse-data-science-Project)

Three self-supervised models trained on a 2.9 GB VLT/MUSE spectral cube — 96,093 spectra, **no
labels of any kind**. The models had to locate the jet, the diffuse gas and the point sources on
their own.

- A CLIP-style dual encoder paired each spectrum with its own image patch (1D + 2D CNNs, symmetric
  InfoNCE). Clustering those embeddings **reproduced the jet boundary astronomers draw by hand**
  from line ratios. Synthetic ARI 1.000.
- A masked-modelling transformer with a per-instrument tokenizer fused MUSE and FEROS spectra across
  a **50× resolution gap** with no resampling onto a shared grid. Synthetic ARI 0.997, leave-one-out
  accuracy 0.889.

### 💳 Credit Card Approval Risk Classifier

`Scikit-learn` `XGBoost` `FastAPI` `Streamlit`

[Live app](https://credit-risk-classifiergit.streamlit.app/) · [Code](https://github.com/Eshan-kumar-jain/Credit-risk-classifier)

Seven grid-searched classifiers reported 91% accuracy while catching **zero of 28 rejections**. The
89/11 split meant the headline number was measuring the class ratio, not the model.

- Balanced class weighting, F1 scoring in every grid search, and restoring all 16 features lifted
  **ROC-AUC 0.55 → 0.77** and rejection-class **F1 0.21 → 0.49**.
- Deployed as a FastAPI service with a Streamlit interface — shipped as a triage signal for human
  review, not an automated decision.

### 📈 WealthIQ — AI Stock Analyzer

`Claude API` `Next.js` `TypeScript` `Vercel`

[Live app](https://wealth-iq-a-stock-analyzer.vercel.app/) · [Code](https://github.com/Eshan-kumar-jain/WealthIQ-a-stock-analyzer)

Production AI agent running multi-step prompt workflows over NSE and BSE fundamentals, returning
plain-English analysis of valuation, growth, financial health and ownership.

### 🛒 Customer Shopping Behavior Analysis

`Python` `Pandas` `SQL` `Power BI`

[Code](https://github.com/Eshan-kumar-jain/Customer-trends-data-analysis-SQL-Python-PowerBI)

End-to-end analysis of 3,900 retail purchases across 18 features: cleaning and feature engineering
in pandas, SQL queries on revenue by segment, discount use and subscriber vs non-subscriber
spending, and an interactive Power BI dashboard. Customers segmented into new, returning and loyal,
with recommendations on retention and discount strategy.

---

## Open Source

| Project | Contribution | Pull request |
|---|---|---|
| **pandas** | Regression test for `read_sql` with `%` in SQLAlchemy queries, run against SQLite and PostgreSQL ([#35484](https://github.com/pandas-dev/pandas/issues/35484)) | [#69435](https://github.com/pandas-dev/pandas/pull/69435) |
| **numpy-financial** | Edge case tests for `npv` and `irr`; reported two unhandled inputs in `irr` ([#58](https://github.com/numpy/numpy-financial/issues/58)) | [#155](https://github.com/numpy/numpy-financial/pull/155) |

Write-ups of each contribution: [open-source-contributions](https://github.com/Eshan-kumar-jain/open-source-contributions)

---

## Tech Stack

**AI & LLMs**

![Claude](https://img.shields.io/badge/Claude_API-D97757?style=flat-square&logo=anthropic&logoColor=white)
![LangChain](https://img.shields.io/badge/LangChain-1C3C3C?style=flat-square&logo=langchain&logoColor=white)
![Agentic](https://img.shields.io/badge/Agentic_Workflows-6E4AFF?style=flat-square)
![Prompt Engineering](https://img.shields.io/badge/Prompt_Engineering-4A4A4A?style=flat-square)
![Groq](https://img.shields.io/badge/Groq-F55036?style=flat-square&logo=groq&logoColor=white)

**Machine Learning**

![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=flat-square&logo=scikitlearn&logoColor=white)
![XGBoost](https://img.shields.io/badge/XGBoost-337AB7?style=flat-square)
![HuggingFace](https://img.shields.io/badge/Hugging_Face-FFD21E?style=flat-square&logo=huggingface&logoColor=black)

**Data & Analytics**

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-CC2927?style=flat-square&logo=microsoftsqlserver&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=flat-square&logo=pandas&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-013243?style=flat-square&logo=numpy&logoColor=white)
![Power BI](https://img.shields.io/badge/Power_BI-F2C811?style=flat-square&logo=powerbi&logoColor=black)

**APIs & Development**

![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![Streamlit](https://img.shields.io/badge/Streamlit-FF4B4B?style=flat-square&logo=streamlit&logoColor=white)
![Next.js](https://img.shields.io/badge/Next.js-000000?style=flat-square&logo=nextdotjs&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black)

**Service Management**

![JIRA](https://img.shields.io/badge/JIRA-0052CC?style=flat-square&logo=jira&logoColor=white)
![ServiceNow](https://img.shields.io/badge/ServiceNow-62D84E?style=flat-square&logo=servicenow&logoColor=white)
![Agile](https://img.shields.io/badge/Agile_/_SDLC-1F6FEB?style=flat-square)
![UAT](https://img.shields.io/badge/UAT_&_Incident_Triage-6C757D?style=flat-square)

---

<div align="center">

<img height="160" src="https://github-readme-stats.vercel.app/api?username=Eshan-kumar-jain&show_icons=true&hide_border=true&title_color=145080&icon_color=145080&text_color=555555&bg_color=00000000&include_all_commits=true" alt="GitHub stats" />
<img height="160" src="https://github-readme-stats.vercel.app/api/top-langs/?username=Eshan-kumar-jain&layout=compact&hide_border=true&title_color=145080&text_color=555555&bg_color=00000000&langs_count=6" alt="Top languages" />

</div>

---

## Education & Credentials

| | |
|---|---|
| **MSc Data Science & Analytics** — on track for 1st Class Honours | Maynooth University, Ireland · 2025–2026 (expected) |
| **B.Tech Computer Science & Engineering** | NIT Nagpur, India · 2019–2023 |
| **Anthropic** | Claude 101 Prompt Engineering · Agent Skills · Subagents |
| **HackerRank** | SQL Certificate |
| **JEE Main 2019** | 99.57th percentile — top 0.43% of 900,000 candidates |
| **Olympiads** | Gold Medalist, International Mathematics & Science |

---

<div align="center">

Open to roles in **AI/ML Engineering**, **Data Science** and **Data/Business Analytics** — Ireland, EU & India.

[eshanjain552@gmail.com](mailto:eshanjain552@gmail.com) &nbsp;·&nbsp; [LinkedIn](https://linkedin.com/in/eshan-kumar-jain-a140921b6) &nbsp;·&nbsp; [Portfolio](https://eshan-kumar-jain.github.io/My-Portfolio-Website)

</div>
