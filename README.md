<h1 align="center">Nitin Kanojiya</h1>

<p align="center">
  <strong>Full-Stack Developer · Backend and AI Applications · Competitive Programmer</strong>
</p>

<p align="center">
  I build practical software with a focus on backend engineering, AI-powered applications, and clean problem solving.
</p>

<p align="center">
  <a href="https://www.linkedin.com/in/nitinkanojiya/"><img src="https://img.shields.io/badge/LinkedIn-Nitin%20Kanojiya-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn" /></a>
  <a href="https://leetcode.com/u/Nitin__26/"><img src="https://img.shields.io/badge/LeetCode-Nitin__26-FFA116?style=for-the-badge&logo=leetcode&logoColor=white" alt="LeetCode" /></a>
  <a href="https://codeforces.com/profile/Nitin__26"><img src="https://img.shields.io/badge/Codeforces-Nitin__26-1F8ACB?style=for-the-badge&logo=codeforces&logoColor=white" alt="Codeforces" /></a>
  <a href="mailto:kanojiyanitin870@gmail.com"><img src="https://img.shields.io/badge/Email-Contact-D14836?style=for-the-badge&logo=gmail&logoColor=white" alt="Email" /></a>
</p>

---

## About

- Computer science student building real, deployable software with Java, TypeScript, and Python
- Strong on backend work: REST APIs, authentication and security, and database design
- Builds AI features into applications, including LLM-powered classification, summarization, and review tools
- Problem solver with a DSA-first approach: 750+ LeetCode problems solved and a 1700+ contest rating
- Based in Gujarat, India

---

## Featured Projects

### 1. [Codexium](https://github.com/Nitin-kanojiya26/Coding-platform)

A competitive programming platform that pairs DSA practice and live contests with **Build Mode**, where learners create and test working REST APIs.

- **Build Mode:** runs learner-built Node.js/Express APIs in Docker-isolated containers and evaluates them with automated HTTP tests
- **Resilient code execution:** uses a self-hosted Judge0 instance as the primary DSA execution engine, with OnlineCompiler.io as an automatic fallback when the primary engine is unavailable
- **Real-time contests:** broadcasts submission verdicts and standings through Socket.IO; the project README reports a 100-user load test where Redis, BullMQ, and sockets improved leaderboard P95 from 12.6 seconds to 271 ms

