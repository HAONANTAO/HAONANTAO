<div align="center">
  <img src="./assets/banner.svg" width="100%" alt="Aaron TAO – AI Engineer & Full-Stack Builder" />
</div>

<p align="center">
  <a href="https://www.aarontao.com/"><img src="https://img.shields.io/badge/Portfolio-000?style=flat&logo=vercel&logoColor=white" /></a>
  <a href="https://raw.githubusercontent.com/HAONANTAO/HAONANTAO/main/2025.09.11Resume.pdf"><img src="https://img.shields.io/badge/Resume-PDF-blue?style=flat&logo=adobeacrobatreader&logoColor=white" /></a>
  <a href="https://www.linkedin.com/in/haonan-tao-aaron/"><img src="https://img.shields.io/badge/LinkedIn-0077b5?style=flat&logo=linkedin&logoColor=white" /></a>
  <a href="mailto:taoaaron5@gmail.com"><img src="https://img.shields.io/badge/Gmail-D14836?style=flat&logo=gmail&logoColor=white" /></a>
  <a href="https://github.com/HAONANTAO"><img src="https://img.shields.io/github/followers/HAONANTAO?style=flat&logo=github&label=Followers&color=181717&logoColor=white" /></a>
</p>

> 📬 **Open to AI Engineer roles** in Melbourne or remote across Australia.
> Reach me at **taoaaron5@gmail.com** — I usually reply within a day.

<div align="center"><img src="./assets/divider.svg" width="100%" alt="" /></div>

<h2 align="center">👋 whoami</h2>

**I build AI systems that ship — not demos.**

