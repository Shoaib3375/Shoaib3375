<div align="center">

<img width="100%" src="https://capsule-render.vercel.app/api?type=waving&color=0:00d9ff,50:7b5ea7,100:050810&height=200&section=header&text=Md%20Shoaib%20Islam&fontSize=55&fontColor=ffffff&fontAlignY=38&desc=Backend%20Developer%20%7C%20Full-Stack%20Engineer&descAlignY=58&descSize=18&animation=fadeIn"/>

**Laravel · Spring Boot · PostgreSQL · Redis · Docker**
<br/>
*Building scalable APIs, payment systems, and exchange platforms. Based in Dhaka, Bangladesh 🇧🇩*

<br/>

<a href="mailto:mdshoaiburislam@gmail.com">
<img src="https://img.shields.io/badge/✉%20Hire%20Me-mdshoaiburislam%40gmail.com-00d9ff?style=for-the-badge&logo=gmail&logoColor=white"/>
</a>
&nbsp;
<a href="https://www.linkedin.com/in/m3s7a/">
<img src="https://img.shields.io/badge/LinkedIn-m3s7a-0077B5?style=for-the-badge&logo=linkedin&logoColor=white"/>
</a>
&nbsp;
<a href="https://twitter.com/MDShoaibmesta">
<img src="https://img.shields.io/badge/X-MDShoaibmesta-000000?style=for-the-badge&logo=x&logoColor=white"/>
</a>

</div>

---

## 👨‍💻 About Me

I'm a **Backend Developer and Full-Stack Engineer** who builds reliable, maintainable, and scalable web applications.

My main stack is **PHP/Laravel**, with experience in **Java/Spring Boot** and **Node.js**. On the frontend I work with **React, Next.js, and Vue.js**. I'm currently a **Software Engineer at Triple Commas Inc** and studying **B.Sc. in Computer Science & Engineering**.

---

## ⚡ At a Glance

