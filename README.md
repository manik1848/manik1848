<h1 align="center">Manikandan Prakash</h1>

<p align="center">
  <b>Full-Stack Engineer</b> · Node.js · TypeScript · React · AWS<br>
  I build the parts that are hard to fake: HLS video pipelines, real-time dispatch, multi-tenant isolation.
</p>

<p align="center">
  <a href="https://manikprakash.netlify.app/">Portfolio</a> ·
  <a href="https://www.linkedin.com/in/manikandan-p-427237238/">LinkedIn</a> ·
  <a href="mailto:manikprakash1848@gmail.com">Email</a> ·
  <a href="https://www.npmjs.com/package/@manik1848/react-date-range-picker">npm</a>
</p>

---

### About

```typescript
const manik = {
  role: "Full-Stack Engineer @ Gravitorix Technologies",
  experience: "~4 years",
  based: "Erode, India. Remote, or Bengaluru for the right team.",
  philosophy: "Handle the hard cases in the design, not in a hotfix",
  askMeAbout: [
    "event-driven architecture", "multi-tenant data isolation",
    "video ingest and transcoding", "background job pipelines",
    "real-time systems at the socket layer",
  ],
};
```

I write backend systems that don't break at 3 AM, mobile apps that feel native, and
infrastructure that stays boring on purpose. Most of my work sits at the seams: where a
queue meets a state machine, where a tenant boundary has to fail closed, where a 4 GB
upload has to survive a flaky connection.

---

### What I've Built

**Multi-tenant SaaS**
A white-labelled school ERP, built end to end. Fastify and MongoDB backend with 202
endpoints across 42 models, three Next.js portals, an Expo mobile app. Tenant isolation
is enforced structurally in Mongoose middleware via `AsyncLocalStorage`, so a query
missing its filter fails closed rather than leaking another tenant's data. Also inside:
a dependency-closure IAM model spanning 19 modules and 39 actions, and a fee engine that
absorbs rounding remainders so instalment splits always reconcile to the total.

**Video Infrastructure**
Browser-to-S3 multipart ingest for multi-GB films, with adaptive chunk sizing and a
sliding window of upload workers. AWS MediaConvert HLS ladder behind a no-upscale guard,
so a 720p master never gets billed for renditions above it. AWS IVS live streaming
wired end to end, from stream key issue to playback.

**Event-Driven Fintech**
Kafka pipelines feeding ML inference into structured expense analytics. Million-record
merchant reports generated off the event loop using BullMQ, worker threads and MongoDB
cursors, so report generation never blocks the API. MQTT messaging out to payment
devices in the field.

**Real-Time Systems**
A BullMQ-backed dispatch state machine for ride-hailing, geospatial driver matching with
MongoDB `$geoNear` over a 2dsphere index, dual-mode background location on React Native,
and Socket.IO scaled horizontally with the Redis adapter. Debugging a silent WebSocket
upgrade failure through an APISIX gateway taught me more than any of it.

**Applied AI, and Knowing When to Quit**
Built a MediaPipe pose-warp engine for virtual try-on, measured it at roughly 30%
believable, and killed it. Moved to Vertex AI `virtual-try-on-001` and reached roughly
95% client-validated accuracy, then repurposed the MediaPipe work as a pre-upload pose
gate to cut inference spend. Throwing away your own working code is a skill.

---

### Public Work

Almost everything above lives in private company repositories, so this profile is
deliberately quiet. What is public:

**[`@manik1848/react-date-range-picker`](https://www.npmjs.com/package/@manik1848/react-date-range-picker)**
A Grafana-style date range picker for React. Predefined ranges plus absolute and
relative tabs, with `now`-anchored expressions.

**[`monorepo-bp`](https://github.com/manik1848/monorepo-bp)**
Turborepo boilerplate wiring Fastify, Next.js and Expo into one pnpm workspace with
shared types. The setup I reach for when starting anything real.

---

### Stack

**Core**
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white)
![Node.js](https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=nodedotjs&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)

**Backend**
![Fastify](https://img.shields.io/badge/Fastify-000000?style=for-the-badge&logo=fastify&logoColor=white)
![Express](https://img.shields.io/badge/Express-000000?style=for-the-badge&logo=express&logoColor=white)
![Socket.io](https://img.shields.io/badge/Socket.io-010101?style=for-the-badge&logo=socketdotio&logoColor=white)
![MQTT](https://img.shields.io/badge/MQTT-660066?style=for-the-badge&logo=mqtt&logoColor=white)

**Frontend & Mobile**
![React](https://img.shields.io/badge/React-61DAFB?style=for-the-badge&logo=react&logoColor=black)
![Next.js](https://img.shields.io/badge/Next.js-000000?style=for-the-badge&logo=nextdotjs&logoColor=white)
![React Native](https://img.shields.io/badge/React_Native-61DAFB?style=for-the-badge&logo=react&logoColor=black)
![Expo](https://img.shields.io/badge/Expo-000020?style=for-the-badge&logo=expo&logoColor=white)
![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-06B6D4?style=for-the-badge&logo=tailwindcss&logoColor=white)

**Data & Messaging**
![MongoDB](https://img.shields.io/badge/MongoDB-47A248?style=for-the-badge&logo=mongodb&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=for-the-badge&logo=redis&logoColor=white)
![Apache Kafka](https://img.shields.io/badge/Kafka-231F20?style=for-the-badge&logo=apachekafka&logoColor=white)
![BullMQ](https://img.shields.io/badge/BullMQ-E34F26?style=for-the-badge&logoColor=white)

**Infra**
![AWS](https://img.shields.io/badge/AWS-232F3E?style=for-the-badge&logo=amazonwebservices&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=for-the-badge&logo=githubactions&logoColor=white)
![Turborepo](https://img.shields.io/badge/Turborepo-EF4444?style=for-the-badge&logo=turborepo&logoColor=white)
![pnpm](https://img.shields.io/badge/pnpm-F69220?style=for-the-badge&logo=pnpm&logoColor=white)

---

<p align="center">
  Open to remote SDE-2 roles. Immediate joiner.<br>
  <a href="mailto:manikprakash1848@gmail.com">manikprakash1848@gmail.com</a>
</p>
