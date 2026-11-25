## Hi there 👋
<h1 align="center">Hi, I'm Rishabh Jha 👋</h1>

<p align="center">
  <b>Backend & Systems Engineer</b> · B.Tech CS '28 (ADGIPS, GGSIPU) · Delhi NCR, India<br/>
  I build distributed backend services and low-level network software in <b>Go</b> and <b>C++</b>.
</p>

<p align="center">
  <a href="https://www.linkedin.com/in/rishabh-jha-756345368"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"/></a>
  <a href="mailto:rrishabh2815@gmail.com"><img src="https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white" alt="Email"/></a>
  <img src="https://img.shields.io/badge/Open%20to-Summer%202027%20SDE%20Internships-2ea44f?style=for-the-badge" alt="Open to Summer 2027 SDE internships"/>
</p>

---

## 🚀 What I'm working on

- 🔨 **RakshaGrid**: a verified hyperlocal SOS dispatch system (Go, Redis, PostgreSQL, WebSockets). Selected for the **Grand Finale of Yantrika 1.0** (Faculty of Technology, University of Delhi).
- 🎯 Looking for a **Summer 2027 SDE / Technology internship** in backend or systems engineering.
- 📚 Going deeper into distributed systems, concurrency, and cloud infrastructure on AWS.

---

## 🧩 Featured projects

### 🛡️ [Sentinel](https://github.com/Rishabh2815/Sentinel): API gateway with ML-based bot detection
`Go` `Redis` `Python (FastAPI, scikit-learn)` `Docker` `Prometheus` `Grafana` `k6`

A reverse-proxy API gateway that rate-limits clients and adjusts each client's limit in real time from an ML bot-risk score.

- **Atomic sliding-window rate limiting** in Redis, enforcing precise per-client limits under concurrent load.
- **Fail-open design:** the scoring microservice has a **150 ms timeout**, so a model outage degrades bot detection but never gateway availability.
- **Measured, not claimed** (k6 on a Docker Compose stack):

| Scenario | Result |
|---|---|
| Normal traffic, 50 VUs | **p95 latency 15.19 ms** |
| Bot flood, 200 req/s (12,001 requests) | **99.17% rejected** by rate limiting |

- Full observability with Prometheus + Grafana dashboards for traffic, latency and rate-limit metrics.

---

