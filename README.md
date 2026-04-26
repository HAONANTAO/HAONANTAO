<div align="center">
  <img src="./assets/banner.svg" width="100%" alt="Aaron TAO – AI Engineer & Full-Stack Builder" />
</div>

<div align="center">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&pause=1200&color=58A6FF&center=true&vCenter=true&width=560&height=45&lines=AI+Engineer+%26+Full-Stack+Developer;RAG+Pipelines+%C2%B7+LLM+Agents+%C2%B7+LangChain;DocuMind+%C2%B7+SkillPath+%C2%B7+iOS+App+Store;Melbourne+%C2%B7+Open+to+Full-Time+Roles" alt="Typing SVG" />
</div>

<p align="center">
  <a href="https://www.aarontao.com/"><img src="https://img.shields.io/badge/Portfolio-000?style=flat&logo=vercel&logoColor=white" /></a>
  <a href="https://raw.githubusercontent.com/HAONANTAO/HAONANTAO/main/2025.09.11Resume.pdf"><img src="https://img.shields.io/badge/Resume-PDF-blue?style=flat&logo=adobeacrobatreader&logoColor=white" /></a>
  <a href="https://www.linkedin.com/in/haonan-tao-aaron/"><img src="https://img.shields.io/badge/LinkedIn-0077b5?style=flat&logo=linkedin&logoColor=white" /></a>
  <a href="mailto:taoaaron5@gmail.com"><img src="https://img.shields.io/badge/Gmail-D14836?style=flat&logo=gmail&logoColor=white" /></a>
  <img src="https://komarev.com/ghpvc/?username=HAONANTAO&color=blueviolet&style=flat&label=Profile+Views" />
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Open%20to%20Full--Time%20Roles-Melbourne%20%F0%9F%87%A6%F0%9F%87%BA-0ea5e9?style=flat" />
</p>

---

<div align="center">
  <img src="./assets/terminal.svg" width="100%" alt="About Aaron TAO" />
</div>

---

<h2 align="center">Tech Stack & AI Tools</h2>

<p align="center">
  <img src="https://skillicons.dev/icons?i=react,nextjs,nodejs,express,mongodb,typescript,tailwind,python,aws,docker,git,figma&theme=dark" />
</p>

<p align="center">
  <img src="https://img.shields.io/badge/React%20Native-20232A?style=flat-square&logo=react&logoColor=61DAFB" />
  <img src="https://img.shields.io/badge/Expo-000020?style=flat-square&logo=expo&logoColor=white" />
  <img src="https://img.shields.io/badge/App%20Store-0D96F6?style=flat-square&logo=apple&logoColor=white" />
</p>

<p align="center">
  <img src="https://img.shields.io/badge/OpenAI-412991?style=flat-square&logo=openai&logoColor=white" />
  <img src="https://img.shields.io/badge/Anthropic%20Claude-c96442?style=flat-square&logoColor=white" />
  <img src="https://img.shields.io/badge/LangChain-1C3C3C?style=flat-square&logo=langchain&logoColor=white" />
  <img src="https://img.shields.io/badge/RAG-6366f1?style=flat-square&logoColor=white" />
  <img src="https://img.shields.io/badge/AI%20Agent-0ea5e9?style=flat-square&logoColor=white" />
  <img src="https://img.shields.io/badge/Pinecone-6d28d9?style=flat-square&logoColor=white" />
  <img src="https://img.shields.io/badge/Vercel-000000?style=flat-square&logo=vercel&logoColor=white" />
</p>

---

<h2 align="center">🚧 Currently Building</h2>

<p align="center">
  <img src="https://img.shields.io/badge/SkillPath-In%20Progress-f59e0b?style=flat-square" />
</p>

**📚 SkillPath** — AI-powered personalized learning platform. Building in public — watch this space.

---

<h2 align="center">💻 Featured Project</h2>

**🤖 [DocuMind](https://docu-mind-neon.vercel.app)** &nbsp;[![DocuMind](https://img.shields.io/badge/-DocuMind-8e44ad?style=flat-square&logo=github&logoColor=white)](https://github.com/HAONANTAO/DocuMind)  
AI-powered document Q&A SaaS — upload a PDF, ask questions, get answers with source citations using RAG.

**Highlights:**  
🔹 RAG pipeline: chunk → embed → vector search → GPT-4o-mini generation  
🔹 Streaming responses via Server-Sent Events (token-by-token)  
🔹 Multi-turn memory across last 6 exchanges  
🔹 Per-user vector isolation with Pinecone namespaces  
🔹 Async background indexing with startup cleanup for orphaned documents  

**⚡ Key Engineering Challenges:**  
🔸 SSE protocol edge case — once HTTP headers are sent, normal error responses are impossible. Solved by detecting `res.headersSent` and pushing LLM crash errors down the open stream so the frontend never hangs mid-response  
🔸 Multi-tenancy isolation at two layers: MongoDB queries filter by JWT-extracted `userId` (never user-supplied), Pinecone vectors isolated per-user namespace — delete is atomic (MongoDB first, Pinecone in try-catch) to prevent orphaned vectors on DB failure  

**Tech:** React 19, Node.js/Express 5, MongoDB, Pinecone, OpenAI GPT-4o-mini, LangChain, Vercel/Render

<img src="https://raw.githubusercontent.com/HAONANTAO/DocuMind/main/DocuMind.png" width="600" alt="DocuMind – AI Document Q&A" />

---

<h2 align="center">🌐 Portfolio</h2>

<p align="center">
  All production projects — full-stack apps, iOS apps, and more:
</p>

<p align="center">
  <a href="https://www.aarontao.com/">
    <img src="https://img.shields.io/badge/aarontao.com-View%20Full%20Portfolio-000000?style=for-the-badge&logo=vercel&logoColor=white" />
  </a>
</p>

---

<h2 align="center">📊 GitHub Stats</h2>

<p align="center">
  <img height="165" src="https://github-readme-stats.vercel.app/api?username=HAONANTAO&show_icons=true&theme=radical&hide_border=true&count_private=true" alt="GitHub Stats" />
  <img height="165" src="https://github-readme-stats.vercel.app/api/top-langs/?username=HAONANTAO&layout=compact&theme=radical&hide_border=true" alt="Top Languages" />
</p>

<p align="center">
  <img src="https://streak-stats.demolab.com?user=HAONANTAO&theme=radical&hide_border=true&date_format=j%20M%5B%20Y%5D" alt="GitHub Streak" />
</p>

<p align="center">
  <img src="https://github-profile-trophy.vercel.app/?username=HAONANTAO&theme=radical&no-frame=true&no-bg=true&margin-w=4&row=1" alt="GitHub Trophies" />
</p>

<p align="center">
  <img src="https://github-readme-activity-graph.vercel.app/graph?username=HAONANTAO&theme=dracula&hide_border=true&area=true" alt="Activity Graph" />
</p>

<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/HAONANTAO/HAONANTAO/output/github-snake-dark.svg" />
    <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/HAONANTAO/HAONANTAO/output/github-snake.svg" />
    <img alt="GitHub contribution snake" src="https://raw.githubusercontent.com/HAONANTAO/HAONANTAO/output/github-snake.svg" />
  </picture>
</p>

<div align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=6,11,20&height=100&section=footer" />
</div>
