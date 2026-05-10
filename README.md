<div align="center">
  <img src="./assets/banner.svg" width="100%" alt="Aaron TAO – AI Engineer & Full-Stack Builder" />
</div>

<p align="center">
  <a href="https://github.com/HAONANTAO">
    <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=28&pause=2500&color=A371F7&center=true&vCenter=true&width=620&height=48&lines=AI+Fullstack+Developer" alt="AI Fullstack Developer" />
  </a>
</p>

<p align="center">
  <a href="https://www.aarontao.com/"><img src="https://img.shields.io/badge/Portfolio-000?style=flat&logo=vercel&logoColor=white" /></a>
  <a href="https://raw.githubusercontent.com/HAONANTAO/HAONANTAO/main/resume.pdf"><img src="https://img.shields.io/badge/Resume-PDF-blue?style=flat&logo=adobeacrobatreader&logoColor=white" /></a>
  <a href="https://www.linkedin.com/in/haonan-tao-aaron/"><img src="https://img.shields.io/badge/LinkedIn-0077b5?style=flat&logo=linkedin&logoColor=white" /></a>
  <a href="mailto:taoaaron5@gmail.com"><img src="https://img.shields.io/badge/Gmail-D14836?style=flat&logo=gmail&logoColor=white" /></a>
</p>

<p align="center">
  <sub><i>Open to AI engineering & full-stack roles · Melbourne or remote across Australia · Australian PR · PMP-certified</i></sub>
</p>

<div align="center"><img src="./assets/divider.svg" width="100%" alt="" /></div>

<h2 align="center">DocuMind</h2>

<p align="center">
  <i>Multi-tenant RAG SaaS — upload a PDF, ask questions, get streamed answers with inline citations.</i><br/>
  <sub>Built on <b>TypeScript</b> · <b>Pinecone</b> vector store · <b>OpenAI</b> embeddings + streaming completions.</sub>
</p>

<p align="center">
  <a href="https://docu-mind-neon.vercel.app">
    <img src="https://raw.githubusercontent.com/HAONANTAO/DocuMind/main/DocuMind.png" width="640" alt="DocuMind – AI Document Q&A" />
  </a>
</p>

<p align="center">
  <a href="https://docu-mind-neon.vercel.app"><img src="https://img.shields.io/badge/Live%20Demo-000000?style=for-the-badge&logo=vercel&logoColor=white" /></a>
  <a href="https://github.com/HAONANTAO/DocuMind"><img src="https://img.shields.io/badge/Source-181717?style=for-the-badge&logo=github&logoColor=white" /></a>
</p>

<details>
<summary align="center"><sub><i>&nbsp;&nbsp;architecture &nbsp;·&nbsp; click to expand&nbsp;&nbsp;</i></sub></summary>

```mermaid
flowchart LR
    PDF[PDF Upload] --> CHUNK[Chunk]
    CHUNK --> EMBED[Embed]
    EMBED --> VS[(Pinecone)]
    Q[User Query] --> QE[Embed]
    QE --> VS
    VS --> CTX[Top-k Context]
    CTX --> LLM[OpenAI<br/>streaming]
    LLM --> OUT[Cited Answer]

    classDef store fill:#a371f7,stroke:#6e40c9,color:#fff;
    classDef io fill:#161b22,stroke:#30363d,color:#e6edf3;
    classDef llm fill:#412991,stroke:#412991,color:#fff;
    class VS store;
    class PDF,Q,OUT io;
    class LLM llm;
```

</details>

<h2 align="center">JD Analyzer</h2>

<p align="center">
  <i>Chrome extension that scores your resume against any job description.</i><br/>
  <sub>Live on the Chrome Web Store · BYO OpenAI key, zero backend — all inference runs against the user's own key.</sub>
</p>

<p align="center">
  <a href="https://chromewebstore.google.com/detail/ohoogdbggeapnlmhlimpffomihldkcba">
    <img src="https://img.shields.io/badge/Install-Chrome%20Web%20Store-4285F4?style=for-the-badge&logo=googlechrome&logoColor=white" alt="Install from Chrome Web Store" />
  </a>
</p>

<p align="center">
  <sub><i>Full archive on <a href="https://www.aarontao.com/"><b>aarontao.com</b></a> · all repos on <a href="https://github.com/HAONANTAO?tab=repositories"><b>GitHub</b></a></i></sub>
</p>

<br/>

<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/HAONANTAO/HAONANTAO/output/github-snake-dark.svg" />
    <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/HAONANTAO/HAONANTAO/output/github-snake.svg" />
    <img alt="GitHub contribution snake" src="https://raw.githubusercontent.com/HAONANTAO/HAONANTAO/output/github-snake.svg" />
  </picture>
</p>

<p align="center">
  <sub><i>Aaron Tao &nbsp;·&nbsp; Melbourne 🇦🇺</i></sub>
</p>
