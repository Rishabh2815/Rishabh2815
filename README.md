# Hi, I'm Rishabh 👋 👨‍💻

![Rishabh Jha - backend & systems engineer](./assets/banner.svg)

I'm a backend and systems-focused software engineer who is passionate about building distributed services and low-level network software. Some technologies I enjoy working with include Go, C++, Redis, PostgreSQL and AWS. My project [RakshaGrid](https://github.com/Rishabh2815/RakshaGrid) was recently selected for the **Grand Finale of Yantrika 1.0**, organized by the Faculty of Technology, University of Delhi. I'm a B.Tech Computer Science student at ADGIPS (GGSIPU), graduating in 2028, and I'm currently looking for a **Summer 2027 SDE / Technology internship**.

## Things I've built 🔨:

- 🛡️ [**Sentinel**](https://github.com/Rishabh2815/Sentinel): a Go reverse-proxy API gateway with Redis-backed atomic sliding-window rate limiting and an ML bot-scoring service (FastAPI, scikit-learn) that adjusts each client's limit in real time. The model is a fail-open dependency with a 150 ms timeout, so a model outage never takes the gateway down. Load-tested with k6: **p95 latency 15.19 ms** at 50 VUs, and **99.17% of a 200 req/s bot flood rejected**. Instrumented with Prometheus and Grafana.
- 🚨 [**RakshaGrid**](https://github.com/Rishabh2815/RakshaGrid): a verified hyperlocal SOS dispatch system. A Go backend uses Redis geospatial search to match an SOS to the nearest verified responder, with auto-escalation if nobody acknowledges in time. Real-time WebSocket alerts, JWT auth, a multi-tenant PostgreSQL schema, an append-only audit trail, and an offline-first React PWA (service worker, IndexedDB queue, Background Sync).
- 📡 [**WireSpectra**](https://github.com/Rishabh2815/WireSpectra): a multi-threaded C++ deep packet inspection engine. It parses Ethernet/IP/TCP from PCAP captures, tracks connections in a 5-tuple flow table, identifies apps via TLS SNI, and enforces per-flow blocking. Load-balancer threads feed fast-path workers over thread-safe queues, with hash-based flow affinity so every packet of a connection reaches the same worker.

## Tech I work with 🧰:

- **Languages:** Go, C++, Python, SQL, JavaScript
- **Backend & systems:** REST APIs, microservices, multithreading, WebSockets, JWT, rate limiting, TCP/IP & TLS, FastAPI
- **Data:** PostgreSQL, Redis
- **Cloud & DevOps:** AWS (VPC, ALB/ASG, RDS, Route 53), Terraform, Docker, Docker Compose, CMake, Git
- **Observability & testing:** Prometheus, Grafana, k6, Go unit testing
- **Fundamentals:** DSA, OOP, system design (HLD & LLD), operating systems, DBMS, computer networks

## Highlights 🏆:

- Completed Striver's SDE Sheet (C++ solutions on GitHub) and solved **200+ LeetCode problems** 🧮
- **AWS Cloud Practitioner Essentials** certified ☁️
- CGPA **8.0 / 10** 🎓

## Find me around the web 🌎:

- Connecting with me on [LinkedIn](https://www.linkedin.com/in/rishabh-jha-756345368) 💼
- Reading my code on [GitHub](https://github.com/Rishabh2815) 💻
- Reaching out by email at [rrishabh2815@gmail.com](mailto:rrishabh2815@gmail.com) 📧
