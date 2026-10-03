<div align="center">

<img width="100%" src="https://capsule-render.vercel.app/api?type=waving&color=0:00d9ff,50:7b5ea7,100:050810&height=200&section=header&text=Md%20Shoaib%20Islam&fontSize=55&fontColor=ffffff&fontAlignY=38&desc=Backend%20Developer%20%7C%20Full-Stack%20Engineer%20%7C%20Open%20to%20Work&descAlignY=58&descSize=17&animation=fadeIn"/>

<img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=20&pause=1000&color=00D9FF&center=true&vCenter=true&width=750&lines=PHP+%7C+Laravel+%7C+Java+%7C+Spring+Boot+%7C+Node.js;React+%7C+Next.js+%7C+REST+APIs+%7C+Microservices+%7C+Docker;PostgreSQL+%7C+Redis+%7C+RabbitMQ+%7C+Sentry+%7C+Horizon;Building+scalable+backend+systems+and+real-world+applications;Open+to+Full-Time+%26+Freelance+Opportunities" alt="Typing SVG"/>

<br/>

<a href="mailto:mdshoaiburislam@gmail.com">
<img src="https://img.shields.io/badge/✉%20Hire%20Me-mdshoaiburislam%40gmail.com-00d9ff?style=for-the-badge&logo=gmail&logoColor=white"/>
</a>
&nbsp;
<a href="https://www.linkedin.com/in/m3s7a/">
<img src="https://img.shields.io/badge/LinkedIn-m3s7a-0077B5?style=for-the-badge&logo=linkedin&logoColor=white"/>
</a>
&nbsp;
<a href="https://github.com/shoaib3375">
<img src="https://img.shields.io/badge/GitHub-shoaib3375-181717?style=for-the-badge&logo=github&logoColor=white"/>
</a>

<br/><br/>

<img src="https://komarev.com/ghpvc/?username=shoaib3375&color=00d9ff&style=flat-square&label=Profile+Views"/>
&nbsp;
<img src="https://img.shields.io/github/followers/shoaib3375?label=Followers&style=flat-square&color=7b5ea7"/>

</div>

---

## 👨‍💻 About Me

I'm a **Backend Developer and Full-Stack Engineer** focused on building reliable, maintainable, and scalable web applications.

My primary backend stack is **PHP/Laravel**, with additional experience in **Java/Spring Boot and Node.js**. I also work with **React, Next.js, relational databases, Redis, RabbitMQ, Docker, Linux, and REST APIs**.

```yaml
name: "Md Shoaib Islam"
location: "Dhaka, Bangladesh 🇧🇩"
education: "B.Sc. in Computer Science & Engineering"
role:
  - Backend Developer
  - Full-Stack Developer
backend:
  - PHP
  - Laravel
  - Java
  - Spring Boot
  - Node.js
  - Express.js
frontend:
  - React
  - Next.js
  - TypeScript
  - Tailwind CSS
  - Vue.js
databases:
  - MySQL
  - PostgreSQL
  - Redis
architecture:
  - REST APIs
  - Microservices
  - Event-driven systems
  - Authentication & Authorization
  - Queue-based processing
devops:
  - Linux
  - Docker
  - Nginx
  - Git
  - GitHub Actions
  - VPS Deployment
messaging:
  - RabbitMQ
  - Redis Queues
status: "Open to Full-Time & Freelance Opportunities"
```

---

## 🚀 What I Build

* Scalable RESTful APIs
* Laravel backend applications
* Business management systems
* Payment and wallet systems
* Crypto & currency exchange platforms
* Microservice-based applications
* Authentication & authorization systems
* Admin dashboards
* Queue-based background processing
* Real-time applications
* Database-driven applications
* Production deployments with Docker

---

## 🔥 Featured Projects

### 💱 AGIO — Crypto Exchange Platform

A production-grade crypto-to-crypto exchange platform with live liquidity provider routing, real-time order tracking, financial reconciliation, and a full admin operations suite.

**Architecture**

```text
                 Next.js 14 (Frontend)
                        │
                 Laravel 13 API (/v1)
                        │
         ┌──────────────┼──────────────┐
         │              │              │
    Quote Engine   Order Service  Reconciliation
         │              │
  ┌──────┴──────┐   SSE Stream
  │  Best-Rate  │   (real-time)
  │   Router    │
  └──────┬──────┘
         │ PHP Fibers (parallel)
  ┌──────┴────────────────────┐
  │  ChangeNOW  │  Changelly  │
  │  SimpleSwap │  FixedFloat │
  └───────────────────────────┘
         │
   PostgreSQL 16
   (1 primary + 2 read replicas)
        +
      Redis 7
```

