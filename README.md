<div align="center">

<sub>AI-ASSISTED FULL-STACK DEVELOPER · BANGKOK, THAILAND</sub>

<h1>Metee Thoenburin (Shuu)</h1>

<h3>Co-Founder & Founding Engineer @ <a href="https://unyhub.org">UNYHUB Automation</a></h3>

<p>I build LLM features that run in production — and put a second check in front of anything the model writes.<br />
<sub>Claude Code is my daily engineering workflow: I write the spec, review the diff and test every change.</sub></p>

<p>
  <a href="https://metee.vercel.app"><img src="https://img.shields.io/badge/Portfolio-metee.vercel.app-0a0d11?style=flat-square&logo=vercel&logoColor=white" alt="Portfolio" /></a>
  <a href="mailto:metee.thoe@gmail.com"><img src="https://img.shields.io/badge/Email-metee.thoe%40gmail.com-2563eb?style=flat-square&logo=gmail&logoColor=white" alt="Email" /></a>
  <img src="https://img.shields.io/badge/KKU%202026-First--Class%20Honours%20·%20GPA%203.81-eab308?style=flat-square" alt="First-Class Honours, GPA 3.81" />
  <img src="https://img.shields.io/badge/Available-immediately-16a34a?style=flat-square" alt="Available immediately" />
</p>

</div>

---

## What teams can evaluate quickly

<table width="100%">
<tr>
<td width="33%" valign="top">
<h3>🎯 Role fit</h3>
<p><strong>AI-Assisted Full-Stack Developer</strong><br />
<sub>Applied AI / LLM engineering on Next.js, TypeScript and Supabase.</sub></p>
</td>
<td width="33%" valign="top">
<h3>🔬 Public proof</h3>
<p><strong>3 open-source demos, live</strong><br />
<sub>Strict TypeScript, client-side, bring-your-own-key. Read the code, then try it.</sub></p>
</td>
<td width="33%" valign="top">
<h3>⚡ In production</h3>
<p><strong>2 AI products with real users</strong><br />
<sub>Bainy has paying customers · Unyna has 900+ LINE OA followers.</sub></p>
</td>
</tr>
</table>

<table width="100%">
<tr>
<td width="25%" align="center"><h2>2</h2><sub>AI products in production</sub></td>
<td width="25%" align="center"><h2>900+</h2><sub>LINE OA followers on Unyna</sub></td>
<td width="25%" align="center"><h2>3</h2><sub>open-source demos, live</sub></td>
<td width="25%" align="center"><h2>3.81</h2><sub>GPA · First-Class Honours</sub></td>
</tr>
</table>

---

## ⚡ Production work at UNYHUB

<sub>Closed source — these live in private company repositories. The live systems are linked.</sub>

