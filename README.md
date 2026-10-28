# Hi, I'm Akira 👋

📍 São José dos Campos, Brazil | 💻 Full Stack Developer | 🚀 Open to Opportunities

Passionate about building modern, reliable, and user-focused web applications — from React front-ends to Node.js and Java / Spring Boot APIs, backed by SQL and NoSQL databases, deployed on the cloud.

## 🚀 Featured Projects

### 💰 [Life and Money](https://github.com/akiratochiro/life-and-money-api) · [web](https://github.com/akiratochiro/life-and-money-web) · [live demo](https://life-and-money-web.akira-tochiro23.workers.dev)

A personal finance app with a Java back-end and a mobile-first React front-end — categories, transactions, monthly budgets, savings goals and month-by-month analytics, with a home feed ordered by what needs attention right now.

- **Back-end:** Java 21 + Spring Boot 4.1, Spring Security as an OAuth2 Resource Server (short-lived JWT + rotating refresh token in an `HttpOnly` cookie), Spring Data JPA / Hibernate, PostgreSQL with Flyway migrations
- **Domain rules:** monthly budgets with **effective dating** (changing a budget never rewrites past months), exact money arithmetic with `BigDecimal` / `NUMERIC`, and averages computed only over closed months
- **Architecture:** package by feature with package-private repositories, dependency inversion to break a cycle between transactions and goals, domain events between features, RFC 9457 error responses
- **Front-end:** React 19 + TypeScript + Vite, TanStack Query, Tailwind CSS 4, API types generated from the OpenAPI spec, custom SVG charts
- **Tests & delivery:** JUnit 5, Mockito and Testcontainers against a real Postgres, GitHub Actions CI, Docker, deployed on Render + Neon + Cloudflare Workers

### 🗂️ [Kanbix](https://github.com/akiratochiro/kanbix) · [live demo](https://kanbix-web.vercel.app)
A full-stack Kanban project management app inspired by Trello, Jira and ClickUp — workspaces, boards, drag-and-drop cards, checklists, labels and a per-board productivity dashboard.
- **Monorepo** (npm workspaces) with shared TypeScript types between front-end and back-end
- **Front-end:** Next.js 16 (App Router), React 19, TanStack Query (optimistic updates with rollback), shadcn/ui, dnd-kit
- **Back-end:** Express 5 + Prisma + PostgreSQL in a layered architecture (routes → controllers → services → repositories), Zod validation, JWT + bcrypt, role-based access (Owner / Admin / Member), transactional reordering
- **339 tests** — API unit tests, integration tests against a real Postgres (Jest + Supertest) and React Testing Library on the front-end
- **Docker Compose**, **GitHub Actions** CI (API, web and Docker image jobs), deployed on Vercel + Render + Neon

### 🔗 [ShortYourLink](https://github.com/akiratochiro/ShortYourLink) · [live demo](https://shortyourlink.onrender.com)
A URL shortener with click analytics, built with Next.js 16, Prisma and PostgreSQL.
- Anonymous sessions, per-link daily click charts, cursor-based pagination
- Security hardening: rate limiting, SSRF guard, malicious-domain blocklist (URLhaus), CSP headers
- Jest unit + integration tests (~86% coverage) and Playwright end-to-end tests
- Sentry error tracking, health-check endpoint, multi-stage Docker build, deployed on Render + Neon

### 🧊 [In My Fridge](https://github.com/akiratochiro/In-My-Fridge) · [live demo](https://in-my-fridge-liard.vercel.app)
Suggests recipes based on the ingredients you already have. React (Vite) + Tailwind on the front-end, Node.js + Express on the back-end, which runs parallel requests to TheMealDB and intersects the results to support multi-ingredient search.

## 🔭 Currently Working On

- **Travel Planner** — a full-stack app for planning trips and managing itineraries

## 🧰 Tech Stack

**Linguagens**