**Core Features**

* Best-rate router — queries all 4 providers concurrently via PHP Fibers, selects highest customer output
* Circuit breaker per provider — auto-trips on failures, degraded state, auto-resets with Slack alert
* Full order lifecycle — 17 states from `awaiting_deposit` → `completed` with full event history
* On-chain verification — blockchain deposit detection, confirmation progress, payout verification
* Financial reconciliation — 9 scopes (wallet balance, ledger invariant, payout mismatch, etc.)
* Real-time SSE — order status streamed to browser every 2s; toast notification on terminal state
* Classic exchange — manual fiat-based flow with payment proof upload
* Subscription payments — bKash / Nagad / bank for Netflix, Spotify, etc.
* PWA — installable, offline fallback, service worker caching
* Admin operations — live system health, provider circuit states, stuck orders, reconciliation dashboard

**Observability**

* Sentry (Laravel + Next.js) — error tracking, performance traces, financial data scrubbed
* Slack critical alerts — circuit trips, reconciliation breaks, stuck orders (5-min dedup)
* Laravel Horizon — queue dashboard, 4 priority queues (critical / high / default / low)
* Structured JSON logging — machine-readable for Loki / CloudWatch / Papertrail
* Deep health endpoint — DB latency, Redis, queue backlog, all provider circuit states

**Infrastructure**

* Docker Compose — 7 containers (app, primary DB, 2 read replicas, Redis, frontend, mailpit)
* PostgreSQL 16 streaming replication — reads load-balanced, sticky writes to primary
* GitHub Actions → Docker Compose deploy on push to `main`

**Technologies**

`Laravel 13` `PHP 8.4` `Next.js 14` `TypeScript` `PostgreSQL 16` `Redis` `Docker` `Laravel Horizon` `Sentry` `SSE` `Tailwind CSS`

---

### 🏗️ Microservices Backend Architecture

A modular backend architecture designed around independent services for authentication, users, wallets, payments, and currency exchange.

```text
                    API / Client
                         │
                         ▼
                  ┌─────────────┐
                  │    Nginx    │
                  └──────┬──────┘
                         │
          ┌──────────────┼──────────────┐
          │              │              │
          ▼              ▼              ▼
     Auth Service   User Service   Wallet Service
          │              │              │
          └──────────────┼──────────────┘
                         │
              ┌──────────┴──────────┐
              │                     │
              ▼                     ▼
         Payment Service      Exchange Service
              │                     │
              └──────────┬──────────┘
                         │
                 ┌───────┴────────┐
                 │                │
              RabbitMQ          Redis
                 │                │
                 └───────┬────────┘
                         │
                    PostgreSQL
```

**Technologies**

`Laravel` `PHP` `PostgreSQL` `Redis` `RabbitMQ` `Docker` `Nginx`

---

### 🔮 Rukaiyah — Spiritual Healing Platform

A web platform designed to connect clients with qualified spiritual healers through appointment scheduling and digital services.

**Features**

* Authentication & role-based access control
* Practitioner management & appointment scheduling
* Wallet functionality & exchange-rate management
* Admin dashboard & real-time communication
* Background jobs and queues

**Technologies**

`Laravel` `PHP` `Vue.js` `Tailwind CSS` `MySQL` `Redis` `WebSockets` `Docker`

---

### 🧺 eLaundry

An online laundry management platform handling users, orders, services, and administrative operations.

**Technologies**

`Laravel` `PHP` `Spring Boot` `MySQL` `REST API` `Microservices`

**Repository**

<a href="https://github.com/Shoaib3375/luandryapi">GitHub → eLaundry API</a>

---

### 🧠 Jetty Healing Model

A personal project integrating **NLP and machine learning** for text classification on the Jetty Healing platform.

**Technologies**

`Python` `scikit-learn` `NLP` `Flask` `NumPy` `Pandas`

**Repository**

<a href="https://github.com/Shoaib3375/JettyMLBackBone">GitHub → JettyMLBackBone</a>

---

## 💻 Tech Stack

<div align="center">

### Languages
<img src="https://skillicons.dev/icons?i=php,java,python,javascript,typescript,cpp,c"/>