### 🚨 [RakshaGrid](https://github.com/Rishabh2815/RakshaGrid): verified hyperlocal SOS dispatch
`Go` `React (PWA)` `Redis` `PostgreSQL` `WebSocket` `Docker` `Vercel` · [**Live demo**](https://github.com/Rishabh2815/RakshaGrid)

Geo-matches a verified SOS to the nearest available verified responder (security, wardens, volunteers).

- **Redis geospatial search** for nearest-responder matching, with **auto-escalation** if nobody acknowledges in time (targeting sub-second matching).
- **Real-time alerts** over WebSockets, **JWT auth**, a **multi-tenant PostgreSQL schema**, and an **append-only audit trail** feeding an admin compliance dashboard.
- **Offline-first PWA** (service worker, IndexedDB queue, Background Sync) so SOS requests survive connectivity loss.
- Core dispatch logic unit-tested using Go interface fakes.

---

### 📡 [WireSpectra](https://github.com/Rishabh2815/WireSpectra): multi-threaded deep packet inspection engine
`C++` `PCAP` `TCP/IP` `TLS` `Multithreading` `CMake`

- Parses **Ethernet/IP/TCP** headers from PCAP captures and tracks connections in a **5-tuple flow table**.
- Identifies applications by extracting **SNI from TLS Client Hello** packets, and enforces per-flow blocking by source IP, application and domain.
- **Concurrency design:** load-balancer threads feed fast-path workers over thread-safe queues, using **5-tuple hash-based flow affinity** so every packet of a connection lands on the same worker.
- Outputs a filtered PCAP with per-application statistics.

---

## 🛠️ Tech stack

| | |
|---|---|
| **Languages** | ![Go](https://img.shields.io/badge/Go-00ADD8?logo=go&logoColor=white) ![C++](https://img.shields.io/badge/C++-00599C?logo=cplusplus&logoColor=white) ![Python](https://img.shields.io/badge/Python-3776AB?logo=python&logoColor=white) ![SQL](https://img.shields.io/badge/SQL-4479A1?logo=postgresql&logoColor=white) ![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?logo=javascript&logoColor=black) |
| **Backend & Systems** | REST APIs · Microservices · Multithreading · WebSockets · JWT · Rate Limiting · TCP/IP & TLS · FastAPI |
| **Data** | ![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?logo=postgresql&logoColor=white) ![Redis](https://img.shields.io/badge/Redis-DC382D?logo=redis&logoColor=white) |
| **Cloud & DevOps** | ![AWS](https://img.shields.io/badge/AWS-232F3E?logo=amazonaws&logoColor=white) ![Terraform](https://img.shields.io/badge/Terraform-7B42BC?logo=terraform&logoColor=white) ![Docker](https://img.shields.io/badge/Docker-2496ED?logo=docker&logoColor=white) ![CMake](https://img.shields.io/badge/CMake-064F8C?logo=cmake&logoColor=white) · AWS (VPC, ALB/ASG, RDS, Route 53) |
| **Observability & Testing** | ![Prometheus](https://img.shields.io/badge/Prometheus-E6522C?logo=prometheus&logoColor=white) ![Grafana](https://img.shields.io/badge/Grafana-F46800?logo=grafana&logoColor=white) · k6 load testing · Go unit testing |
| **Frontend** | ![React](https://img.shields.io/badge/React-61DAFB?logo=react&logoColor=black) · PWA / Service Workers |
| **Applied ML** | scikit-learn |
| **CS Fundamentals** | DSA · OOP · System Design (HLD & LLD) · Operating Systems · DBMS · Computer Networks |

---

## 🏆 Highlights

- 🥇 **RakshaGrid** selected for the **Grand Finale of Yantrika 1.0**, University of Delhi.
- 🧮 Completed **Striver's SDE Sheet** (C++ solutions on GitHub) and solved **200+ LeetCode problems**.
- ☁️ **AWS Cloud Practitioner Essentials** certified.
- 🎓 B.Tech CSE, **CGPA 8.0/10** (Expected 2028).

---

## 📊 GitHub stats

<p align="center">
  <img height="165" src="https://github-readme-stats.vercel.app/api?username=Rishabh2815&show_icons=true&hide_border=true&count_private=true" alt="GitHub stats"/>
  <img height="165" src="https://github-readme-stats.vercel.app/api/top-langs/?username=Rishabh2815&layout=compact&hide_border=true" alt="Top languages"/>
</p>

---

## 📫 Let's connect

I'm actively looking for **Summer 2027 SDE / Technology internships**. The best ways to reach me:

- 📧 [rrishabh2815@gmail.com](mailto:rrishabh2815@gmail.com)
- 💼 [linkedin.com/in/rishabh-jha-756345368](https://www.linkedin.com/in/rishabh-jha-756345368)
<!--<h1 align="center">Hi, I'm Rishabh Jha 👋</h1>

<p align="center">
  <b>Backend & Systems Engineer</b> · B.Tech CS '28 (ADGIPS, GGSIPU) · Delhi NCR, India<br/>
  I build distributed backend services and low-level network software in <b>Go</b> and <b>C++</b>.
</p>

<p align="center">
  <a href="https://www.linkedin.com/in/rishabh-jha-756345368"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"/></a>
  <a href="mailto:rrishabh2815@gmail.com"><img src="https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white" alt="Email"/></a>
  <img src="https://img.shields.io/badge/Open%20to-Summer%202027%20SDE%20Internships-2ea44f?style=for-the-badge" alt="Open to Summer 2027 SDE internships"/>
</p>

---

## 🚀 What I'm working on

- 🔨 **RakshaGrid**: a verified hyperlocal SOS dispatch system (Go, Redis, PostgreSQL, WebSockets). Selected for the **Grand Finale of Yantrika 1.0** (Faculty of Technology, University of Delhi).
- 🎯 Looking for a **Summer 2027 SDE / Technology internship** in backend or systems engineering.
- 📚 Going deeper into distributed systems, concurrency, and cloud infrastructure on AWS.

---

## 🧩 Featured projects

### 🛡️ [Sentinel](https://github.com/Rishabh2815/Sentinel): API gateway with ML-based bot detection
`Go` `Redis` `Python (FastAPI, scikit-learn)` `Docker` `Prometheus` `Grafana` `k6`

A reverse-proxy API gateway that rate-limits clients and adjusts each client's limit in real time from an ML bot-risk score.

- **Atomic sliding-window rate limiting** in Redis, enforcing precise per-client limits under concurrent load.
- **Fail-open design:** the scoring microservice has a **150 ms timeout**, so a model outage degrades bot detection but never gateway availability.
- **Measured, not claimed** (k6 on a Docker Compose stack):

| Scenario | Result |
|---|---|
| Normal traffic, 50 VUs | **p95 latency 15.19 ms** |
| Bot flood, 200 req/s (12,001 requests) | **99.17% rejected** by rate limiting |

- Full observability with Prometheus + Grafana dashboards for traffic, latency and rate-limit metrics.

---

### 🚨 [RakshaGrid](https://github.com/Rishabh2815/RakshaGrid): verified hyperlocal SOS dispatch
`Go` `React (PWA)` `Redis` `PostgreSQL` `WebSocket` `Docker` `Vercel` · [**Live demo**](https://github.com/Rishabh2815/RakshaGrid)

Geo-matches a verified SOS to the nearest available verified responder (security, wardens, volunteers).

- **Redis geospatial search** for nearest-responder matching, with **auto-escalation** if nobody acknowledges in time (targeting sub-second matching).
- **Real-time alerts** over WebSockets, **JWT auth**, a **multi-tenant PostgreSQL schema**, and an **append-only audit trail** feeding an admin compliance dashboard.
- **Offline-first PWA** (service worker, IndexedDB queue, Background Sync) so SOS requests survive connectivity loss.
- Core dispatch logic unit-tested using Go interface fakes.

---

### 📡 [WireSpectra](https://github.com/Rishabh2815/WireSpectra): multi-threaded deep packet inspection engine
`C++` `PCAP` `TCP/IP` `TLS` `Multithreading` `CMake`

- Parses **Ethernet/IP/TCP** headers from PCAP captures and tracks connections in a **5-tuple flow table**.
- Identifies applications by extracting **SNI from TLS Client Hello** packets, and enforces per-flow blocking by source IP, application and domain.
- **Concurrency design:** load-balancer threads feed fast-path workers over thread-safe queues, using **5-tuple hash-based flow affinity** so every packet of a connection lands on the same worker.
- Outputs a filtered PCAP with per-application statistics.

---

## 🛠️ Tech stack

| | |
|---|---|
| **Languages** | ![Go](https://img.shields.io/badge/Go-00ADD8?logo=go&logoColor=white) ![C++](https://img.shields.io/badge/C++-00599C?logo=cplusplus&logoColor=white) ![Python](https://img.shields.io/badge/Python-3776AB?logo=python&logoColor=white) ![SQL](https://img.shields.io/badge/SQL-4479A1?logo=postgresql&logoColor=white) ![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?logo=javascript&logoColor=black) |
| **Backend & Systems** | REST APIs · Microservices · Multithreading · WebSockets · JWT · Rate Limiting · TCP/IP & TLS · FastAPI |
| **Data** | ![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?logo=postgresql&logoColor=white) ![Redis](https://img.shields.io/badge/Redis-DC382D?logo=redis&logoColor=white) |
| **Cloud & DevOps** | ![AWS](https://img.shields.io/badge/AWS-232F3E?logo=amazonaws&logoColor=white) ![Terraform](https://img.shields.io/badge/Terraform-7B42BC?logo=terraform&logoColor=white) ![Docker](https://img.shields.io/badge/Docker-2496ED?logo=docker&logoColor=white) ![CMake](https://img.shields.io/badge/CMake-064F8C?logo=cmake&logoColor=white) · AWS (VPC, ALB/ASG, RDS, Route 53) |
| **Observability & Testing** | ![Prometheus](https://img.shields.io/badge/Prometheus-E6522C?logo=prometheus&logoColor=white) ![Grafana](https://img.shields.io/badge/Grafana-F46800?logo=grafana&logoColor=white) · k6 load testing · Go unit testing |
| **Frontend** | ![React](https://img.shields.io/badge/React-61DAFB?logo=react&logoColor=black) · PWA / Service Workers |
| **Applied ML** | scikit-learn |
| **CS Fundamentals** | DSA · OOP · System Design (HLD & LLD) · Operating Systems · DBMS · Computer Networks |

---

## 🏆 Highlights

- 🥇 **RakshaGrid** selected for the **Grand Finale of Yantrika 1.0**, University of Delhi.
- 🧮 Completed **Striver's SDE Sheet** (C++ solutions on GitHub) and solved **200+ LeetCode problems**.
- ☁️ **AWS Cloud Practitioner Essentials** certified.
- 🎓 B.Tech CSE, **CGPA 8.0/10** (Expected 2028).

---

## 📊 GitHub stats

<p align="center">
  <img height="165" src="https://github-readme-stats.vercel.app/api?username=Rishabh2815&show_icons=true&hide_border=true&count_private=true" alt="GitHub stats"/>
  <img height="165" src="https://github-readme-stats.vercel.app/api/top-langs/?username=Rishabh2815&layout=compact&hide_border=true" alt="Top languages"/>
</p>

---

## 📫 Let's connect

I'm actively looking for **Summer 2027 SDE / Technology internships**. The best ways to reach me:

- 📧 [rrishabh2815@gmail.com](mailto:rrishabh2815@gmail.com)
- 💼 [linkedin.com/in/rishabh-jha-756345368](https://www.linkedin.com/in/rishabh-jha-756345368)
**Rishabh2815/Rishabh2815** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->