| System | What it is | Engineering worth a look |
|---|---|---|
| 💳 **[Bainy](https://bainy.unyhub.org)** | LINE-native expense & accounting SaaS — **paying customers** | Receipt OCR (Sharp preprocessing + Gemini Flash) into a strict JSON schema, so the model classifies and the code does the arithmetic · Mini-CFO chat agent · multi-tenant, every query scoped to the organization · Beam payment subscriptions |
| 🩺 **[Unyna](https://unyna.unyhub.org)** | LINE health assistant for families — **900+ LINE OA followers** | Dual-witness vision for 7-segment blood-pressure displays: OpenAI Vision reads first, Google Vision is called only when the reading looks doubtful, and if the two disagree the user confirms — nothing is guessed |
| 🛡️ **SHUUVIS** | My personal command center for AI agents and production | Watches every Claude Code session live · a Cloudflare Worker health-checks each system every minute, opens a Discord incident, and an agent drafts the fix as a PR that only merges after I approve · local LLMs via Ollama |
| ⚡ **[Many](https://many.unyhub.org)** | Instagram comment-to-DM automation, used in-house | Deliberately **rule-based**, with no model in the decision path, so every rule can be read and audited · scheduled metric snapshots for content analysis |

---

## 🔬 Open-source demos

<sub>Small modules lifted out of real problems above, rebuilt in public.</sub>

<table width="100%">
<tr>
<td width="55%" valign="top">
<picture>
  <source media="(prefers-color-scheme: light)" srcset="https://www.gitskins.com/api/section/projects?username=Shuumei&theme=github-dark&avatar=https%3A%2F%2Favatars.githubusercontent.com%2Fu%2F283490304%3Fv%3D4&repos=Shuumei%2Focr-dual-witness-pipeline%2CShuumei%2Fedge-privacy-csv-analyst%2CShuumei%2Fllm-structured-booking-agent&v=recruiter-projects-2&mode=light" />
  <img src="https://www.gitskins.com/api/section/projects?username=Shuumei&theme=github-dark&avatar=https%3A%2F%2Favatars.githubusercontent.com%2Fu%2F283490304%3Fv%3D4&repos=Shuumei%2Focr-dual-witness-pipeline%2CShuumei%2Fedge-privacy-csv-analyst%2CShuumei%2Fllm-structured-booking-agent&v=recruiter-projects-2&mode=dark" width="100%" alt="Pinned open-source projects" />
</picture>
</td>
<td width="45%" valign="top">

**[ocr-dual-witness-pipeline](https://github.com/Shuumei/ocr-dual-witness-pipeline)**<br />
The public version of Unyna's 7-segment reader: two independent reads must agree, otherwise confidence gating asks the user instead of guessing.<br />
<sub><a href="https://ocr-dual-witness-pipeline.vercel.app">Live demo ↗</a></sub>

**[edge-privacy-csv-analyst](https://github.com/Shuumei/edge-privacy-csv-analyst)**<br />
Ask a spreadsheet questions in plain language. The work runs in browser Web Workers, and only summarized metadata ever reaches the LLM.<br />
<sub><a href="https://edge-privacy-csv-analyst.vercel.app">Live demo ↗</a></sub>

**[llm-structured-booking-agent](https://github.com/Shuumei/llm-structured-booking-agent)**<br />
Strict JSON Schema extraction drives a deterministic state machine with interval-overlap conflict checks, so double-booking can't happen · 19 Vitest unit tests.<br />
<sub><a href="https://llm-structured-booking-agent.vercel.app">Live demo ↗</a></sub>

</td>
</tr>
</table>

---

## 🧭 How I build with LLMs

> *"Deterministic when possible, probabilistic only when necessary."*

- **The model classifies; code does the arithmetic.** Every number is computed in code and checked by a schema (Zod) before it is saved.
- **A second reader that can object.** When a wrong answer is costly, a second read has to agree, and if it doesn't the user decides.
- **A human gate before production.** Agents may draft the fix, but nothing merges or deploys without approval.

---

## 💻 Toolkit

<sub>Grouped by area. The <a href="https://metee.vercel.app/#stack">stack section of my portfolio</a> shows where each tool was used.</sub>

**AI & LLM** &nbsp;
<img src="https://img.shields.io/badge/Claude%20Code-D97706?style=flat-square&logo=anthropic&logoColor=white" alt="Claude Code" />
<img src="https://img.shields.io/badge/OpenAI-412991?style=flat-square&logo=openai&logoColor=white" alt="OpenAI" />
<img src="https://img.shields.io/badge/Gemini-8E75B2?style=flat-square&logo=googlegemini&logoColor=white" alt="Gemini" />
<img src="https://img.shields.io/badge/Google%20Cloud%20Vision-4285F4?style=flat-square&logo=googlecloud&logoColor=white" alt="Google Cloud Vision" />
<img src="https://img.shields.io/badge/Zod-3E67B1?style=flat-square&logo=zod&logoColor=white" alt="Zod" />
<img src="https://img.shields.io/badge/Ollama-000000?style=flat-square&logo=ollama&logoColor=white" alt="Ollama" />
<img src="https://img.shields.io/badge/OpenCV-5C3EE8?style=flat-square&logo=opencv&logoColor=white" alt="OpenCV" />

**Frontend** &nbsp;
<img src="https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white" alt="TypeScript" />
<img src="https://img.shields.io/badge/Next.js-000000?style=flat-square&logo=nextdotjs&logoColor=white" alt="Next.js" />
<img src="https://img.shields.io/badge/React-20232A?style=flat-square&logo=react&logoColor=61DAFB" alt="React" />
<img src="https://img.shields.io/badge/Tailwind%20CSS-06B6D4?style=flat-square&logo=tailwindcss&logoColor=white" alt="Tailwind CSS" />
<img src="https://img.shields.io/badge/Astro-BC52EE?style=flat-square&logo=astro&logoColor=white" alt="Astro" />
<img src="https://img.shields.io/badge/Three.js-000000?style=flat-square&logo=threedotjs&logoColor=white" alt="Three.js" />
<img src="https://img.shields.io/badge/WebAssembly-654FF0?style=flat-square&logo=webassembly&logoColor=white" alt="WebAssembly" />

**Backend & data** &nbsp;
<img src="https://img.shields.io/badge/Node.js-339933?style=flat-square&logo=nodedotjs&logoColor=white" alt="Node.js" />
<img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white" alt="PostgreSQL" />
<img src="https://img.shields.io/badge/Supabase%20(RLS)-3ECF8E?style=flat-square&logo=supabase&logoColor=white" alt="Supabase" />
<img src="https://img.shields.io/badge/Prisma-2D3748?style=flat-square&logo=prisma&logoColor=white" alt="Prisma" />
<img src="https://img.shields.io/badge/SQLite-003B57?style=flat-square&logo=sqlite&logoColor=white" alt="SQLite" />
<img src="https://img.shields.io/badge/Upstash%20Redis-00E9A3?style=flat-square&logo=upstash&logoColor=black" alt="Upstash Redis" />
<img src="https://img.shields.io/badge/PHP%20·%20Laravel-FF2D20?style=flat-square&logo=laravel&logoColor=white" alt="Laravel" />
<img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white" alt="Python" />

**Cloud & ops** &nbsp;
<img src="https://img.shields.io/badge/Vercel-000000?style=flat-square&logo=vercel&logoColor=white" alt="Vercel" />
<img src="https://img.shields.io/badge/Cloudflare%20Workers-F38020?style=flat-square&logo=cloudflare&logoColor=white" alt="Cloudflare Workers" />
<img src="https://img.shields.io/badge/Google%20Cloud-4285F4?style=flat-square&logo=googlecloud&logoColor=white" alt="Google Cloud" />
<img src="https://img.shields.io/badge/Sentry-362D59?style=flat-square&logo=sentry&logoColor=white" alt="Sentry" />
<img src="https://img.shields.io/badge/Tailscale-242424?style=flat-square&logo=tailscale&logoColor=white" alt="Tailscale" />
<img src="https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white" alt="Git" />

**Platforms & APIs** &nbsp;
<img src="https://img.shields.io/badge/LINE%20Messaging%20API%20·%20LIFF-00C300?style=flat-square&logo=line&logoColor=white" alt="LINE Messaging API and LIFF" />
<img src="https://img.shields.io/badge/Beam%20Payments-0f172a?style=flat-square" alt="Beam Payment Gateway" />
<img src="https://img.shields.io/badge/Meta%20Graph%20API-0668E1?style=flat-square&logo=meta&logoColor=white" alt="Meta Graph API" />
<img src="https://img.shields.io/badge/Discord%20API-5865F2?style=flat-square&logo=discord&logoColor=white" alt="Discord API" />
<img src="https://img.shields.io/badge/Figma-F24E1E?style=flat-square&logo=figma&logoColor=white" alt="Figma" />

---

<table width="100%">
<tr>
<td width="62%" valign="middle">
<h3>Let's talk about the next build</h3>
<p>Open to <strong>AI-Assisted Full-Stack Developer</strong> and <strong>Applied AI / LLM Engineering</strong> roles on teams shipping AI features to real users. Available immediately, based in Bangkok.</p>
</td>
<td width="38%" valign="middle" align="right">
  <a href="https://metee.vercel.app">Portfolio ↗</a><br />
  <a href="mailto:metee.thoe@gmail.com">metee.thoe@gmail.com</a><br />
  <a href="https://github.com/Shuumei">github.com/Shuumei</a>
</td>
</tr>
</table>