| | |
|:--|:--|
| **Role** | Software Engineer @ Triple Commas Inc (Feb 2024 – Present) |
| **Focus** | Backend engineering · REST APIs · Payment, wallet & exchange systems |
| **Primary stack** | PHP / Laravel · Spring Boot · PostgreSQL · Redis · Docker |
| **Education** | B.Sc. in Computer Science & Engineering (ongoing), Institute of Science and Technology, Dhaka |
| **Location** | Dhaka, Bangladesh 🇧🇩 |
| **Open to** | Full-time roles · Freelance projects |
| **Contact** | [mdshoaiburislam@gmail.com](mailto:mdshoaiburislam@gmail.com) · [LinkedIn](https://www.linkedin.com/in/m3s7a/) |

<!-- TODO (optional): add "Work preference: Remote / Hybrid / On-site" and availability / notice period -->

---

## 🔥 Featured Projects

### 💱 AGIO — Crypto Exchange Platform

A production-grade crypto-to-crypto exchange platform with live liquidity-provider routing, real-time order tracking, financial reconciliation, and a full admin operations suite.

<!-- TODO: add link to your public showcase repo or demo here, e.g. [📂 View project →](https://github.com/Shoaib3375/...) -->

```text
 Next.js 14  ──►  Laravel 13 API  ──►  Best-Rate Router (PHP Fibers, parallel)
                       │                    ├─ ChangeNOW   ├─ Changelly
                       │                    └─ SimpleSwap  └─ FixedFloat
                       │
          ┌────────────┼─────────────┐
     Order Service   SSE Stream   Reconciliation ──► Slack / Sentry alerts
          │
   PostgreSQL 16 (1 primary + 2 read replicas)  ·  Redis 7  ·  Laravel Horizon
```

- **Best-rate routing:** queries 4 providers in parallel with PHP Fibers and picks the highest customer output
- **Circuit breakers:** per-provider auto-trip on failure, auto-reset, Slack alert
- **Order lifecycle:** 17 states from `awaiting_deposit` to `completed`, with full event history and on-chain deposit/payout verification
- **Double-entry ledger** with reconciliation across 9 scopes (wallet balance, ledger invariant, payout mismatch, etc.)
- **Real-time tracking** via Server-Sent Events, with a 5-step quote wizard on the frontend
- **Subscription payments** via bKash / Nagad / bank, and a manual fiat exchange flow with payment-proof upload
- **Admin operations:** system health, provider circuit state, stuck orders, refund / retry payout / cancel / resume, and an immutable audit trail
- **Observability:** Sentry, structured JSON logs, Prometheus + Grafana + Loki, Slack alerts with 5-min dedup, deep health endpoint
- **Infrastructure:** Docker Compose, PostgreSQL streaming replication with read/write splitting, GitHub Actions CI/CD with zero-downtime deploys

`Laravel 13` `PHP 8.4` `Next.js 14` `TypeScript` `PostgreSQL 16` `Redis` `Docker` `Horizon` `Sentry` `SSE` `Tailwind CSS`

---

### 🧺 eLaundry — Laundry Management System

A full-stack laundry management platform covering users, orders, pricing, coupons, services, and admin operations, with secure JWT-based REST APIs, role-based access, and order tracking from creation to completion.

📂 [Laravel API](https://github.com/Shoaib3375/luandryapi) · [Frontend](https://github.com/Shoaib3375/LaundryFrontEnd)

`Laravel` `Spring Boot` `React` `MySQL` `REST API` `JWT` `Swagger`

---

### 🔮 Rukaiyah — Spiritual Healing Platform

A web platform that connects clients with qualified spiritual healers through appointment scheduling and digital services: role-based access, practitioner management, wallet and exchange-rate management, an admin dashboard, real-time communication, and background jobs.

<!-- TODO: add repo / demo / screenshot link -->

`Laravel` `Vue.js` `Tailwind CSS` `MySQL` `Redis` `WebSockets` `Docker`

---

### 🏗️ Microservices Backend Architecture

A modular backend split into independent services for authentication, users, wallets, payments, and currency exchange, communicating through RabbitMQ and Redis behind an Nginx gateway.

<!-- TODO: add repo / diagram link -->

`Laravel` `PostgreSQL` `Redis` `RabbitMQ` `Docker` `Nginx`

---

### 🧠 Jetty Healing Model

An NLP and machine-learning project for text classification on the Jetty Healing platform.

📂 [JettyMLBackBone](https://github.com/Shoaib3375/JettyMLBackBone)

`Python` `scikit-learn` `NLP` `Flask` `NumPy` `Pandas`

---

## 💻 Tech Stack

<div align="center">

**Core stack (what I use in production)**

<img src="https://img.shields.io/badge/PHP-777BB4?style=for-the-badge&logo=php&logoColor=white"/> <img src="https://img.shields.io/badge/Laravel-FF2D20?style=for-the-badge&logo=laravel&logoColor=white"/> <img src="https://img.shields.io/badge/Spring%20Boot-6DB33F?style=for-the-badge&logo=springboot&logoColor=white"/> <img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white"/> <img src="https://img.shields.io/badge/Redis-DC382D?style=for-the-badge&logo=redis&logoColor=white"/> <img src="https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white"/> <img src="https://img.shields.io/badge/REST%20APIs-00d9ff?style=for-the-badge&logo=openapiinitiative&logoColor=white"/>

</div>

<br/>

| Area | Technologies |
|:--|:--|
| **Languages** | <img src="https://img.shields.io/badge/PHP-777BB4?style=flat-square&logo=php&logoColor=white"/> <img src="https://img.shields.io/badge/Java-ED8B00?style=flat-square&logo=openjdk&logoColor=white"/> <img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black"/> <img src="https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white"/> <img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white"/> |
| **Backend** | <img src="https://img.shields.io/badge/Laravel-FF2D20?style=flat-square&logo=laravel&logoColor=white"/> <img src="https://img.shields.io/badge/Spring%20Boot-6DB33F?style=flat-square&logo=springboot&logoColor=white"/> <img src="https://img.shields.io/badge/Node.js-339933?style=flat-square&logo=nodedotjs&logoColor=white"/> <img src="https://img.shields.io/badge/Express-000000?style=flat-square&logo=express&logoColor=white"/> <img src="https://img.shields.io/badge/Flask-000000?style=flat-square&logo=flask&logoColor=white"/> |
| **Frontend** | <img src="https://img.shields.io/badge/React-61DAFB?style=flat-square&logo=react&logoColor=black"/> <img src="https://img.shields.io/badge/Next.js-000000?style=flat-square&logo=nextdotjs&logoColor=white"/> <img src="https://img.shields.io/badge/Vue.js-4FC08D?style=flat-square&logo=vuedotjs&logoColor=white"/> <img src="https://img.shields.io/badge/Tailwind%20CSS-06B6D4?style=flat-square&logo=tailwindcss&logoColor=white"/> <img src="https://img.shields.io/badge/HTML5-E34F26?style=flat-square&logo=html5&logoColor=white"/> <img src="https://img.shields.io/badge/CSS3-1572B6?style=flat-square&logo=css3&logoColor=white"/> |
| **Databases & Messaging** | <img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white"/> <img src="https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white"/> <img src="https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white"/> <img src="https://img.shields.io/badge/RabbitMQ-FF6600?style=flat-square&logo=rabbitmq&logoColor=white"/> |
| **DevOps & Infra** | <img src="https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white"/> <img src="https://img.shields.io/badge/Docker%20Compose-2496ED?style=flat-square&logo=docker&logoColor=white"/> <img src="https://img.shields.io/badge/GitHub%20Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white"/> <img src="https://img.shields.io/badge/Nginx-009639?style=flat-square&logo=nginx&logoColor=white"/> <img src="https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black"/> |
| **Observability** | <img src="https://img.shields.io/badge/Sentry-362D59?style=flat-square&logo=sentry&logoColor=white"/> <img src="https://img.shields.io/badge/Prometheus-E6522C?style=flat-square&logo=prometheus&logoColor=white"/> <img src="https://img.shields.io/badge/Grafana-F46800?style=flat-square&logo=grafana&logoColor=white"/> <img src="https://img.shields.io/badge/Laravel%20Horizon-FF2D20?style=flat-square&logo=laravel&logoColor=white"/> |
| **Tools & Docs** | <img src="https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white"/> <img src="https://img.shields.io/badge/GitHub-181717?style=flat-square&logo=github&logoColor=white"/> <img src="https://img.shields.io/badge/Postman-FF6C37?style=flat-square&logo=postman&logoColor=white"/> <img src="https://img.shields.io/badge/Swagger-85EA2D?style=flat-square&logo=swagger&logoColor=black"/> <img src="https://img.shields.io/badge/IntelliJ%20IDEA-000000?style=flat-square&logo=intellijidea&logoColor=white"/> <img src="https://img.shields.io/badge/VS%20Code-007ACC?style=flat-square&logo=visualstudiocode&logoColor=white"/> |

**Engineering practices:** MVC & DTO architecture · REST API design · JWT authentication & role-based access control · Queue-based background jobs · Read/write DB splitting · Double-entry ledgers & reconciliation · CI/CD with zero-downtime deploys · API documentation (Swagger)

---

## 🎯 Currently Focused On

- Production-ready backend systems and secure payment / exchange flows
- Scalable microservice architecture, Redis and RabbitMQ
- Docker, CI/CD, and observability (Sentry, Prometheus, Grafana)
- System design and software architecture

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
<a href="https://twitter.com/MDShoaibmesta">
<img src="https://img.shields.io/badge/X-000000?style=for-the-badge&logo=x&logoColor=white"/>
</a>

<br/><br/>

**Open to full-time roles, freelance projects & engineering collaborations**

<img width="100%" src="https://capsule-render.vercel.app/api?type=waving&color=0:050810,50:7b5ea7,100:00d9ff&height=100&section=footer"/>

</div>
