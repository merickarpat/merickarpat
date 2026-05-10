<div align="center">
<!-- HEADER -->
<img width="100%" src="https://capsule-render.vercel.app/api?type=waving&color=0:25bfff,100:9600ff&height=200&section=header&text=Meri%C3%A7%20Karpat&fontSize=48&fontColor=ffffff&animation=twinkling" />
</div>

<!-- INTRO -->
<p align="center">
  <a href="https://github.com/merickarpat">
    <img src="https://readme-typing-svg.herokuapp.com?size=24&duration=4000&pause=800&color=3B82F6&center=true&vCenter=true&width=650&lines=Full+Stack+TypeScript+Engineer;SaaS+Founder;AI-powered+Platforms;Heyfield+%7C+AI+Voice+Receptionist;RevTune+%7C+AI+Pricing+Engine+for+SaaS" />
  </a>
</p>

---

## 🚀 What I'm Shipping

### <img src="assets/heyfield-icon.svg" width="28" align="absmiddle" /> Heyfield — AI Voice Receptionist for Home Service Businesses

<p>
  <a href="https://heyfield.app"><img src="https://img.shields.io/badge/Live-heyfield.app-22c55e?style=for-the-badge&logo=googlechrome&logoColor=white" /></a>
  <img src="https://img.shields.io/badge/Status-In%20Production-16a34a?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Stack-Next.js%2016%20·%20Retell%20AI%20·%20Twilio-0F172A?style=for-the-badge" />
</p>

