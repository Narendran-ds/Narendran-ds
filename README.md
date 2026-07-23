<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0f0c29,50:302b63,100:24243e&height=280&section=header&text=Narendran%20L&fontSize=60&fontColor=C9A9FF&animation=fadeIn&fontAlignY=38&desc=Backend%20%26%20AI%20Engineer%20%7C%20Java%20%2B%20Python&descAlignY=58&descSize=18" width="100%"/>

<a href="https://git.io/typing-svg">
  <img src="https://readme-typing-svg.demolab.com/?font=Fira+Code&size=24&duration=3000&pause=1000&color=B39DDB&center=true&vCenter=true&width=650&lines=Java+%2B+Spring+Boot+%2B+PostgreSQL;Computer+Vision+%2B+LLM+Pipelines;Final+Year+B.Tech+AI+%26+Data+Science;Open+to+Backend+%2F+AI+Engineer+Roles" alt="Typing SVG" />
</a>

<br/>

![Academic](https://img.shields.io/badge/B.Tech-AI%20%26%20Data%20Science-6A0DAD?style=flat-square&logo=googlescholar&logoColor=white)
![University](https://img.shields.io/badge/Anna%20University-R2023-4B0082?style=flat-square)
![Location](https://img.shields.io/badge/Chennai%2C%20India-8A2BE2?style=flat-square&logo=googlemaps&logoColor=white)

<br/>

<a href="https://linkedin.com/in/narendran-l1125" target="_blank"><img src="https://img.shields.io/badge/LinkedIn-6D28D9?style=for-the-badge&logo=linkedin&logoColor=white"/></a>
<a href="mailto:narendranlofficial@gmail.com"><img src="https://img.shields.io/badge/Email-5B21B6?style=for-the-badge&logo=gmail&logoColor=white"/></a>
<a href="https://zipforgex.in" target="_blank"><img src="https://img.shields.io/badge/ZipForgeX-7C3AED?style=for-the-badge&logo=vercel&logoColor=white"/></a>

<br/><br/>

![Profile Views](https://komarev.com/ghpvc/?username=Narendran-ds&color=8a2be2&style=flat-square&label=PROFILE+VIEWS)
![Followers](https://img.shields.io/github/followers/Narendran-ds?style=flat-square&color=8a2be2&label=FOLLOWERS)
![Stars](https://img.shields.io/github/stars/Narendran-ds?style=flat-square&color=8a2be2&label=STARS)

</div>

<br/>

---

## About

I'm **Narendran L**, a final-year **B.Tech Artificial Intelligence & Data Science** student at Rajalakshmi Institute of Technology, Chennai.

I build and deploy complete systems rather than notebooks. Two projects represent most of my engineering work:

- **ZipForgeX** — a Spring Boot + React SaaS running in production under a custom domain, with JWT/Spring Security auth, Google and GitHub OAuth2, and PostgreSQL.
- **ChainSight** — a five-layer computer vision pipeline that turns warehouse video into auditable safety events, with a fine-tuned YOLOv8 detector and 58 passing tests.

Between them I've handled the parts that don't show up in tutorials: a production Spring Security filter chain failure, a full credential rotation after a secrets exposure, a database migration when a free tier ran out of compute, and a dataset leakage bug that would have quietly inflated my model metrics.

I care about correctness, deployment discipline, and being able to defend every number I publish.

```yaml
Working with:
  - Java, Spring Boot, Spring Security, REST APIs, PostgreSQL
  - Python, YOLOv8, Gemini API, PaddleOCR
  - React, Vite, Tailwind
  - Git, Render, Vercel, Supabase
```

**Open to:** Backend Engineer, AI/GenAI Engineer, and Software Engineer roles — graduating 2027.

---

## Tech Stack

<div align="center">

**Languages**
<br/>
<img src="https://skillicons.dev/icons?i=java,python&theme=dark"/>

**Backend & Databases**
<br/>
<img src="https://skillicons.dev/icons?i=spring,postgresql&theme=dark"/>

**Frontend**
<br/>
<img src="https://skillicons.dev/icons?i=react,vite,tailwind&theme=dark"/>

**Tooling & Deployment**
<br/>
<img src="https://skillicons.dev/icons?i=git,github,vercel,postman,vscode&theme=dark"/>

</div>

---

## Projects

<details open>
<summary><b>ZipForgeX — Full-Stack Folder-to-ZIP Platform</b></summary>
<br/>

Converts indented folder-structure text into downloadable ZIP archives. Live in production on Render + Vercel under a custom domain.

| Category | Detail |
|---|---|
| **Backend** | Spring Boot 3.5, Java 17, Maven, JUnit |
| **Frontend** | React + Vite + Tailwind v4 |
| **Auth** | JWT + Spring Security, Google OAuth2, GitHub OAuth2 |
| **Database** | PostgreSQL on Supabase |
| **Security** | Zip Slip path-traversal protection; full credential rotation after a secrets exposure incident |
| **Testing** | 12 passing JUnit tests |
| **Live** | [zipforgex.in](https://zipforgex.in) |

Notable work beyond the feature list: diagnosing a production Spring Security `addFilterBefore` overload crash, fixing a 401 on authenticated history fetches via a custom `RestAuthenticationEntryPoint`, and migrating the database from Neon to Supabase after exhausting a compute quota.

</details>

<details>
<summary><b>ChainSight — Five-Layer Warehouse Safety Pipeline</b></summary>
<br/>

Turns raw warehouse video into auditable safety events through a layered pipeline: Vision → Spatial → World Graph → Rule Engine → Narration.

| Category | Detail |
|---|---|
| **Stack** | Python, YOLOv8, Shapely/STRtree, NetworkX, Gemini Flash, Streamlit |
| **Detector** | Fine-tuned YOLOv8 on a merged 17-class, 13,731-image dataset |
| **Metrics** | mAP@50 = 0.7678 (exit-zone markers: AP@50 = 0.8892) |
| **Rule Engine** | Deterministic rules R1–R5, each event carrying explicit trigger, evidence, and conclusion |
| **Testing** | 58 passing tests |
| **Deployment** | Live on Streamlit Community Cloud |
| **Repository** | [github.com/Narendran-ds/chainsight](https://github.com/Narendran-ds/chainsight) |

The design decision I'd defend first: the narration layer uses an LLM but is constrained to *rephrase only*. It cannot introduce facts the rule engine didn't produce. Every claim in the output traces back to a deterministic rule, so the system stays auditable.

Dataset splitting was done three-way with leakage checks — an earlier naive split was inflating validation metrics.

</details>

<details>
<summary><b>AI Response Watchdog — Final-Year Project (in progress)</b></summary>
<br/>

A browser extension that watches AI chatbot responses, extracts checkable claims, and verifies each against independent sources — surfacing results through a guardian mascot that reacts to verification status.

| Category | Detail |
|---|---|
| **Status** | Early development, started July 2026 |
| **Team** | 3 people — my module is aggregation, scoring, and reason generation |
| **Approach** | Single-model multi-source aggregation with source-authority weighting |
| **Design principle** | Never claims absolute truth — only whether an independent source agrees. Biased toward "unverified" over "wrong" to minimise false positives. |

Architecture and mascot states are designed; the detection engine is being built. I'll update this section with results rather than intentions.

</details>

<details>
<summary><b>Earlier Projects</b></summary>
<br/>

- **Political Sentiment Intelligence Dashboard** — LinearSVC (78.75%) and Logistic Regression (74.56%) on a Ukraine–Russia tweet dataset, with SHAP explanations, served via Streamlit.
- **Customer Churn Prediction** — XGBoost at 89% accuracy with SHAP explainability, deployed on Streamlit.
- **English–French Neural Machine Translation** — sequence-to-sequence model in PyTorch.

</details>

---

## Experience

**AI Developer Intern** · Syncorb Geotech Pvt Ltd, Chennai
`Oct 2025 — May 2026`

Built production AI pipelines for BizOp Analytica, a client-facing analytics product.

- Designed a Gemini API pipeline generating 500+ global cuisines and up to 500 dishes per cuisine, replacing a manual BeautifulSoup/Scrapy workflow — with history tracking so completed entries are skipped on reruns, cutting redundant API calls.
- Rebuilt the restaurant menu extraction pipeline from scratch using PaddleOCR after third-party API access was restricted, adding folder-based batch processing to turn an incomplete prototype into a working system.
- Owned prompt design, output validation, error handling, and pipeline reliability end to end.

<img src="https://img.shields.io/badge/-Gemini%20API-6D28D9?style=flat-square"/> <img src="https://img.shields.io/badge/-PaddleOCR-4C1D95?style=flat-square"/> <img src="https://img.shields.io/badge/-Python-2D1B69?style=flat-square"/>

---

## Achievements

| Recognition | Details |
|---|---|
| Cognizant Technoverse 2026 | Shortlisted to represent Rajalakshmi Institute of Technology at a national hackathon with 22,000+ participants |
| Cognizant Digital Nurture 5.0 | Cleared Rounds 1 & 2 |
| PROTOSPARK, Velammal Institute of Technology | Presented ZipForgeX in the ICT category |
| Production Deployment | ZipForgeX live across Vercel, Render, and Supabase |

---

<!--
  CERTIFICATIONS — add back only the ones you actually hold and can produce
  a verification link or credential ID for. Delete the rest.

  ## Certifications
  ![NPTEL](https://img.shields.io/badge/NPTEL-6A0DAD?style=for-the-badge&logo=googlescholar&logoColor=white)
-->

<!--
  CODING PROFILES — add back once you have real profiles with real links.
  Point them at YOUR profile URL, never the platform homepage.

  ## Coding Profiles
  [![LeetCode](https://img.shields.io/badge/LeetCode-2D1B69?style=for-the-badge&logo=leetcode&logoColor=white)](https://leetcode.com/u/YOUR_USERNAME/)
-->

## GitHub Analytics

<div align="center">
<img src="https://github-readme-stats.vercel.app/api?username=Narendran-ds&show_icons=true&theme=tokyonight&hide_border=true&bg_color=0D1117&title_color=B39DDB&icon_color=8A2BE2&text_color=C9A9FF" width="49%"/>
<img src="https://streak-stats.demolab.com?user=Narendran-ds&theme=tokyonight&hide_border=true&background=0D1117&stroke=8A2BE2&ring=B39DDB&fire=B39DDB&currStreakLabel=C9A9FF" width="49%"/>
</div>

<div align="center">
<img src="https://github-readme-stats.vercel.app/api/top-langs/?username=Narendran-ds&layout=compact&theme=tokyonight&hide_border=true&bg_color=0D1117&title_color=B39DDB&text_color=C9A9FF" width="50%"/>
</div>

---

## GitHub Trophies

<div align="center">
<img src="https://github-profile-trophy.vercel.app/?username=Narendran-ds&theme=discord&no-frame=true&column=7&margin-w=10&margin-h=10&title=Commits,Repositories,Followers,Stars,PullRequest,Issues,Experience"/>
</div>

---

## Contribution Activity

<div align="center">
<img src="https://github-readme-activity-graph.vercel.app/graph?username=Narendran-ds&theme=tokyo-night&hide_border=true&bg_color=0D1117&color=B39DDB&line=8A2BE2&point=C9A9FF"/>
</div>

---

<!--
  CONTRIBUTION SNAKE — this image only exists if you have the generator
  GitHub Action set up. If the Action isn't running, this renders broken.
  Setup: create .github/workflows/snake.yml using Platane/snk, output to
  the "output" branch. Uncomment once the Action has run successfully.

  ## Contribution Snake

  <div align="center">
  <img src="https://raw.githubusercontent.com/Narendran-ds/Narendran-ds/output/github-contribution-grid-snake-dark.svg"/>
  </div>

  ---
-->



## Currently

```yaml
building:
  - ZipForgeX v2 (AI folder generation, account management)
  - AI Response Watchdog (final-year project)
  - Portfolio site

learning:
  - Data structures & algorithms in Java
  - Backend system design

open_to:
  - Backend Engineer / Software Engineer roles
  - AI & GenAI Engineer roles
```

---

<div align="center">

[![Gmail](https://img.shields.io/badge/narendranlofficial%40gmail.com-5B21B6?style=for-the-badge&logo=gmail&logoColor=white)](mailto:narendranlofficial@gmail.com)
[![LinkedIn](https://img.shields.io/badge/narendran--l1125-6D28D9?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/narendran-l1125)

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:24243e,50:302b63,100:0f0c29&height=150&section=footer"/>

</div>
