<div align="center">

<!-- Animated header -->
<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0d1117,50:1a1a2e,100:16213e&height=200&section=header&text=Bhagvendra%20Singh%20Parihar&fontSize=40&fontColor=58a6ff&animation=fadeIn&fontAlignY=38&desc=Node.js%20Backend%20Developer%20%7C%20Distributed%20Systems%20%7C%20Cloud%20Architecture&descAlignY=58&descColor=8b949e" width="100%"/>

<!-- Typing SVG -->
<a href="https://yashcodes.in">
  <img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=500&size=18&duration=3000&pause=1000&color=58A6FF&center=true&vCenter=true&multiline=false&width=600&lines=Building+scalable+microservices+with+Kafka+%26+Redis;250%2B+production+APIs+shipped+to+date;Event-driven+systems+%7C+AWS+cloud+architecture;BullMQ+%7C+gRPC+%7C+MongoDB+%7C+TypeScript" alt="Typing SVG" />
</a>

<br/>

<!-- Badges row -->
[![Portfolio](https://img.shields.io/badge/Portfolio-yashcodes.in-58a6ff?style=for-the-badge&logo=vercel&logoColor=white)](https://yashcodes.in)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-bhagvendra--singh-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/bhagvendra-singh)
[![Email](https://img.shields.io/badge/Email-pariharyash1989%40gmail.com-EA4335?style=for-the-badge&logo=gmail&logoColor=white)](mailto:pariharyash1989@gmail.com)
[![Postman](https://img.shields.io/badge/Postman-Student%20Expert-FF6C37?style=for-the-badge&logo=postman&logoColor=white)](https://yashcodes.in)

<br/>

<!-- Stats row -->
![Production APIs](https://img.shields.io/badge/Production%20APIs-250%2B-1f6feb?style=flat-square)
![Performance](https://img.shields.io/badge/Backend%20Performance%20Gain-30–50%25-238636?style=flat-square)
![Dispatch Accuracy](https://img.shields.io/badge/Dispatch%20Accuracy%20Improved-40%25-3fb950?style=flat-square)
![Monthly Transactions](https://img.shields.io/badge/Monthly%20Payments-1%2C000%2B-8957e5?style=flat-square)

</div>

---

## 👾 About Me

```ts
const bhagvendra = {
  alias     : "Yashcodes",
  role      : "Node.js Backend Developer",
  location  : "India 🇮🇳",
  experience: "2+ years in production backend engineering",

  currentWork: "Infinity Genesis Techso — microservices for SaaS platforms",

  focus: [
    "Distributed systems & event-driven architecture",
    "High-throughput Kafka pipelines",
    "Redis caching, Lua concurrency, rate limiting",
    "BullMQ job queues with per-tenant fairness",
    "Scalable cloud-native backends on AWS",
  ],

  superpower: "Turning complex system design problems into clean, measurable solutions",
};
```

---

## 🛠️ Tech Stack

<div align="center">

### ⚙️ Core Backend
![Node.js](https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=node.js&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![C++](https://img.shields.io/badge/C++-00599C?style=for-the-badge&logo=cplusplus&logoColor=white)
![Express.js](https://img.shields.io/badge/Express.js-000000?style=for-the-badge&logo=express&logoColor=white)

### 📨 Messaging & Queues
![Apache Kafka](https://img.shields.io/badge/Apache%20Kafka-231F20?style=for-the-badge&logo=apachekafka&logoColor=white)
![BullMQ](https://img.shields.io/badge/BullMQ-FF6B6B?style=for-the-badge&logo=redis&logoColor=white)
![gRPC](https://img.shields.io/badge/gRPC-244c5a?style=for-the-badge&logo=grpc&logoColor=white)

### ⚡ Caching & Data
![Redis](https://img.shields.io/badge/Redis-DC382D?style=for-the-badge&logo=redis&logoColor=white)
![MongoDB](https://img.shields.io/badge/MongoDB-47A248?style=for-the-badge&logo=mongodb&logoColor=white)

### ☁️ Cloud & Infrastructure
![AWS](https://img.shields.io/badge/AWS-232F3E?style=for-the-badge&logo=amazonaws&logoColor=white)
![Amazon S3](https://img.shields.io/badge/Amazon%20S3-569A31?style=for-the-badge&logo=amazons3&logoColor=white)
![Amazon Cognito](https://img.shields.io/badge/Amazon%20Cognito-FF9900?style=for-the-badge&logo=amazonaws&logoColor=white)
![AWS Lambda](https://img.shields.io/badge/AWS%20Lambda-FF9900?style=for-the-badge&logo=awslambda&logoColor=white)
![AWS EC2](https://img.shields.io/badge/AWS%20EC2-FF9900?style=for-the-badge&logo=amazonec2&logoColor=white)
![Amazon Location Service](https://img.shields.io/badge/Amazon%20Location%20Service-FF9900?style=for-the-badge&logo=amazonaws&logoColor=white)

### 🧰 Tooling & DevOps
![GitHub Actions](https://img.shields.io/badge/GitHub%20Actions-2088FF?style=for-the-badge&logo=githubactions&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![Postman](https://img.shields.io/badge/Postman-FF6C37?style=for-the-badge&logo=postman&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)

</div>

---

## 🏗️ Architecture Highlights

<details>
<summary><b>🔁 Inventory Bulk Upload — BullMQ + Redis Lua + S3 Streaming</b></summary>

<br/>

**Problem:** Large Excel uploads across multiple orgs caused race conditions, memory spikes, and one org blocking others for minutes.

**Solution:** Built a multi-tenant pipeline using:
- **BullMQ** workers (10–15 concurrent) for background processing
- **Redis Lua scripts** for atomic, per-org concurrency cap (max 2 active uploads/org)
- **`moveToDelayed`** to park capacity-blocked jobs — 0 retries consumed
- **ExcelJS streaming** + **S3 multipart upload** for flat memory usage
- **`setImmediate` yield points** to keep BullMQ lock renewal alive
- **Server-Sent Events (SSE)** for real-time client progress

**Result:** A 4-org upload scenario dropped from ~10 min → ~2.5 min with zero memory spikes.

</details>

<details>
<summary><b>⚡ Event-Driven SaaS with Kafka, Redis & gRPC</b></summary>

<br/>

**Problem:** Tightly coupled HTTP-based service communication was slowing down a growing SaaS platform with 1,000+ monthly transactions.

**Solution:**
- Introduced **Kafka** as the central message broker — services publish/subscribe instead of direct HTTP calls
- Used **Redis** for hot-data caching, rate limiting, and session state
- **gRPC** for latency-critical synchronous inter-service calls

**Result:** Decoupled architecture, improved horizontal scaling, and lower latency across services.

</details>

<details>
<summary><b>🔐 Unified Auth with Amazon Cognito — 20+ Roles, SSO</b></summary>

<br/>

**Problem:** Multiple internal tools and apps each maintained their own auth logic, creating security gaps and onboarding friction.

**Solution:** Centralized identity with **Amazon Cognito** — user pools, JWT-based API authorization, RBAC enforced at gateway and service layer, and SSO so users sign in once across all systems.

**Result:** 20+ roles managed uniformly, reduced security surface, faster developer onboarding.

</details>

<details>
<summary><b>📡 Geospatial Roadside Assistance Routing</b></summary>

<br/>

Combined **MongoDB geospatial indexes** with **Amazon Location Service** to match mechanics to breakdown locations in real-time. Improved dispatch accuracy by **40%** and reduced wait times across **500+ monthly requests**.

</details>

<details>
<summary><b>🌐 CodeNesters — Ed-Tech Platform (React.js, Node.js, AWS, Razorpay)</b></summary>

<br/>

- JWT auth with password hashing & reset-password flow — **50+ registered users**
- Reduced bandwidth by **40–50%** using pre-signed S3 URLs for direct uploads
- Improved performance by **30–40%** through Redis caching of redundant data

</details>

---

## 🎓 Education & Certifications

| | |
|---|---|
| 🎓 **B.Tech CSE** — Raipur Institute of Technology | CGPA: **8.7** · 2020–2024 |
| 🏫 **Class 12 PCM** — Bal Bharti Public School | **86%** · 2019–2020 |

**Certifications:** AI For India 2.0 &nbsp;·&nbsp; Career Essentials in Generative AI *(Microsoft & LinkedIn)* &nbsp;·&nbsp; HTML5 & CSS3 &nbsp;·&nbsp; Postman Student Expert

---

## 🎤 Mentorship & Community

- Mentored **40+ students** through backend engineering workshops
- Hosted interactive sessions with **90% attendance rate**
- Helped improve student proficiency levels by **30%**

---

## 📈 GitHub Stats

<div align="center">

<img height="180em" src="https://github-readme-stats.vercel.app/api?username=Yashcodes&show_icons=true&theme=github_dark&include_all_commits=true&count_private=true&hide_border=true&bg_color=0d1117&title_color=58a6ff&icon_color=1f6feb&text_color=8b949e"/>
<img height="180em" src="https://github-readme-stats.vercel.app/api/top-langs/?username=Yashcodes&layout=compact&theme=github_dark&hide_border=true&bg_color=0d1117&title_color=58a6ff&text_color=8b949e"/>

</div>

<div align="center">
  <img src="https://github-readme-streak-stats.herokuapp.com/?user=Yashcodes&theme=github-dark-blue&hide_border=true&background=0d1117&stroke=1f6feb&ring=58a6ff&fire=ff7b72&currStreakLabel=58a6ff" />
</div>

---

## 💼 Experience

| Period | Role | Company |
|--------|------|---------|
| **Nov 2024 – Present** | Backend Developer · Microservices · Node.js · MongoDB | Infinity Genesis Techso Pvt. Ltd. |
| **May 2024 – Oct 2024** | Software Developer Trainee · Flutter · REST APIs | DiracERP Solution Pvt. Ltd. |
| **Apr 2022 – Jul 2022** | Web Developer · Frontend | AMH Communications Pvt. Ltd. |

---

## 🔢 By the Numbers

<div align="center">

| Metric | Value |
|---|---|
| 🚀 Production APIs shipped | **250+** |
| ⚡ Backend performance improvement | **30–50%** |
| 🧭 Dispatch accuracy improvement | **40%** |
| 💳 Monthly payments processed | **1,000+** |
| 🛠 Monthly roadside assistance requests | **500+** |
| 📖 Developer onboarding time reduction | **35%** |
| 🔄 BullMQ concurrent workers | **10–15** |
| 🏢 Per-org upload cap (Redis Lua) | **2 active jobs** |

</div>

---

## 📬 Let's Connect

<div align="center">

I'm open to backend engineering roles, architecture reviews, and production systems discussions.

[![Portfolio](https://img.shields.io/badge/🌐%20Portfolio-yashcodes.in-58a6ff?style=for-the-badge)](https://yashcodes.in)
[![LinkedIn](https://img.shields.io/badge/💼%20LinkedIn-Connect-0077B5?style=for-the-badge)](https://linkedin.com/in/bhagvendra-singh)
[![Email](https://img.shields.io/badge/📧%20Email-Say%20Hello-EA4335?style=for-the-badge)](mailto:pariharyash1989@gmail.com)
[![Resume](https://img.shields.io/badge/📄%20Resume-Download-238636?style=for-the-badge)](https://yashcodes.in/resume.pdf)

<br/>

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:16213e,50:1a1a2e,100:0d1117&height=100&section=footer" width="100%"/>

</div>
