<!-- Pleiades '26 — Project Showcase README -->

<div align="center">

```
 ____  __    ____  __   __   ____  ____  ____
(  _ \(  )  ( ___)(__) /__\ (  _ \( ___)/ ___)
 )___/ )(__  )__)  )( /(__)\ )(_) ))__)  \___ \
(__)  (____)(____)(__(__)(__)(___ /(____) (___/
```

```
┌──────────────────────────────────────────────────────────────┐
│   techno-cultural fest platform built for  KLE Tech          │
├──────────────────────────────────────────────────────────────┤
│   8,000+ concurrent users  •  live in production  •  2026    │
└──────────────────────────────────────────────────────────────┘
```
[![Status](https://img.shields.io/badge/status-live_in_production-00FF88?style=for-the-badge&labelColor=000)](https://pleiades.kletech.ac.in)

[![Visit Pleiades](https://img.shields.io/badge/click_to_visit-D4AF37?style=for-the-badge&labelColor=000&logo=link&logoColor=white)](https://pleiades.kletech.ac.in)
</div>

---

## `whoami`

Pleiades is the official techno-cultural fest platform for **KLE Technological University, Hubballi** — built, architected, and shipped by a student team under real production constraints.

Not a demo. Not a hackathon prototype. A live system that handled thousands of concurrent users during active fest operations with zero downtime.

> Source code is private.  
> Architecture overview available on request.

---

## `cat ./scale`

```
PEAK LOAD        8,000+ concurrent users
DOWNTIME         zero — during active fest operations
DEPLOYMENT       live, continuously maintained
AUDIENCE         students, faculty, national participants
```

---

## `ls ./stack`

```
FRONTEND ──────────────────────────────────────────────────────
  Next.js 14        App Router          TypeScript
  Tailwind CSS      GSAP ScrollTrigger  Lenis smooth scroll
  Framer Motion     React Three Fiber   Custom animation pipeline

BACKEND ───────────────────────────────────────────────────────
  Node.js           REST API            Rate limiting
  JWT Auth          PostgreSQL          Complex relational queries

INFRA ─────────────────────────────────────────────────────────
  Nginx             PM2                 Linux VPS
  GitHub Actions    Environment configs
```

---

## `./engineering --what-was-hard`

```diff
# backend + infra

+ REST API with rate limiting — prevented abuse during registration spikes
+ JWT auth with session management across concurrent users
+ PostgreSQL query optimization — indexed lookups under load
+ Nginx reverse proxy config for zero-downtime deploys
+ PM2 cluster mode — utilized all CPU cores under peak traffic
+ environment-separated configs — dev / staging / prod pipeline

# frontend + performance

+ custom Lenis + GSAP ScrollTrigger integration without RAF conflicts
+ 60fps scroll pipeline maintained on low-end mobile devices
+ code splitting + lazy loading — reduced initial bundle size
+ horizontal overflow from marquee animations — fixed across all viewports
+ hero section scaling on short screens — no layout shift
+ modal scroll behavior consistent across all breakpoints
+ navbar collapse on mobile without jank or reflow

# scale

+ zero downtime during 8K+ concurrent user peak
+ no CDN — optimized static delivery through Nginx directly
+ real users, real load, real deadline — shipped on time
```

---

## `./architecture --overview`

```
  BROWSER
    │
    ▼
  Nginx  ──────────────────────────────────── static assets
    │
    ▼
  PM2 cluster (Next.js)
    │
    ├── App Router (SSR + SSG mixed strategy)
    ├── API routes (rate limited, JWT verified)
    │
    ▼
  PostgreSQL
    ├── event registration tables
    ├── user sessions
    └── indexed queries for concurrent reads

  FRONTEND RENDER PIPELINE
    Lenis (scroll) → GSAP ScrollTrigger → R3F scene → DOM
```

---

## `./live`

```bash
$ curl -I https://pleiades.kletech.ac.in

HTTP/2 200 OK
server: nginx
x-powered-by: Next.js
```

<div align="center">

[![Live Platform](https://img.shields.io/badge/view_live-pleiades.kletech.ac.in-FF3C3C?style=for-the-badge&logo=vercel&logoColor=white)](https://pleiades.kletech.ac.in)

</div>

---

## `ping`

<div align="center">

[![Email](https://img.shields.io/badge/workwarush%40gmail.com-FF3C3C?style=for-the-badge&logo=gmail&logoColor=white)](mailto:workwarush@gmail.com)
[![Portfolio](https://img.shields.io/badge/arushstack.dev-111?style=for-the-badge&logo=vercel&logoColor=white)](https://arushstack.dev)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/arush-talgeri-5bb866320)

</div>

---

<div align="center">

```
┌─────────────────────────────────────────────────────────────┐
│         Pleiades '26  •  KLE Technological University       │
│              built for scale. shipped on time.              │
└─────────────────────────────────────────────────────────────┘
```

*© 2026 Arush Talgeri. Source code is private.*

</div>
