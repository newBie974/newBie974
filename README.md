<div align="center">

# Aymeric Dijoux

**Agentic developer — I ship production apps with agents, and I publish the method.**

Paris, France · Remote worldwide

[![Portfolio](https://img.shields.io/badge/aymeric.dijoux.dev-000000?style=flat-square&logo=vercel&logoColor=white)](https://aymeric.dijoux.dev)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=flat-square&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/aymeric-dijoux)
[![X](https://img.shields.io/badge/X-000000?style=flat-square&logo=x&logoColor=white)](https://x.com/AymericDijoux)
[![Instagram](https://img.shields.io/badge/Instagram-E4405F?style=flat-square&logo=instagram&logoColor=white)](https://www.instagram.com/aymeric.builder)
[![TikTok](https://img.shields.io/badge/TikTok-000000?style=flat-square&logo=tiktok&logoColor=white)](https://www.tiktok.com/@aymeric.builder)
[![Email](https://img.shields.io/badge/Email-D14836?style=flat-square&logo=gmail&logoColor=white)](mailto:aymericelie.dijoux@gmail.com)

</div>

---

Most people talk about building with AI. I'd rather show you the files.

**Four apps in production**, designed, built and shipped solo — through App Store review, with paying users. All of them built the same way: a written contract the agents work against, hard limits they can't negotiate, and gates that reject anything the types and tests don't back.

That method is below, and the artifacts are public. Steal any of it.

---

### 🧠 How I Build

I don't prompt my way to features. Every repo starts with a **`CLAUDE.md` contract** — 700 to 1400 lines of architecture, invariants and non-negotiable limits. The agent reads it before writing a line, and it's the same document I review against. No contract, no code.

**The rules are identical across every project I ship:**

| Constraint | Why it holds |
|---|---|
| **120 lines max per file** · 20 per function | The real reason isn't taste — it's that I reason better about code I can hold in context at once, and so does the model. Large files are where agent edits go wrong. |
| **Architectural invariants, stated up front** | Every project declares 2-4 things that must never be violated (*"everything is scoped to `householdId`, never `userId` alone"*). Agents drift; invariants are what they drift against. |
| **Strict TypeScript, zero `any`** | The type checker is the cheapest reviewer I have, and the only one that never gets tired at 2am. |
| **Explicit test scope — including what we don't test** | Naming what stays untested in an MVP is what keeps the suite honest instead of decorative. |
| **A written "not in v1" list** | Scope creep is the default failure mode of an agent that wants to be helpful. The refusal list is part of the contract. |
| **A commit checklist the agent runs itself** | Verification before the claim, every time. "It works" is not a result. |

**Beyond the contract:** specialized sub-agents with narrow jobs and defined hand-offs · MCP servers so the model reasons on real state instead of guesses · reference files the agent **appends to itself** after each run, so the next session starts where the last one ended.

That last one is the pattern I'd hand anyone first — it's the difference between an agent that repeats your work and one that compounds it. My App Store memo below is 400 lines that no human sat down to write; it accumulated, one submission at a time.

---

### 📂 Public Artifacts

The method above, as files you can read and run:

| Artifact | What's in it |
|---|---|
| **[skills](https://github.com/newBie974/skills)** | Five Claude Code skills, three carrying their own reference file. Including **`app-store-review`** — 650 lines of App Store Connect answers and review traps accumulated across four submissions, and **`claude-md-init`**, which writes the contract below by reading your codebase first. |
| **[claude-md-templates](https://github.com/newBie974/claude-md-templates)** | The `CLAUDE.md` contracts behind my shipped apps, stripped of product logic. React Native + Expo on Convex, and on Supabase. The spine, not the secrets. |

---

### 🚀 Shipped & Live

| App | What it does | Stack |
|---|---|---|
| **[Noan](https://apps.apple.com/fr/app/noan-lorganisation-famille/id6793809327)** | Family organisation that redistributes the mental load — so it's not always the same person remembering | React Native · Expo · Convex |
| **[VoiceJournal](https://apps.apple.com/fr/app/voicejournal-journal-vocal-ia/id6762176421)** | Turn your voice into a daily journal, powered by AI | React Native · Expo · Supabase · Claude |
| **[Ti Boug](https://tiboug.re)** | Fights the cost of living in Réunion — which fruits & vegetables are cheap, when, and where | React Native · Expo · Convex · Gemini |
| **[Tookta](https://tookta.fr)** | Find the perfect activity for your kids, effortlessly | Flutter · NestJS · Typesense |

---

### 🛠️ Tech

**Agentic** &ensp;
![Claude](https://img.shields.io/badge/Claude-D97757?style=flat-square&logo=anthropic&logoColor=white)
![Claude Code](https://img.shields.io/badge/Claude_Code-D97757?style=flat-square&logo=anthropic&logoColor=white)
![MCP](https://img.shields.io/badge/MCP-1A1A1A?style=flat-square&logo=modelcontextprotocol&logoColor=white)
![LangGraph](https://img.shields.io/badge/LangGraph-1C3C3C?style=flat-square&logo=langgraph&logoColor=white)
![Cursor](https://img.shields.io/badge/Cursor-000000?style=flat-square&logo=cursor&logoColor=white)

**Mobile** &ensp;
![React Native](https://img.shields.io/badge/React_Native-61DAFB?style=flat-square&logo=react&logoColor=black)
![Expo](https://img.shields.io/badge/Expo-000020?style=flat-square&logo=expo&logoColor=white)
![Flutter](https://img.shields.io/badge/Flutter-02569B?style=flat-square&logo=flutter&logoColor=white)

**Web** &ensp;
![Next.js](https://img.shields.io/badge/Next.js-000000?style=flat-square&logo=nextdotjs&logoColor=white)
![Astro](https://img.shields.io/badge/Astro-BC52EE?style=flat-square&logo=astro&logoColor=white)
![Tailwind](https://img.shields.io/badge/Tailwind-06B6D4?style=flat-square&logo=tailwindcss&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)

**Backend & Data** &ensp;
![Convex](https://img.shields.io/badge/Convex-EE342F?style=flat-square&logo=convex&logoColor=white)
![Supabase](https://img.shields.io/badge/Supabase-3FCF8E?style=flat-square&logo=supabase&logoColor=white)
![NestJS](https://img.shields.io/badge/NestJS-E0234E?style=flat-square&logo=nestjs&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![Typesense](https://img.shields.io/badge/Typesense-1A1A1A?style=flat-square&logo=typesense&logoColor=white)

**Payments & Tooling** &ensp;
![RevenueCat](https://img.shields.io/badge/RevenueCat-F2545B?style=flat-square&logo=revenuecat&logoColor=white)
![Stripe](https://img.shields.io/badge/Stripe-635BFF?style=flat-square&logo=stripe&logoColor=white)
![Linear](https://img.shields.io/badge/Linear-5E6AD2?style=flat-square&logo=linear&logoColor=white)
![Figma](https://img.shields.io/badge/Figma-F24E1E?style=flat-square&logo=figma&logoColor=white)

---

### 📍 Now

- Growing four live apps and listening hard to users
- Publishing the harness piece by piece — skills, contracts, and the traps I hit
- Writing about agentic development in FR & EN on [aymeric.dijoux.dev](https://aymeric.dijoux.dev)

---

### 🤝 Work with me

Open to contracts, consulting & technical partnerships:

- **Agentic systems & automation** — I design the harness your team codes inside: `CLAUDE.md` contracts, skills, MCP integrations, quality gates. The goal is leverage that survives contact with production.
- **MVP in 6–8 weeks** — from Figma to the App Store. Mobile (RN/Flutter) or web (Next/Astro).
- **AI prototype in 2 weeks** — you have an AI app idea, I ship a working proto so you can decide.
- **Tech rescue mission** — your team is stuck. I come in, unblock, leave.
- **Consulting / pair design** — 90-min sessions on architecture, stack and agentic workflow.

<div align="center">

**Let's build something →** [aymeric.dijoux.dev](https://aymeric.dijoux.dev)

[![Email](https://img.shields.io/badge/aymericelie.dijoux@gmail.com-D14836?style=flat-square&logo=gmail&logoColor=white)](mailto:aymericelie.dijoux@gmail.com)
[![LinkedIn](https://img.shields.io/badge/aymeric--dijoux-0A66C2?style=flat-square&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/aymeric-dijoux)

</div>
