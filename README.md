## Hi there 👋
<!-- Rename to README.md and place in your profile repo: github.com/Rishabh2815/Rishabh2815 -->

<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0f2027,50:203a43,100:2c5364&height=190&section=header&text=Rishabh%20Jha&fontSize=58&fontColor=ffffff&fontAlignY=38&desc=Backend%20%26%20Systems%20Engineer&descSize=20&descAlignY=60" alt="Rishabh Jha - Backend and Systems Engineer" width="100%" />

<a href="https://github.com/Rishabh2815">
  <img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=600&size=20&pause=1200&color=2DD4BF&center=true&vCenter=true&width=720&height=40&lines=I+build+backend+systems+that+stay+fast+and+stay+up;Go+%7C+C%2B%2B+%7C+Distributed+Systems+%7C+Networking;Rate+limiting%2C+real-time+dispatch%2C+packet+inspection;Open+to+SDE+internships+-+Summer+2027" alt="Typing animation" />
</a>

<br/>

<a href="https://www.linkedin.com/in/rishabh-jha-756345368"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn" /></a>
<a href="mailto:rrishabh2815@gmail.com"><img src="https://img.shields.io/badge/Email-EA4335?style=for-the-badge&logo=gmail&logoColor=white" alt="Email" /></a>
<img src="https://komarev.com/ghpvc/?username=Rishabh2815&style=for-the-badge&color=2c5364&label=PROFILE+VIEWS" alt="Profile views" />

</div>

<br/>

## `$ whoami`

```go
package main

type Engineer struct {
	Name      string
	Focus     []string
	Education string
	Location  string
	Seeking   string
}

var rishabh = Engineer{
	Name:      "Rishabh Jha",
	Focus:     []string{"Distributed backend services", "Multi-threaded network software", "Systems design"},
	Education: "B.Tech CSE, ADGIPS (GGSIPU) - expected 2028 - CGPA 8.0/10",
	Location:  "Delhi NCR, India",
	Seeking:   "SDE / Technology internship, Summer 2027",
}
```

<br/>

## By the numbers

| **15.19 ms** | **99.17%** | **150 ms** | **200+** |
| :---: | :---: | :---: | :---: |
| p95 gateway latency at 50 VUs | bot-flood requests rejected (12,001 req at 200 req/s) | ML-scorer timeout, fail-open by design | LeetCode problems solved, Striver's SDE Sheet completed |

<br/>

## Featured projects

### Sentinel - API gateway with ML-based bot detection
`Go` `Redis` `Python (FastAPI, scikit-learn)` `Docker` `Prometheus` `Grafana` `k6`

A reverse-proxy gateway with Redis-backed atomic sliding-window rate limiting. A bot-scoring microservice adjusts each client's limit in real time, and it is a fail-open dependency, so a model outage degrades detection but never gateway availability. Load-tested with k6 on a Docker Compose stack.

```mermaid
flowchart LR
    C([Client]) --> G["Go gateway<br/>reverse proxy"]
    G <--> R[("Redis<br/>sliding-window limiter")]
    G -->|"150ms timeout, fail-open"| M["FastAPI + scikit-learn<br/>bot risk score"]
    M -.->|"adjusts rate limit"| G
    G --> U([Upstream service])
    G -.-> P["Prometheus"] -.-> Gr["Grafana"]
```

<br/>

### RakshaGrid - verified hyperlocal SOS dispatch
`Go` `React PWA` `Redis` `PostgreSQL` `WebSocket` `Docker` `Vercel`

Geo-matches a verified SOS to the nearest available verified responder (security, wardens, volunteers) using Redis geospatial search, and auto-escalates if nobody acknowledges in time. Offline-first PWA so requests survive connectivity loss. Selected for the **Grand Finale of Yantrika 1.0** (Faculty of Technology, University of Delhi).

