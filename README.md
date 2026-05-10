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

### 📞 Heyfield — AI Voice Receptionist for Home Service Businesses

<p>
  <img src="https://img.shields.io/badge/Heyfield-AI%20Voice%20Receptionist-0F172A?style=for-the-badge&logo=phone&logoColor=22c55e" />
  <img src="https://img.shields.io/badge/Status-In%20Production-16a34a?style=for-the-badge" />
</p>

A production AI receptionist purpose-built for plumbers, HVAC, electricians and field service crews. 24/7 voice agent that books jobs, qualifies leads and never lets a call go to voicemail.

**Highlights**

- Realtime voice agent powered by **Retell AI** with custom tools
- **Auto appointment scheduling** — agent finds open slots and books on the call
- **Two-way Google Calendar sync** — real-time availability, no double-booking
- Per-business knowledge base: pricing, service area, hours, recurring jobs
- Multi-tenant SaaS with call transcripts, AI summaries and CRM-ready handoffs

```typescript
const heyfield = {
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
  webhook --> transcripts[Transcripts & AI Summaries]
  transcripts --> db

  db --> dashboard[Next.js Dashboard]
```

---

### 📈 RevTune — AI Pricing Engine for SaaS

<p>
  <img src="https://img.shields.io/badge/RevTune-AI%20Pricing%20Engine-020617?style=for-the-badge&logo=stripe&logoColor=635BFF" />
  <img src="https://img.shields.io/badge/Status-In%20Production-16a34a?style=for-the-badge" />
</p>

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

```mermaid
flowchart TB
  stripe[Stripe / Paddle / LemonSqueezy / Chargebee] --> connect[OAuth & API Key Connectors]
  connect --> sync[Inngest Sync Jobs]
  webhooks[Billing Webhooks] --> sync

  sync --> normalize[Normalization Layer]
  normalize --> db[(Neon PostgreSQL)]

  db --> metrics[Metrics Engine - MRR, Churn, LTV]
  db --> elasticity[Price Elasticity Model]
  db --> stats[Statistical Significance Layer]

  elasticity --> ai[Claude AI Pricing Engine]
  stats --> ai
  ai --> insights[Proven Recommendations & Weekly Brief]

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
| 🚀 **Production SaaS Shipped** | 2 (Heyfield + RevTune) |
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
