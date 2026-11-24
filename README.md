<div align="center">
<img src="https://readme-typing-svg.herokuapp.com?font=JetBrains+Mono&weight=700&size=26&pause=1000&color=58A6FF&center=true&vCenter=true&random=false&width=750&height=50&lines=Jo%C3%A3o+Henrique+Miranda+Mendon%C3%A7a;AI+Engineer+%C2%B7+LLM+Agents+in+Production;LangGraph+%C2%B7+RAG+%C2%B7+Python+%C2%B7+FastAPI;17k%2B+conversations%2Fmonth+handled+by+my+agents" alt="Typing SVG" />
<p>
  <a href="https://www.linkedin.com/in/joao-henrique-mirandamendonca-70b052322/"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn" /></a>
  <a href="mailto:jaohenrique732@gmail.com"><img src="https://img.shields.io/badge/Email-EA4335?style=for-the-badge&logo=gmail&logoColor=white" alt="Email" /></a>
  <img src="https://img.shields.io/badge/Ribeir%C3%A3o_Preto%2C_Brazil-009C3B?style=for-the-badge&logo=googlemaps&logoColor=white" alt="Location" />
</p>
</div>
<hr/>
<h2>👋 About me</h2>
 
<p>
I'm an <b>AI Engineer</b> at <b>Dryve (Finx Capital)</b> and a <b>Software Engineering</b> student at UNAERP.
I build and maintain <b>LLM-powered conversational agents that run in production</b> on WhatsApp — from agent architecture
in <b>LangGraph</b> to RAG, CRM integrations, automated tests and deployment.
</p>
<p>
I work data-first: I use metrics and real conversations to decide what to improve next, and I validate every delivery with automated tests.
</p>
```python
joao = {
    "role": "AI Engineer @ Dryve (Finx Capital)",
    "since": "Sep 2025",
    "education": "B.Sc. Software Engineering @ UNAERP",
    "focus": ["LLM agents", "RAG", "Backend (Python/FastAPI)", "Automation (n8n)"],
    "languages": ["Portuguese (native)", "English (advanced)", "Spanish (basic)"],
}
```
 
<h2>📊 Impact at a glance</h2>
 
<table>
  <tr>
    <td align="center" width="25%"><h3>17k+</h3>conversations / month handled by agents I migrated</td>
    <td align="center" width="25%"><h3>n8n → LangGraph</h3>led the migration of WhatsApp agents to Python</td>
    <td align="center" width="25%"><h3>56% → 0</h3>flow failure eliminated by moving business rules into code</td>
    <td align="center" width="25%"><h3>End-to-end</h3>collections agent built from scratch (OCR + CRM)</td>
  </tr>
</table>
<h2>🧠 How I design agents</h2>
 
<p>Agents are built as <b>state graphs</b>: an LLM router sends each message to the right step of the conversation, and each step has its own prompt and tools. Critical business rules live in code, not in the prompt.</p>
```mermaid
flowchart LR
    U([WhatsApp message]) --> R{LLM Router}
    R --> A[Step: qualification]
    R --> B[Step: pricing]
    R --> C[Step: FAQ]
    A --> G[Guardrails & validation in code]
    B --> G
    C --> K[(RAG · PostgreSQL + pgvector)]
    K --> G
    G --> T[Tool calling · CRM · external APIs]
    T --> O([Reply to customer])
```
 
<h2>🔥 What I build</h2>
 
<table>
  <tr>
    <td width="50%" valign="top">
      <h3>🤖 Production LLM agents</h3>
      <p>WhatsApp customer-service agents in <b>Python + LangGraph</b>: LLM routing, per-step prompts, tool calling and guardrails. They collect and validate data, answer questions, quote prices and resume conversations automatically.</p>
    </td>
    <td width="50%" valign="top">
      <h3>💸 Collections agent</h3>
      <p>Built from scratch: negotiates payment dates, validates payment receipts with <b>OCR</b> and updates the <b>CRM</b> automatically.</p>
    </td>
  </tr>
  <tr>
    <td width="50%" valign="top">
      <h3>🔎 RAG & semantic search</h3>
      <p>Semantic search with <b>PostgreSQL + pgvector</b> to answer frequently asked questions, with the knowledge base versioned through <b>Alembic</b> migrations.</p>
    </td>
    <td width="50%" valign="top">
      <h3>🧪 Testing & quality</h3>
      <p>Automated tests that run against a <b>real LLM using production conversations</b>, plus data audits to prioritize the next fixes. I also review the team's pull requests.</p>
    </td>
  </tr>
  <tr>
    <td width="50%" valign="top">
      <h3>⚡ Automation & integrations</h3>
      <p><b>n8n</b> workflows integrated with CRM, external APIs and <b>WhatsApp Flows</b> (forms and scheduling).</p>
    </td>
    <td width="50%" valign="top">
      <h3>🚢 Shipping to production</h3>
      <p>Containerized services with <b>Docker</b>, deployed through <b>CI/CD</b> (Bitbucket Pipelines, Argo CD), with messaging over <b>RabbitMQ</b>.</p>
    </td>
  </tr>