```mermaid
flowchart LR
    A["React PWA<br/>IndexedDB queue + Background Sync"] -->|"SOS"| B["Go API<br/>JWT, multi-tenant"]
    B --> C[("Redis GEO<br/>nearest verified responder")]
    C --> D["WebSocket alert"]
    D -->|"no ack in time"| E["Auto-escalate"]
    E --> C
    B --> F[("PostgreSQL<br/>append-only audit trail")]
    F --> G["Admin compliance dashboard"]
```

<br/>

### WireSpectra - multi-threaded deep packet inspection engine
`C++` `PCAP` `TCP/IP` `TLS` `Multithreading` `CMake`

Parses Ethernet/IP/TCP headers from PCAP captures, tracks connections in a 5-tuple flow table, identifies applications by extracting SNI from TLS Client Hello packets, and enforces per-flow blocking by source IP, application and domain. Hash-based flow affinity guarantees every packet of a connection reaches the same worker.

```mermaid
flowchart LR
    A["PCAP input"] --> B["Parse<br/>Ethernet / IP / TCP"]
    B --> C["Load-balancer threads<br/>hash the 5-tuple"]
    C --> D1["Fast-path worker 1"]
    C --> D2["Fast-path worker N"]
    D1 & D2 --> E["Flow table, SNI classification,<br/>block rules"]
    E --> F["Filtered PCAP<br/>per-application stats"]
```

<br/>

## Tech stack

<table>
  <tr>
    <td><b>Languages</b></td>
    <td><img src="https://skillicons.dev/icons?i=go,cpp,py,js&theme=dark" alt="Go, C++, Python, JavaScript" /></td>
  </tr>
  <tr>
    <td><b>Backend</b></td>
    <td><img src="https://skillicons.dev/icons?i=fastapi,react&theme=dark" alt="FastAPI, React" /> &nbsp;REST, Microservices, WebSockets, JWT, Rate Limiting, TCP/IP, TLS</td>
  </tr>
  <tr>
    <td><b>Data</b></td>
    <td><img src="https://skillicons.dev/icons?i=postgres,redis&theme=dark" alt="PostgreSQL, Redis" /></td>
  </tr>
  <tr>
    <td><b>Cloud and DevOps</b></td>
    <td><img src="https://skillicons.dev/icons?i=aws,terraform,docker,git,github,vercel&theme=dark" alt="AWS, Terraform, Docker, Git, GitHub, Vercel" /> &nbsp;VPC, ALB/ASG, RDS, Route 53</td>
  </tr>
  <tr>
    <td><b>Observability and ML</b></td>
    <td><img src="https://skillicons.dev/icons?i=prometheus,grafana,sklearn&theme=dark" alt="Prometheus, Grafana, scikit-learn" /> &nbsp;k6 load testing</td>
  </tr>
  <tr>
    <td><b>CS fundamentals</b></td>
    <td>Data Structures and Algorithms, OOP, Operating Systems, DBMS, Computer Networks, System Design (HLD and LLD)</td>
  </tr>
</table>

<br/>

## Achievements

- **Yantrika 1.0 Grand Finale** - RakshaGrid selected, organized by the Faculty of Technology, University of Delhi
- **Striver's SDE Sheet** completed (C++ solutions on GitHub) and **200+ LeetCode** problems solved
- **AWS Cloud Practitioner Essentials** certified

<br/>

## GitHub activity

<div align="center">

<img height="170" src="https://github-readme-stats.vercel.app/api?username=Rishabh2815&show_icons=true&theme=tokyonight&hide_border=true&count_private=true" alt="GitHub stats" />
<img height="170" src="https://github-readme-stats.vercel.app/api/top-langs/?username=Rishabh2815&layout=compact&theme=tokyonight&hide_border=true" alt="Top languages" />

<img src="https://streak-stats.demolab.com?user=Rishabh2815&theme=tokyonight&hide_border=true" alt="GitHub streak" />

</div>

<br/>

## Let's talk

I'm looking for **Summer 2027 SDE / Technology internships** where I can work on backend, distributed systems or networking problems. The fastest way to reach me is email: **rrishabh2815@gmail.com**.

<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:2c5364,50:203a43,100:0f2027&height=110&section=footer" alt="" width="100%" />

</div>

<!--
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