### Backend
<img src="https://skillicons.dev/icons?i=laravel,spring,nodejs,express,flask"/>

### Frontend
<img src="https://skillicons.dev/icons?i=react,nextjs,vue,html,css,tailwind,vite"/>

### Databases & Infrastructure
<img src="https://skillicons.dev/icons?i=mysql,postgres,redis,docker,nginx,linux"/>

### Development Tools
<img src="https://skillicons.dev/icons?i=git,github,postman,idea,vscode"/>

</div>

---

## 🔧 Backend Skills

```text
✓ PHP & Laravel                    ✓ Redis Caching
✓ Java & Spring Boot               ✓ Queue & Background Jobs
✓ Node.js & Express.js             ✓ RabbitMQ
✓ REST API Development             ✓ Microservices
✓ API Authentication               ✓ WebSockets & SSE
✓ JWT / Token Authentication       ✓ Payment & Wallet Logic
✓ Laravel Sanctum                  ✓ Transaction Processing
✓ Role & Permission Systems        ✓ Admin Systems
✓ Database Design                  ✓ Laravel Horizon
✓ MySQL & PostgreSQL               ✓ Sentry & Observability
✓ Eloquent ORM                     ✓ CI/CD & Docker
```

---

## 🐳 DevOps & Infrastructure

```text
Linux
 │
 ├── Nginx
 ├── PHP / Laravel
 ├── Node.js / Next.js
 ├── Redis
 ├── MySQL / PostgreSQL (with streaming replication)
 │
 └── Docker
      ├── Application Containers
      ├── Database (primary + replicas)
      ├── Redis
      ├── Laravel Horizon
      └── GitHub Actions CI/CD
```

---

## 📊 GitHub Stats

<div align="center">

<img height="180" src="https://github-readme-stats.vercel.app/api?username=shoaib3375&show_icons=true&theme=tokyonight&include_all_commits=true&count_private=true&hide_border=true&bg_color=050810&title_color=00d9ff&icon_color=7b5ea7&text_color=e8edf5"/>

<img height="180" src="https://github-readme-stats.vercel.app/api/top-langs/?username=shoaib3375&layout=compact&langs_count=8&theme=tokyonight&hide_border=true&bg_color=050810&title_color=00d9ff&text_color=e8edf5"/>

</div>

<div align="center">
<img src="https://streak-stats.demolab.com/?user=shoaib3375&theme=tokyonight&hide_border=true&background=050810&ring=00d9ff&fire=7b5ea7&currStreakLabel=00d9ff"/>
</div>

<div align="center">
<img src="https://github-readme-activity-graph.vercel.app/graph?username=shoaib3375&theme=react-dark&bg_color=050810&color=00d9ff&line=7b5ea7&point=ffffff&hide_border=true"/>
</div>

---

## 🎯 Current Focus

```text
🚀 Building production-ready backend systems
🏗️ Designing scalable microservice architectures
⚡ Working with Redis & RabbitMQ
🐳 Docker & containerization in production
☁️ Cloud infrastructure & CI/CD pipelines
🔐 Secure payment & crypto exchange systems
📊 Observability: Sentry, Slack alerts, structured logging
📚 System design & software architecture
🌍 Growing open-source contributions
```

---

## 🤝 Let's Connect

<div align="center">

<a href="mailto:mdshoaiburislam@gmail.com">
<img src="https://img.shields.io/badge/Gmail-D14836?style=for-the-badge&logo=gmail&logoColor=white"/>
</a>
&nbsp;
<a href="https://www.linkedin.com/in/m3s7a/">
<img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white"/>
</a>
&nbsp;
<a href="https://github.com/shoaib3375">
<img src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white"/>
</a>
&nbsp;
<a href="https://twitter.com/MDShoaibmesta">
<img src="https://img.shields.io/badge/X-000000?style=for-the-badge&logo=x&logoColor=white"/>
</a>

<br/><br/>

<strong>Open to Full-Time Roles, Freelance Projects & Engineering Collaborations</strong>
<br/>
<em>Backend Development · Full-Stack Development · Microservices · Software Engineering</em>

</div>

---

<div align="center">

<img width="100%" src="https://capsule-render.vercel.app/api?type=waving&color=0:050810,50:7b5ea7,100:00d9ff&height=120&section=footer&animation=fadeIn"/>

<strong><code>Build · Learn · Ship · Improve</code></strong> 🚀

</div>