</table>
<h2>🛠️ Tech stack</h2>
 
<p><b>AI & LLMs</b><br/>
  <img src="https://img.shields.io/badge/LangGraph-1C3C3C?style=for-the-badge&logo=langchain&logoColor=white" alt="LangGraph" />
  <img src="https://img.shields.io/badge/LangChain-1C3C3C?style=for-the-badge&logo=langchain&logoColor=white" alt="LangChain" />
  <img src="https://img.shields.io/badge/OpenAI-412991?style=for-the-badge&logo=openai&logoColor=white" alt="OpenAI" />
  <img src="https://img.shields.io/badge/RAG_%26_Embeddings-58A6FF?style=for-the-badge" alt="RAG" />
  <img src="https://img.shields.io/badge/Tool_Calling-6E40C9?style=for-the-badge" alt="Tool calling" />
  <img src="https://img.shields.io/badge/OCR-555555?style=for-the-badge" alt="OCR" />
</p>
<p><b>Backend</b><br/>
  <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" alt="Python" />
  <img src="https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white" alt="FastAPI" />
  <img src="https://img.shields.io/badge/SQLAlchemy-D71F00?style=for-the-badge&logo=sqlalchemy&logoColor=white" alt="SQLAlchemy" />
  <img src="https://img.shields.io/badge/RabbitMQ-FF6600?style=for-the-badge&logo=rabbitmq&logoColor=white" alt="RabbitMQ" />
  <img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black" alt="JavaScript" />
</p>
<p><b>Data & Infra</b><br/>
  <img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white" alt="PostgreSQL" />
  <img src="https://img.shields.io/badge/pgvector-336791?style=for-the-badge&logo=postgresql&logoColor=white" alt="pgvector" />
  <img src="https://img.shields.io/badge/Alembic-6BA81E?style=for-the-badge" alt="Alembic" />
  <img src="https://img.shields.io/badge/Supabase-3FCF8E?style=for-the-badge&logo=supabase&logoColor=white" alt="Supabase" />
  <img src="https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white" alt="Docker" />
  <img src="https://img.shields.io/badge/Argo_CD-EF7B4D?style=for-the-badge&logo=argo&logoColor=white" alt="Argo CD" />
  <img src="https://img.shields.io/badge/Bitbucket_Pipelines-0052CC?style=for-the-badge&logo=bitbucket&logoColor=white" alt="Bitbucket Pipelines" />
</p>
<p><b>Automation & Integrations</b><br/>
  <img src="https://img.shields.io/badge/n8n-EA4B71?style=for-the-badge&logo=n8n&logoColor=white" alt="n8n" />
  <img src="https://img.shields.io/badge/WhatsApp_Business_API-25D366?style=for-the-badge&logo=whatsapp&logoColor=white" alt="WhatsApp Business API" />
  <img src="https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white" alt="Git" />
  <img src="https://img.shields.io/badge/Azure_DevOps-0078D7?style=for-the-badge&logo=azuredevops&logoColor=white" alt="Azure DevOps" />
</p>
<p><b>Also exploring</b><br/>
  <img src="https://img.shields.io/badge/Kotlin-7F52FF?style=for-the-badge&logo=kotlin&logoColor=white" alt="Kotlin" />
  <img src="https://img.shields.io/badge/Spring_Boot-6DB33F?style=for-the-badge&logo=springboot&logoColor=white" alt="Spring Boot" />
</p>
<h2>🎓 Education & certifications</h2>
 
<ul>
  <li><b>B.Sc. Software Engineering</b> — UNAERP, Brazil (2026 – 2028)</li>
  <li><b>Computer Engineering</b> — UNAERP, Brazil (2023 – 2026)</li>
  <li>Certifications: LGPD (Brazilian Data Protection Law) · Information Security · Artificial Intelligence</li>
</ul>
<div align="center">
<img src="https://capsule-render.vercel.app/api?type=waving&color=58A6FF&height=90&section=footer&text=Let's%20build%20something%20smart&fontSize=20&fontColor=ffffff&fontAlignY=65" width="100%" alt="footer" />
</div>
 
