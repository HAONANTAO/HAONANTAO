<div align="center">
  <img src="./assets/banner.svg" width="100%" alt="Aaron TAO – Full-Stack Developer & AI Builder" />
</div>

<div align="center">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&pause=1000&center=true&vCenter=true&width=500&lines=AI+Agent+%7C+RAG+%7C+LangChain+%7C" alt="Typing SVG" />
</div>


<p align="center">
  <a href="https://github.com/HAONANTAO"><img src="https://img.shields.io/badge/GitHub-000?style=flat&logo=github&logoColor=white" /></a>
  <a href="https://www.aarontao.com/"><img src="https://img.shields.io/badge/Portfolio-000?style=flat&logo=vercel&logoColor=white" /></a>
 <a href="https://raw.githubusercontent.com/HAONANTAO/HAONANTAO/main/2025.09.11Resume.pdf"><img src="https://img.shields.io/badge/Resume-PDF-blue?style=flat&logo=adobeacrobatreader&logoColor=white" /></a>
  <a href="https://www.linkedin.com/in/haonan-tao-aaron/"><img src="https://img.shields.io/badge/-LinkedIn-0077b5?style=flat&logo=linkedin&logoColor=white" /></a>
  <a href="mailto:taoaaron5@gmail.com"><img src="https://img.shields.io/badge/Gmail-D14836?style=flat&logo=gmail&logoColor=white" /></a>
</p>

<h2 align="center">
  💼 <strong>About Me</strong>
</h2>

<p align="center" style="font-size:16px; line-height:1.8; max-width:640px; margin:auto;">
🧠 I build production AI apps — RAG pipelines, LLM integrations, and full-stack platforms shipped from zero to live users.<br/>
🚀 Published iOS app on the App Store — 6+ full-stack projects in production — Currently building an <strong>AI Agent</strong> project<br/>
🔥 Deeply passionate about AI: exploring autonomous agents, tool use, and what LLMs can actually do in production<br/>
🎓 Monash University CS — University of Melbourne IT<br/>
🇦🇺 Australian PR — Open to Full-Time roles in Melbourne
</p>


<h3 align="center">Tech Stack</h3>
<p align="center">
  <img src="https://skillicons.dev/icons?i=react,nextjs,nodejs,express,mongodb,typescript,tailwind,aws,docker,git,github,figma&theme=dark" />
</p>

<h3 align="center">AI & Tools</h3>
<p align="center">
  <img src="https://img.shields.io/badge/OpenAI-412991?style=flat-square&logo=openai&logoColor=white" />
  <img src="https://img.shields.io/badge/LangChain-1C3C3C?style=flat-square&logo=langchain&logoColor=white" />
  <img src="https://img.shields.io/badge/RAG-6366f1?style=flat-square&logoColor=white" />
  <img src="https://img.shields.io/badge/AI%20Agent-0ea5e9?style=flat-square&logoColor=white" />
  <img src="https://img.shields.io/badge/Pinecone-000000?style=flat-square&logoColor=white" />
  <img src="https://img.shields.io/badge/React%20Native-20232A?style=flat-square&logo=react&logoColor=61DAFB" />
  <img src="https://img.shields.io/badge/Vercel-000000?style=flat-square&logo=vercel&logoColor=white" />
</p>

---

## 💻 Latest Projects

---
**🤖 [DocuMind](https://docu-mind-neon.vercel.app)** [![DocuMind](https://img.shields.io/badge/-DocuMind-8e44ad?style=flat-square&logo=github&logoColor=white)](https://github.com/HAONANTAO/DocuMind)  
An AI-powered document Q&A SaaS — upload a PDF, ask questions, get answers with source citations using RAG.

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

**🗄️ [AllStorage](https://github.com/HAONANTAO/AllStorage)** [![AllStorage](https://img.shields.io/badge/-AllStorage-3498db?style=flat-square&logo=github&logoColor=white)](https://github.com/HAONANTAO/AllStorage)  
A cloud-based file storage platform with real-time sync and role-based access control.  

**Highlights:**  
🔹 Independently implemented file upload & sharing  
🔹 Designed folder structure & large file handling  
🔹 Maximum single file upload: >2GB  
🔹 Real-time sync latency: <1s on average  
🔹 Successfully tested with 100+ files by friends/internal users  

**Tech:** Next.js (App Router), TypeScript, TailwindCSS, Appwrite, AWS S3, Clerk  

<img src="https://raw.githubusercontent.com/HAONANTAO/AllStorage/main/Demo1.png" width="480" alt="AllStorage Dashboard" /> 
<img src="https://raw.githubusercontent.com/HAONANTAO/AllStorage/main/Features3.png" width="480" alt="AllStorage Dashboard 3" />

---

**💰 [Money Recorder](https://apps.apple.com/us/app/moneyrecorder/id6744058988)** [![MoneyRecorder](https://img.shields.io/badge/-MoneyRecorder-1abc9c?style=flat-square&logo=github&logoColor=white)](https://github.com/HAONANTAO/Money_Recorder)  
A personal finance management iOS app for tracking expenses, managing budgets, and visualizing analytics.

**Highlights:**  
🔹 Track expenses/income, manage budgets, and visualize analytics
🔹 Real-time sync & offline mode, bilingual UI (English/Chinese)
🔹 Successfully tested with 10+ users
🔹 Handles >500 transactions per user without lag
🔹 Average screen load time <2s

**Tech:** React Native, Expo, NativeWind, Appwrite, Chart Kit, AsyncStorage  

<img src="https://raw.githubusercontent.com/HAONANTAO/Money_Recorder/main/assets/Demo1.jpg" width="220" alt="Money Recorder – Home" />
<img src="https://raw.githubusercontent.com/HAONANTAO/Money_Recorder/main/assets/Demo2.jpg" width="220" alt="Money Recorder – Analytics" />

---

**🛒 [E-Commerce Rabbit](https://www.wanyancanrui.com/)** [![E-Commerce](https://img.shields.io/badge/-E--Commerce-1abc9c?style=flat-square&logo=github&logoColor=white)](https://github.com/HAONANTAO/E-Commerce-Rabbit)  
Independently developed, production-ready full-stack MERN e-commerce platform with secure transactions and real-time features.

**Highlights:**  
🔹 Dynamic product catalog & real-time shopping cart
🔹 Secure JWT authentication & PayPal payment integration
🔹 Handles >100 concurrent users with smooth performance
🔹 Successfully processed 200+ orders in internal testing
🔹 Average page load: <1.2s

**Tech:** React, Redux Toolkit, Tailwind CSS, Express, MongoDB, Cloudinary, PayPal API, Vercel/AWS  

<img src="https://raw.githubusercontent.com/HAONANTAO/E-Commerce-Rabbit/main/ScreenShow.png" width="600" alt="E-Commerce Rabbit – Dashboard" />

---

<p align="center">
  🔗 Check my <a href="https://www.aarontao.com/">Portfolio</a> for more production-ready apps & projects!
</p>

<h2 align="center">📊 GitHub Stats</h2>

<p align="center">
  <img src="https://streak-stats.demolab.com?user=HAONANTAO&theme=radical&date_format=j%20M%5B%20Y%5D" alt="GitHub Streak" />
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