I'm Aaron, an AI Engineer in Melbourne 🇦🇺. **Monash CS · University of Melbourne IT · Australian PR.**
6+ production projects shipped — including [DocuMind](https://docu-mind-neon.vercel.app) (RAG SaaS) and an iOS app live on the App Store.

These days I'm obsessed with **multi-tenant RAG**, **streaming UX**, and **agent loops that don't hallucinate**.

Currently building **[SkillPath](https://github.com/HAONANTAO/skillpath)** — an AI Learning Coach with agent-driven roadmaps and adaptive quizzes.

<div align="center"><img src="./assets/divider.svg" width="100%" alt="" /></div>

<h2 align="center">🧭 How I build</h2>

- **Ship beats demo.** A v1 in production teaches more than a v3 in slides.
- **Numbers over adjectives.** "Fast" means nothing; `<400ms p95` does.
- **Architecture before code.** I draw the system before writing the first line.
- **AI-augmented, human-verified.** I lean on Claude Code daily, but I read every line that ships.

<div align="center"><img src="./assets/divider.svg" width="100%" alt="" /></div>

<h2 align="center">🛠 Tech Stack</h2>

<p align="center">
  <img src="https://skillicons.dev/icons?i=python,typescript,react,nextjs,nodejs,mongodb,aws,docker&theme=dark" />
</p>

<p align="center">
  <sub><b>MODELS</b></sub>&nbsp;
  <img src="https://img.shields.io/badge/Claude-c96442?style=flat-square&labelColor=0d1117" />
  <img src="https://img.shields.io/badge/GPT--4o-412991?style=flat-square&logo=openai&logoColor=white&labelColor=0d1117" />
  &nbsp;·&nbsp;
  <sub><b>AI STACK</b></sub>&nbsp;
  <img src="https://img.shields.io/badge/LangChain-1C3C3C?style=flat-square&logo=langchain&logoColor=white&labelColor=0d1117" />
  <img src="https://img.shields.io/badge/RAG-6366f1?style=flat-square&labelColor=0d1117" />
  <img src="https://img.shields.io/badge/Pinecone-6d28d9?style=flat-square&labelColor=0d1117" />
  <img src="https://img.shields.io/badge/SSE-0ea5e9?style=flat-square&labelColor=0d1117" />
</p>

<div align="center"><img src="./assets/divider.svg" width="100%" alt="" /></div>

<h2 align="center">💻 Featured Project</h2>

**🤖 [DocuMind](https://docu-mind-neon.vercel.app)** &nbsp;[![DocuMind](https://img.shields.io/badge/-DocuMind-8e44ad?style=flat-square&logo=github&logoColor=white)](https://github.com/HAONANTAO/DocuMind)
AI-powered document Q&A SaaS — upload a PDF, ask questions, get answers with source citations using RAG.

### Architecture

```mermaid
flowchart LR
    User([👤 User]) -- question --> API[Express API]
    PDF([📄 PDF upload]) --> Indexer[Async Indexer]
    Indexer -- chunk + embed --> Pinecone[(Pinecone<br/>per-user namespace)]
    API -- retrieve top-k --> Pinecone
    API -- prompt + context --> LLM[GPT-4o-mini]
    LLM -- token stream --> SSE{{SSE channel}}
    SSE -- live tokens --> User
    API <--> Mongo[(MongoDB<br/>JWT-scoped)]
```

**Highlights**
🔹 RAG pipeline: chunk → embed → vector search → GPT-4o-mini generation
🔹 Streaming responses via Server-Sent Events (token-by-token)
🔹 Multi-turn memory across last 6 exchanges
🔹 Per-user vector isolation with Pinecone namespaces
🔹 Async background indexing with startup cleanup for orphaned documents

**⚡ Key Engineering Challenges**
🔸 SSE protocol edge case — once HTTP headers are sent, normal error responses are impossible. Solved by detecting `res.headersSent` and pushing LLM crash errors down the open stream so the frontend never hangs mid-response
🔸 Multi-tenancy isolation at two layers: MongoDB queries filter by JWT-extracted `userId` (never user-supplied), Pinecone vectors isolated per-user namespace — delete is atomic (MongoDB first, Pinecone in try-catch) to prevent orphaned vectors on DB failure

**Tech:** React 19, Node.js/Express 5, MongoDB, Pinecone, OpenAI GPT-4o-mini, LangChain, Vercel/Render

<img src="https://raw.githubusercontent.com/HAONANTAO/DocuMind/main/DocuMind.png" width="600" alt="DocuMind – AI Document Q&A" />

<div align="center"><img src="./assets/divider.svg" width="100%" alt="" /></div>

<h2 align="center">🚀 More Work</h2>

<p align="center">
  A curated slice — full archive on <a href="https://www.aarontao.com/">aarontao.com</a>
</p>

<table align="center">
  <tr>
    <td valign="top" width="50%">
      <h3>🤖 <a href="https://github.com/HAONANTAO/ai-customer-support-system">ai-customer-support-system</a></h3>
      <p>LangChain-powered customer support agent in TypeScript.</p>
      <a href="https://github.com/HAONANTAO/ai-customer-support-system"><img src="https://img.shields.io/github/last-commit/HAONANTAO/ai-customer-support-system?style=flat-square&label=last%20commit&color=58a6ff&labelColor=0d1117" /></a>
      <a href="https://github.com/HAONANTAO/ai-customer-support-system"><img src="https://img.shields.io/github/languages/top/HAONANTAO/ai-customer-support-system?style=flat-square&color=a371f7&labelColor=0d1117" /></a>
    </td>
    <td valign="top" width="50%">
      <h3>📱 <a href="https://github.com/HAONANTAO/Money_Recorder">Money Recorder</a></h3>
      <p>Personal finance iOS app — React Native + Expo, live on the App Store.</p>
      <a href="https://github.com/HAONANTAO/Money_Recorder"><img src="https://img.shields.io/github/last-commit/HAONANTAO/Money_Recorder?style=flat-square&label=last%20commit&color=58a6ff&labelColor=0d1117" /></a>
      <img src="https://img.shields.io/badge/iOS-App%20Store-000?style=flat-square&logo=apple&logoColor=white&labelColor=0d1117" />
    </td>
  </tr>
</table>

<p align="center">
  <a href="https://github.com/HAONANTAO?tab=repositories"><img src="https://img.shields.io/badge/View%20All%20Repos-181717?style=for-the-badge&logo=github&logoColor=white" /></a>
  <a href="https://www.aarontao.com/"><img src="https://img.shields.io/badge/aarontao.com-Full%20Portfolio-000000?style=for-the-badge&logo=vercel&logoColor=white" /></a>
</p>

<div align="center"><img src="./assets/divider.svg" width="100%" alt="" /></div>

<h2 align="center">🐍 Coding Trail</h2>

<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/HAONANTAO/HAONANTAO/output/github-snake-dark.svg" />
    <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/HAONANTAO/HAONANTAO/output/github-snake.svg" />
    <img alt="GitHub contribution snake" src="https://raw.githubusercontent.com/HAONANTAO/HAONANTAO/output/github-snake.svg" />
  </picture>
</p>

<p align="center">
  <code>$ aaron --status=shipping --location=melbourne --version=2026</code>
</p>

<p align="center">
  <sub><a href="https://www.aarontao.com/">aarontao.com</a> · <a href="mailto:taoaaron5@gmail.com">taoaaron5@gmail.com</a></sub>
</p>
