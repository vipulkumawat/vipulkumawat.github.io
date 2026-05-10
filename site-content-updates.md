# vipulkumawat.in — Content Updates
> Find each section in your `index.html` and replace with the content below.
> Search for the old text (in quotes) and paste the new content in its place.

---

## 1. ABOUT ME SECTION
**Find:** the existing `<p>` tags inside `<!-- about --> section`
**Replace with this text:**

```
👋 Hello! I'm Vipul Kumawat — a Senior Software Engineer with 7+ years of 
experience building high-performance Java backend systems for global enterprise 
clients in banking and fintech.

🏦 I currently work at EPAM Systems, where I architect microservices-based 
platforms handling real-time financial data for Tier-1 banking clients across 
Europe. My work involves Java 11, Spring Boot, Apache Kafka, Redis, Spring Cloud 
Gateway, and Kubernetes — at production scale.

🚀 I'm passionate about clean architecture, system design, and helping other 
developers level up through real-world, project-based learning. That's why I 
created courses based on actual enterprise projects — not toy examples.

📬 Open to collaboration, mentorship conversations, or just geeking out about 
Java and distributed systems!
```

---

## 2. EXPERIENCE SECTION
**Find:** the 4 experience `<li>` items under `<!-- experience -->`

### Entry 1 — Replace "Software Engineer II" block:
```
Title:  Senior Software Engineer
Company: EPAM Systems
Period:  Sep 2021 — Present

Description:
Working as a Java Backend Engineer on enterprise-grade financial systems for 
global banking clients. Architected and developed microservices for a 
Credit Score Analysis Tool serving a leading Swedish bank.

Key contributions:
• Built real-time credit scoring pipelines using Apache Kafka, processing 
  high-volume financial data with low latency across distributed brokers
• Implemented OAuth 2.0 security with Spring Cloud Gateway using 
  TokenRelayGatewayFilterFactory for secure token validation
• Integrated Redis caching with @Cacheable, @CachePut, and @CacheEvict 
  annotations, reducing DB load on credit score lookups significantly
• Ensured GDPR compliance via AES-256 encryption and 
  @JsonSerialize(using=PartialMaskingSerializer.class) for data masking in logs
• Led Java 8 → Java 11 migration, replacing javax.xml.bind with modern APIs 
  and resolving all deprecated dependencies
• Implemented automated credit score alert notifications using JavaMailSender
• Set up CI/CD pipeline with Jenkins + Maven + Docker + Kubernetes for 
  zero-downtime blue-green deployments
• Maintained 80%+ code coverage enforced by SonarQube in the CI pipeline
```

### Entry 2 — Replace "Senior Software Engineer 2020-2021" block:
```
Title:  [Your Previous Job Title]
Company: [Your Previous Company]
Period:  2020 — 2021

Description:
[Add your real experience here — role responsibilities, technologies used,
and key achievements from this role.]
```

### Entry 3 — Replace "Software Engineer 2017-2019" block:
```
Title:  [Your Previous Job Title]
Company: [Your Previous Company]
Period:  2017 — 2019

Description:
[Add your real experience here — role responsibilities, technologies used,
and key achievements from this role.]
```

### Entry 4 — Replace "Trainee Software Engineer 2017" block:
```
Title:  Trainee Software Engineer
Company: [Your First Company]
Period:  2017 — 2017

Description:
Started software engineering career, learning Java development fundamentals,
agile practices, and enterprise application development workflows.
```

---

## 3. SKILLS SECTION
**Find:** the 4 skill bars under `<!-- skills -->`
**Replace with these 6 updated skills:**

```
Skill 1:
  Label: Java 11 + Spring Boot
  Value: 90%

Skill 2:
  Label: Apache Kafka + Redis
  Value: 80%

Skill 3:
  Label: MySQL + Spring Data JPA
  Value: 78%

Skill 4:
  Label: Docker + Kubernetes
  Value: 65%

Skill 5:
  Label: CI/CD (Jenkins + SonarQube)
  Value: 70%

Skill 6:
  Label: System Design + Microservices
  Value: 75%
```

---

## 4. ADD "COURSES" TO THE NAVIGATION
**Find:** your `<ul class="navbar-list">` in the nav
**Add this new item** between Resume and Blog:

```html
<li class="navbar-item">
  <a href="./courses.html" class="navbar-link">Courses</a>
</li>
```

---

## 5. UPDATE THE "WHAT I'M DOING" CARDS (About section)
**Find:** the service cards section
**Replace the two existing cards with:**

```
Card 1:
  Icon: icon-dev.svg (or any code icon)
  Title: Enterprise Java Backend
  Description: Building high-performance microservices for banking and fintech
  clients using Java 11, Spring Boot, Kafka, and Redis at production scale.

Card 2:
  Icon: icon-design.svg (or any learning icon)
  Title: Real-World Courses
  Description: Teaching enterprise Java development through actual production 
  projects — Credit Score Analysis Tools, real Kafka pipelines, real OAuth flows.
```

---

## 6. NEW FILE TO ADD
**Upload `courses.html`** (provided separately) to the root of your GitHub repo
alongside your `index.html`.

Commit message suggestion:
```
Add courses page + update experience, skills, and about sections
```

---

## QUICK CHECKLIST
- [ ] About me text updated
- [ ] EPAM experience entry filled with real content
- [ ] Previous job entries filled (Entries 2, 3, 4)
- [ ] Skills updated to Java/Kafka/Redis/Docker stack
- [ ] "Courses" added to navbar
- [ ] "What I'm doing" cards updated
- [ ] courses.html file added to repo root
- [ ] Commit and push to GitHub