🔗 **Live at [heyfield.app](https://heyfield.app)**

A production AI receptionist purpose-built for plumbers, HVAC, electricians and field service crews. 24/7 voice agent that books jobs, qualifies leads and never lets a call go to voicemail.

**Highlights**

- Realtime voice agent powered by **Retell AI** with custom tools
- **Auto appointment scheduling** — agent finds open slots and books on the call
- **Two-way Google Calendar sync** — real-time availability, no double-booking
- Per-business knowledge base: pricing, service area, hours, recurring jobs
- Multi-tenant SaaS with call transcripts, AI summaries and CRM-ready handoffs

```typescript
const heyfield = {
  url: "https://heyfield.app",
  problem: "Home service businesses miss calls = lost jobs",
  solution: "24/7 AI voice agent that books jobs and captures leads",
  tech: [
    "Next.js 16 (App Router, React 19)",
    "Neon PostgreSQL + Drizzle ORM",
    "Clerk (multi-tenant auth)",
    "Retell AI (realtime voice agent)",
    "Twilio + Google Calendar + Stripe",
  ],
  status: "Live with home service operators",
};
```

<h4 align="center">⏬ Heyfield Architecture ⏬</h4>

<p align="center">
  <img src="https://mermaid.ink/svg/Zmxvd2NoYXJ0IFRCCiAgY2FsbGVyW0N1c3RvbWVyIENhbGxzIEJ1c2luZXNzIE51bWJlcl0gLS0+IHR3aWxpb1tUd2lsaW8gVGVsZXBob255XQogIHR3aWxpbyAtLT4gcmV0ZWxsW1JldGVsbCBBSSAtIFJlYWx0aW1lIFZvaWNlIEFnZW50XQogIHJldGVsbCAtLT4ga2JbKFBlci1CdXNpbmVzcyBLbm93bGVkZ2UgQmFzZSldCiAgcmV0ZWxsIC0tPiB0b29sc1tDdXN0b20gVG9vbHM6IENoZWNrIEF2YWlsYWJpbGl0eSwgQm9vaywgUXVvdGUsIFRyYW5zZmVyXQogIHRvb2xzIC0tPiBhcGlbTmV4dC5qcyBBUEkgUm91dGVzXQogIGFwaSAtLT4gZGJbKE5lb24gUG9zdGdyZVNRTCldCiAgYXBpIDwtLT4gZ2NhbFtHb29nbGUgQ2FsZW5kYXIgLSBUd28tV2F5IFN5bmNdCiAgZ2NhbCAtLT4gc2NoZWR1bGVyW0F1dG8gQXBwb2ludG1lbnQgU2NoZWR1bGVyXQogIHNjaGVkdWxlciAtLT4gZGIKICByZXRlbGwgLS0+IHdlYmhvb2tbUG9zdC1DYWxsIFdlYmhvb2tdCiAgd2ViaG9vayAtLT4gdHJhbnNjcmlwdHNbVHJhbnNjcmlwdHMgYW5kIEFJIFN1bW1hcmllc10KICB0cmFuc2NyaXB0cyAtLT4gZGIKICBkYiAtLT4gZGFzaGJvYXJkW05leHQuanMgRGFzaGJvYXJkXQo" alt="Heyfield Architecture" />
</p>

<details>
<summary>View diagram source (Mermaid)</summary>

```mermaid
flowchart TB
  caller[Customer Calls Business Number] --> twilio[Twilio Telephony]
  twilio --> retell[Retell AI - Realtime Voice Agent]
  retell --> kb[(Per-Business Knowledge Base)]
  retell --> tools[Custom Tools: Check Availability, Book, Quote, Transfer]
  tools --> api[Next.js API Routes]
  api --> db[(Neon PostgreSQL)]
  api <--> gcal[Google Calendar - Two-Way Sync]
  gcal --> scheduler[Auto Appointment Scheduler]
  scheduler --> db
  retell --> webhook[Post-Call Webhook]
  webhook --> transcripts[Transcripts and AI Summaries]
  transcripts --> db
  db --> dashboard[Next.js Dashboard]
```

</details>

---

### <img src="assets/revtune-icon.svg" width="28" align="absmiddle" /> RevTune — AI Pricing Engine for SaaS

<p>
  <a href="https://revtune.io"><img src="https://img.shields.io/badge/Live-revtune.io-7c5fd6?style=for-the-badge&logo=googlechrome&logoColor=white" /></a>
  <img src="https://img.shields.io/badge/Status-In%20Production-16a34a?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Stack-Next.js%2016%20·%20Claude%20AI%20·%20Inngest-020617?style=for-the-badge" />
</p>

🔗 **Live at [revtune.io](https://revtune.io)**

An AI pricing intelligence platform for SaaS founders and indie hackers. Connect Stripe, Paddle, LemonSqueezy or Chargebee and get statistically-proven pricing recommendations — not vibes.

**Highlights**

- One-click Stripe Connect; Paddle, LemonSqueezy and **Chargebee** via API key
- **Price elasticity modeling** — data-driven sensitivity curves per plan and segment
- **Statistically-proven AI recommendations** — every suggestion backed by significance tests
- **Experiment engine** — A/B pricing tests with statistical significance & confidence intervals
- **Revenue forecasting** — predicted MRR impact, actual vs predicted tracker
- Weekly AI Brief email — the single most impactful pricing action of the week

```typescript
const revtune = {
  url: "https://revtune.io",
  problem: "30-50% of SaaS companies are underpriced",
  solution: "Connect Stripe. Get statistically-proven pricing recommendations.",
  tech: [
    "Next.js 16 (App Router, React 19)",
    "Neon PostgreSQL + Drizzle ORM",
    "Clerk + Stripe Connect (OAuth)",
    "Inngest (sync + AI pipelines)",
    "Claude API + Vercel AI SDK",
  ],
  status: "Live — Stripe / Paddle / LemonSqueezy / Chargebee",
};
```

<h4 align="center">⏬ RevTune Architecture ⏬</h4>

<p align="center">
  <img src="https://mermaid.ink/svg/Zmxvd2NoYXJ0IFRCCiAgc3RyaXBlW1N0cmlwZSAvIFBhZGRsZSAvIExlbW9uU3F1ZWV6eSAvIENoYXJnZWJlZV0gLS0+IGNvbm5lY3RbT0F1dGggYW5kIEFQSSBLZXkgQ29ubmVjdG9yc10KICBjb25uZWN0IC0tPiBzeW5jW0lubmdlc3QgU3luYyBKb2JzXQogIHdlYmhvb2tzW0JpbGxpbmcgV2ViaG9va3NdIC0tPiBzeW5jCiAgc3luYyAtLT4gbm9ybWFsaXplW05vcm1hbGl6YXRpb24gTGF5ZXJdCiAgbm9ybWFsaXplIC0tPiBkYlsoTmVvbiBQb3N0Z3JlU1FMKV0KICBkYiAtLT4gbWV0cmljc1tNZXRyaWNzIEVuZ2luZSAtIE1SUiwgQ2h1cm4sIExUVl0KICBkYiAtLT4gZWxhc3RpY2l0eVtQcmljZSBFbGFzdGljaXR5IE1vZGVsXQogIGRiIC0tPiBzdGF0c1tTdGF0aXN0aWNhbCBTaWduaWZpY2FuY2UgTGF5ZXJdCiAgZWxhc3RpY2l0eSAtLT4gYWlbQ2xhdWRlIEFJIFByaWNpbmcgRW5naW5lXQogIHN0YXRzIC0tPiBhaQogIGFpIC0tPiBpbnNpZ2h0c1tQcm92ZW4gUmVjb21tZW5kYXRpb25zIGFuZCBXZWVrbHkgQnJpZWZdCiAgZGIgLS0+IGV4cGVyaW1lbnRzW0V4cGVyaW1lbnQgRW5naW5lIC0gQS9CIFRlc3RzXQogIHN0YXRzIC0tPiBleHBlcmltZW50cwogIGRiIC0tPiBmb3JlY2FzdFtSZXZlbnVlIEZvcmVjYXN0aW5nXQogIGV4cGVyaW1lbnRzIC0tPiBpbXBhY3RbQWN0dWFsIHZzIFByZWRpY3RlZCBUcmFja2VyXQogIGZvcmVjYXN0IC0tPiBpbXBhY3QKICBpbnNpZ2h0cyAtLT4gcmVzZW5kW1Jlc2VuZCBFbWFpbF0KICBtZXRyaWNzIC0tPiBkYXNoYm9hcmRbTmV4dC5qcyBEYXNoYm9hcmRdCiAgaW5zaWdodHMgLS0+IGRhc2hib2FyZAogIGV4cGVyaW1lbnRzIC0tPiBkYXNoYm9hcmQKICBmb3JlY2FzdCAtLT4gZGFzaGJvYXJkCiAgaW1wYWN0IC0tPiBkYXNoYm9hcmQKICBlbGFzdGljaXR5IC0tPiBkYXNoYm9hcmQK" alt="RevTune Architecture" />
</p>

<details>
<summary>View diagram source (Mermaid)</summary>

```mermaid
flowchart TB
  stripe[Stripe / Paddle / LemonSqueezy / Chargebee] --> connect[OAuth and API Key Connectors]
  connect --> sync[Inngest Sync Jobs]
  webhooks[Billing Webhooks] --> sync
  sync --> normalize[Normalization Layer]
  normalize --> db[(Neon PostgreSQL)]
  db --> metrics[Metrics Engine - MRR, Churn, LTV]
  db --> elasticity[Price Elasticity Model]
  db --> stats[Statistical Significance Layer]
  elasticity --> ai[Claude AI Pricing Engine]
  stats --> ai
  ai --> insights[Proven Recommendations and Weekly Brief]
  db --> experiments[Experiment Engine - A/B Tests]
  stats --> experiments
  db --> forecast[Revenue Forecasting]
  experiments --> impact[Actual vs Predicted Tracker]
  forecast --> impact
  insights --> resend[Resend Email]
  metrics --> dashboard[Next.js Dashboard]
  insights --> dashboard
  experiments --> dashboard
  forecast --> dashboard
  impact --> dashboard
  elasticity --> dashboard
```

</details>

---

## 🧠 Tech Arsenal

<p align="left">
  <img src="https://skillicons.dev/icons?i=ts,nextjs,react,nodejs,postgres,redis,tailwind,vercel,docker,git,vscode,cloudflare" />
</p>

**Strong Focus Areas**

- **End-to-end TypeScript systems** — Next.js 16, React 19, strict TS
- **Multi-tenant SaaS architecture** — Clerk orgs, scoped data, billing
- **AI product engineering** — Retell AI voice agents, Claude API, RAG
- **Statistically-grounded ML** — elasticity modeling, significance testing, confidence intervals
- **Postgres at scale** — Drizzle ORM, schema design, migrations on Neon
- **Async pipelines** — Inngest jobs, webhooks, cron, retries

---

## 📊 Real Impact

| Metric | Value |
|--------|-------|
| 🚀 **Production SaaS Shipped** | 2 ([Heyfield](https://heyfield.app) + [RevTune](https://revtune.io)) |
| 📞 **Voice AI Calls Handled** | 24/7 via Retell AI for home service operators |
| 📅 **Appointments Booked** | Auto-scheduled with two-way Google Calendar sync |
| 💳 **Billing Platforms Integrated** | Stripe, Paddle, LemonSqueezy, Chargebee |
| 📈 **Pricing Recommendations** | Statistically-proven, elasticity-driven, A/B tested |
| ⚡ **API Response Time** | <200ms (p95) |

---

## 🏗️ Architecture Philosophy

> **"Build for scale from day one, optimize for developer experience always."**

- **Type-safe everything** — TypeScript end-to-end, Zod validation, Drizzle types
- **AI-first product thinking** — voice agents, structured LLM output, evals
- **Statistically grounded** — no advice without significance, no forecasts without confidence intervals
- **Observability built-in** — Sentry, structured logging, PostHog funnels
- **Zero-downtime deploys** — Vercel CI/CD, gradual rollouts
- **Cost-conscious scaling** — cache aggressively, batch AI calls, edge where it matters

---

## 💡 Side Interests

- **Realtime voice AI** — latency budgets, barge-in, tool-use during calls
- **Pricing & monetization** — willingness-to-pay, geo pricing, packaging
- **Developer tools** — internal CLIs, codegen, AI-assisted workflows
- **Vector search & RAG** — pgvector indexes for sub-second retrieval

---

## 📫 Let's Build Something

<p>
  <a href="mailto:meric.karpat@icloud.com"><img src="https://img.shields.io/badge/Email-meric.karpat%40icloud.com-D14836?style=for-the-badge&logo=gmail&logoColor=white" /></a>
  <a href="https://linkedin.com/in/meric-karpat"><img src="https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" /></a>
  <a href="https://www.google.com/maps/place/Izmir"><img src="https://img.shields.io/badge/Location-Izmir%2C%20Turkey-00ADD8?style=for-the-badge&logo=google-maps&logoColor=white" /></a>
</p>

**Open to:**

- 🤝 Technical co-founders for AI/SaaS projects
- 💼 Contract work or consulting on complex backend systems
- 🎙️ Speaking about SaaS architecture & AI integration
- ☕ Coffee chats about startup ideas

---

<div align="center">

### "Ship fast, iterate faster, never stop learning."

⭐ If you find my work interesting, feel free to reach out or star my public repos!

</div>

<!-- FOOTER -->
<img width="100%" src="https://capsule-render.vercel.app/api?type=waving&color=0:25bfff,100:9600ff&height=150&section=footer" />