![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?logo=javascript&logoColor=black)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?logo=typescript&logoColor=white)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?logo=css3&logoColor=white)
![Java](https://img.shields.io/badge/Java-ED8B00?logo=openjdk&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?logo=python&logoColor=white)


**Back-end**

![Node.js](https://img.shields.io/badge/Node.js-339933?logo=nodedotjs&logoColor=white)
![Express.js](https://img.shields.io/badge/Express.js-000000?logo=express&logoColor=white)
![NestJS](https://img.shields.io/badge/NestJS-E0234E?logo=nestjs&logoColor=white)
![Spring Boot](https://img.shields.io/badge/Spring_Boot-6DB33F?logo=springboot&logoColor=white) ![Spring Security](https://img.shields.io/badge/Spring_Security-6DB33F?logo=springsecurity&logoColor=white) ![Hibernate](https://img.shields.io/badge/Hibernate-59666C?logo=hibernate&logoColor=white) ![Maven](https://img.shields.io/badge/Maven-C71A36?logo=apachemaven&logoColor=white)

**Front-end**

![Vue.js](https://img.shields.io/badge/Vue.js-4FC08D?logo=vuedotjs&logoColor=white)
![React](https://img.shields.io/badge/React-61DAFB?logo=react&logoColor=black)
![Next.js](https://img.shields.io/badge/Next.js-000000?logo=nextdotjs&logoColor=white)
![Vite](https://img.shields.io/badge/Vite-646CFF?logo=vite&logoColor=white)
![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-06B6D4?logo=tailwindcss&logoColor=white)
![shadcn/ui](https://img.shields.io/badge/shadcn%2Fui-000000?logo=shadcnui&logoColor=white)
![TanStack Query](https://img.shields.io/badge/TanStack_Query-FF4154?logo=reactquery&logoColor=white)

**Autenticação & Validação**

![JWT](https://img.shields.io/badge/JWT-000000?logo=jsonwebtokens&logoColor=white)
![Zod](https://img.shields.io/badge/Zod-3E67B1?logo=zod&logoColor=white)

**Banco de Dados**

![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?logo=postgresql&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-4479A1?logo=mysql&logoColor=white)
![MongoDB](https://img.shields.io/badge/MongoDB-47A248?logo=mongodb&logoColor=white)
![Prisma](https://img.shields.io/badge/Prisma-2D3748?logo=prisma&logoColor=white)
![Neon](https://img.shields.io/badge/Neon-00E599?logo=postgresql&logoColor=black)
![Flyway](https://img.shields.io/badge/Flyway-CC0200?logo=flyway&logoColor=white)

**Testes**

![Jest](https://img.shields.io/badge/Jest-C21325?logo=jest&logoColor=white)
![Supertest](https://img.shields.io/badge/Supertest-343434?logo=javascript&logoColor=white)
![Testing Library](https://img.shields.io/badge/Testing_Library-E33332?logo=testinglibrary&logoColor=white)
![Playwright](https://img.shields.io/badge/Playwright-2EAD33?logo=playwright&logoColor=white)
![JUnit 5](https://img.shields.io/badge/JUnit_5-25A162?logo=junit5&logoColor=white) ![Mockito](https://img.shields.io/badge/Mockito-78A641) ![Testcontainers](https://img.shields.io/badge/Testcontainers-291A3F)

**Cloud & DevOps**

![AWS](https://img.shields.io/badge/AWS-FF9900?logo=amazonaws&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?logo=docker&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?logo=githubactions&logoColor=white)
![Vercel](https://img.shields.io/badge/Vercel-000000?logo=vercel&logoColor=white)
![Render](https://img.shields.io/badge/Render-46E3B7?logo=render&logoColor=white)
![Sentry](https://img.shields.io/badge/Sentry-362D59?logo=sentry&logoColor=white)
![Cloudflare](https://img.shields.io/badge/Cloudflare-F38020?logo=cloudflare&logoColor=white)

**IA no Desenvolvimento**

![Claude Code](https://img.shields.io/badge/Claude_Code-D97757?logo=claude&logoColor=white)

**Ferramentas & Métodos**

![Git](https://img.shields.io/badge/Git-F05032?logo=git&logoColor=white)
![GitHub](https://img.shields.io/badge/GitHub-181717?logo=github&logoColor=white)
![Postman](https://img.shields.io/badge/Postman-FF6C37?logo=postman&logoColor=white)
![VS Code](https://img.shields.io/badge/VS_Code-007ACC?logo=visualstudiocode&logoColor=white)

## 📫 Get In Touch

- Email: [akira.tochiro23@gmail.com](mailto:akira.tochiro23@gmail.com)
- LinkedIn: [linkedin.com/in/leandro-akira-tochiro](https://www.linkedin.com/in/leandro-akira-tochiro-661a52164/)
- Portfolio: [https://akira-portfolio-dev.vercel.app](https://akira-portfolio-dev.vercel.app)