[Repository](https://github.com/Nitin-kanojiya26/Coding-platform) · [Live demo](https://coding-platform-kohl-alpha.vercel.app)

> **Execution setup:** Judge0 is self-hosted and can run on a local machine. When the deployed backend needs to reach a Judge0 instance running on your PC, expose it through a secure tunnel such as ngrok; if Judge0 is offline or errors, the configured OnlineCompiler.io fallback can handle submissions. Build Mode uses a separate Docker worker, which can connect outbound to the cloud queue without port forwarding.

---

### 2. [GitPR](https://github.com/Nitin-kanojiya26/GitPR)

An AI pull request reviewer built as a GitHub App. It analyzes pull request changes, retrieves relevant team style-guide rules, and posts contextual inline review comments.

- Verifies signed GitHub webhooks and maps diffs to per-file changed-line ranges for valid inline comments
- Uses retrieval-augmented generation (RAG) to find relevant style-guide rules and ground review feedback in team conventions
- Validates structured LLM output, filters comments outside the diff, and processes work with a queue, idempotent webhook handling, and retries

<p>
  <img src="https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white" alt="TypeScript" />
  <img src="https://img.shields.io/badge/Node.js-339933?style=flat-square&logo=nodedotjs&logoColor=white" alt="Node.js" />
  <img src="https://img.shields.io/badge/GitHub_Apps-181717?style=flat-square&logo=github&logoColor=white" alt="GitHub Apps" />
  <img src="https://img.shields.io/badge/Google_Gemini-4285F4?style=flat-square&logo=google&logoColor=white" alt="Google Gemini" />
  <img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white" alt="PostgreSQL" />
  <img src="https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white" alt="Redis" />
</p>

[Repository](https://github.com/Nitin-kanojiya26/GitPR)

---

### 3. [AI Expense Tracker](https://github.com/Nitin-kanojiya26/expense-tracker-ai)

A full-stack personal finance application with AI-powered expense classification and analytics.

- Classifies transactions with an LLM and supports conversational questions about spending
- Includes rolling analytics, dynamic categories, input validation, and transactional persistence
- Secured with JWT authentication, built on a Spring Boot REST API with a React client and PostgreSQL

<p>
  <img src="https://img.shields.io/badge/Java-ED8B00?style=flat-square&logo=openjdk&logoColor=white" alt="Java" />
  <img src="https://img.shields.io/badge/Spring_Boot-6DB33F?style=flat-square&logo=springboot&logoColor=white" alt="Spring Boot" />
  <img src="https://img.shields.io/badge/React-20232A?style=flat-square&logo=react&logoColor=61DAFB" alt="React" />
  <img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white" alt="PostgreSQL" />
</p>

[Repository](https://github.com/Nitin-kanojiya26/expense-tracker-ai)

---

### 4. [ClassPluse](https://github.com/Nitin-kanojiya26/ClassPluse)

A classroom attendance system that combines rotating QR codes with face verification, course management, and attendance reporting.

- Faculty can run live sessions with a QR image refreshed every 15 seconds; students scan the current code and verify their identity against a face registered to their account
- Uses **FaceRecognitionDotNet** with Dlib models for face encodings and matching, and **QRCoder** to generate QR images; a high-confidence match refreshes the stored face encoding
- Provides attendance history, live class counts, faculty adjustments, spreadsheet exports, and automatic marking of unrecorded students as absent after a session

[Repository](https://github.com/Nitin-kanojiya26/ClassPluse)

> **Note:** the live-session page refreshes its QR image every 15 seconds, but the backend currently reuses tokens for local testing and gives newly generated tokens a one-day expiry. The server-side token expiry is therefore not currently 15 seconds.

---

### More Projects

| Project | Description | Stack |
|---|---|---|
| [SmartDoc](https://github.com/Nitin-kanojiya26/SmartDoc) | AI-powered document learning app. Summarizes PDFs and answers questions about them with Google Gemini, with Firebase sync and local indexing. | Flutter, Dart, Firebase, Gemini |
| [Portfolio](https://github.com/Nitin-kanojiya26/portfolio) | Interactive developer portfolio with animated UI, a WebGL globe, and a responsive layout. | Next.js, TypeScript, Tailwind CSS, Framer Motion |

---

## Tech Stack

| Area | Technologies |
|---|---|
| **Languages** | Java, C++, Python, JavaScript, TypeScript, SQL |
| **Backend** | Spring Boot, Spring Security, Hibernate, Node.js, REST APIs, JWT |
| **Frontend and mobile** | React, Next.js, Flutter |
| **Databases** | PostgreSQL, MySQL, MongoDB, Redis, Firebase |
| **DevOps and tools** | Docker, AWS, Git, GitHub, GitHub Actions |
| **AI** | LLM integration (Gemini), retrieval-augmented generation, structured output validation |

<p>
  <img src="https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white" alt="Java" />
  <img src="https://img.shields.io/badge/C%2B%2B-00599C?style=for-the-badge&logo=cplusplus&logoColor=white" alt="C++" />
  <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" alt="Python" />
  <img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black" alt="JavaScript" />
  <img src="https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white" alt="TypeScript" />
  <img src="https://img.shields.io/badge/Spring_Boot-6DB33F?style=for-the-badge&logo=springboot&logoColor=white" alt="Spring Boot" />
  <img src="https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB" alt="React" />
  <img src="https://img.shields.io/badge/Next.js-000000?style=for-the-badge&logo=nextdotjs&logoColor=white" alt="Next.js" />
  <img src="https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=nodedotjs&logoColor=white" alt="Node.js" />
  <img src="https://img.shields.io/badge/Flutter-02569B?style=for-the-badge&logo=flutter&logoColor=white" alt="Flutter" />
  <img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white" alt="PostgreSQL" />
  <img src="https://img.shields.io/badge/Redis-DC382D?style=for-the-badge&logo=redis&logoColor=white" alt="Redis" />
  <img src="https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white" alt="Docker" />
  <img src="https://img.shields.io/badge/AWS-232F3E?style=for-the-badge&logo=amazonaws&logoColor=white" alt="AWS" />
</p>

---

## Currently Learning

- Production-grade Spring Boot architecture, Spring Security, and REST API design
- Reliable AI application design: evaluation, retrieval quality, and LLM output validation
- Docker, AWS, CI/CD, and scalable cloud deployment
- System design: caching, queues, and distributed systems
- Advanced data structures, algorithms, and competitive programming techniques

---

## Competitive Programming

- **LeetCode:** 750+ problems solved, 1700+ contest rating
- **Codeforces:** active participant

<p align="center">
  <img src="https://leetcard.jacoblin.cool/Nitin__26?theme=dark&font=Karma&ext=heatmap" alt="LeetCode stats and submission heatmap" />
</p>

<p align="center">
  <img src="https://codeforces-readme-stats.vercel.app/api/card?username=Nitin__26&theme=dark" alt="Codeforces stats" />
</p>

---

## GitHub Stats

<p align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=Nitin-kanojiya26&show_icons=true&theme=dark&hide_border=true" alt="GitHub stats" />
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=Nitin-kanojiya26&layout=compact&theme=dark&hide_border=true" alt="Top languages" />
</p>

---

## Contact

I'm open to internships, collaborations, and conversations about backend and AI engineering.

<p>
  <a href="https://github.com/Nitin-kanojiya26"><img src="https://img.shields.io/badge/GitHub-Nitin--kanojiya26-181717?style=for-the-badge&logo=github&logoColor=white" alt="GitHub" /></a>
  <a href="https://www.linkedin.com/in/nitinkanojiya/"><img src="https://img.shields.io/badge/LinkedIn-Nitin%20Kanojiya-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn" /></a>
  <a href="mailto:kanojiyanitin870@gmail.com"><img src="https://img.shields.io/badge/Email-kanojiyanitin870%40gmail.com-D14836?style=for-the-badge&logo=gmail&logoColor=white" alt="Email" /></a>
</p>
