<!--
████████████████████████████████████████████████████████████
  ADITYA RAJ — github.com/Aditgm
  Terminal / Hacker Aesthetic README
  
  HOW STATS WORK (no more broken images):
  ─────────────────────────────────────────────────────────
  GitHub Stats & Top Languages:
    → Self-host in 3 min: fork anuraghazra/github-readme-stats
      → deploy to Vercel → add PAT_1 env var → replace URL below
    → Until then: uses GitHub Actions to generate static SVGs
      (see readme-update.yml workflow)
  
  Streak Stats:
    → Self-host: fork DenverCoder1/github-readme-streak-stats
      → switch to `vercel` branch → deploy to Vercel → add TOKEN env var
    → Until then: demolab.com with herokuapp fallback

  Pac-Man Graph:
    → Uses abozanona/pacman-contribution-graph (NOT platane/snk)
    → See readme-update.yml — run it once to populate `output` branch
████████████████████████████████████████████████████████████
-->

<div align="center">

<!-- ══════════════════════════════════════════════
     ANIMATED TERMINAL HEADER
══════════════════════════════════════════════ -->

<img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=700&size=15&duration=2200&pause=500&color=00FF41&background=0d0d0d&center=true&vCenter=true&multiline=true&width=760&height=130&lines=%24+whoami+%23+aditya_raj+%7C+SWE+%7C+AI%2FML+%7C+Competitive+Programmer;%24+curl+--rating+codeforces%2Faditya2005+%23+2131+%E2%80%94+Master+%7C+%2356+India;%24+grep+-c+%22problems%22+.%2Fsolved%2F*+%23+2000%2B+results;%24+echo+%22Open+to+SDE+Internships+2025%E2%80%9326+%E2%96%AE%22" alt="Terminal Typing SVG" />

```
╔══════════════════════════════════════════════════════════════╗
║  $ whoami                                                    ║
║    aditya_raj — SWE · AI/ML · Competitive Programmer         ║
║  $ uname -a                                                  ║
║    DIT University · B.Tech CSE (AI/ML) · GPA 8.41            ║
║  $ echo $STATUS                                              ║
║    Open to SDE Internships · Building cool stuff ▮          ║
╚══════════════════════════════════════════════════════════════╝
```

<!-- PLATFORM BADGES -->
<a href="https://codeforces.com/profile/aditya2005"><img src="https://img.shields.io/badge/Codeforces-MASTER_|_2131_|_%2356_India-00FF41?style=flat-square&logo=codeforces&logoColor=00FF41&labelColor=0d0d0d&color=0d0d0d"/></a>
<a href="https://leetcode.com/u/adityagm/"><img src="https://img.shields.io/badge/LeetCode-GUARDIAN_|_2360%2B_|_Top_0.4%25-00FF41?style=flat-square&logo=leetcode&logoColor=00FF41&labelColor=0d0d0d&color=0d0d0d"/></a>
<a href="https://www.codechef.com/users/adityagm"><img src="https://img.shields.io/badge/CodeChef-5★_|_2132_|_335th_India-00FF41?style=flat-square&logo=codechef&logoColor=00FF41&labelColor=0d0d0d&color=0d0d0d"/></a>

<br/><br/>

<a href="https://linkedin.com/in/aditya-raj-18401a377"><img src="https://img.shields.io/badge/LinkedIn-connect-00FF41?style=flat-square&logo=linkedin&logoColor=00FF41&labelColor=0d0d0d&color=0d0d0d"/></a>
<a href="mailto:arajsinha4@gmail.com"><img src="https://img.shields.io/badge/Gmail-arajsinha4@gmail.com-00FF41?style=flat-square&logo=gmail&logoColor=00FF41&labelColor=0d0d0d&color=0d0d0d"/></a>
<a href="https://portfolio-chi-taupe-70.vercel.app/"><img src="https://img.shields.io/badge/Portfolio-live_site-00FF41?style=flat-square&logo=vercel&logoColor=00FF41&labelColor=0d0d0d&color=0d0d0d"/></a>

</div>

---

## `$ cat /proc/stats`

<div align="center">

| `KEY` | `VALUE` |
|:---|:---|
| `CF_RATING` | **2131 — Master** · 56th in India · Top 0.8% globally |
| `LC_RATING` | **2360+ — Guardian** · Top 0.4% · #169 / 30,000+ in Contest 462 |
| `CC_RATING` | **2132 — 5★** · 335th in India |
| `PROBLEMS_SOLVED` | **2,000+** across CF · LC · CSES · VJudge · HackerRank |
| `BEST_FINISH` | **45 / 20,000+** CF Round 1068 Div.2 — Top 0.003% globally |
| `AMAZON_ML` | Selected — Top **5% of 60,000+** applicants |

</div>

---

## `$ cat ~/.profile`

```typescript
// ~/.config/aditya/profile.ts

const dev = {
  name:        "Aditya Raj",
  location:    "Dehradun, India 🇮🇳",
  education:   "B.Tech CSE (AI/ML) @ DIT University · GPA 8.41",
  focus:       ["System Design", "Distributed Systems", "LLM Infrastructure"],
  stack:       ["Full-Stack", "RAG Pipelines", "Vector DBs", "PWA", "DevOps"],
  cp:          "CF Master 2131 · LC Guardian 2360+ · 2000+ problems",
  seeking:     "SDE Internships 2025–26",
  principle:   "Measure twice. `git push --force` once.",
} satisfies Engineer;

export default dev;
```

---

## `$ ls -la ./projects/`

<details>
<summary><b><code>📁 DIT-PYQ-Hub/</code></b> &nbsp;—&nbsp; Full-Stack Academic Resource Platform (PWA)</summary>

<br/>

```bash
$ cat DIT-PYQ-Hub/README.md
```

> Production-grade PWA for browsing, uploading and downloading university question papers.

```
ARCHITECTURE
├── frontend/   React 18 + TypeScript + TanStack Query v5 + Workbox 7.x
├── backend/    Node.js + Express + Supabase RLS + PL/pgSQL triggers
├── infra/      DigitalOcean + GitHub Actions CI/CD + SSH zero-downtime deploy
└── security/   Rate limiting · Zod validation · watermarked delivery
```

**Key engineering decisions:**
- `O(1)` download counters via PL/pgSQL triggers — eliminated expensive `COUNT(*)` queries
- Offline-first: Workbox multi-strategy caching (`NetworkFirst` · `CacheFirst` · `StaleWhileRevalidate`)
- Sub-50ms UI sync: TanStack Query v5 optimistic updates + Supabase Realtime `postgres_changes`
- 99.9% uptime · 5 req/3hr rate limiting · Bearer token injection with row-level security

![React](https://img.shields.io/badge/React_18-0d0d0d?style=flat-square&logo=react&logoColor=00FF41) ![TypeScript](https://img.shields.io/badge/TypeScript-0d0d0d?style=flat-square&logo=typescript&logoColor=00FF41) ![PostgreSQL](https://img.shields.io/badge/PostgreSQL-0d0d0d?style=flat-square&logo=postgresql&logoColor=00FF41) ![Supabase](https://img.shields.io/badge/Supabase-0d0d0d?style=flat-square&logo=supabase&logoColor=00FF41) ![Express](https://img.shields.io/badge/Express.js-0d0d0d?style=flat-square&logo=express&logoColor=00FF41) ![DigitalOcean](https://img.shields.io/badge/DigitalOcean-0d0d0d?style=flat-square&logo=digitalocean&logoColor=00FF41) ![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-0d0d0d?style=flat-square&logo=github-actions&logoColor=00FF41) ![Workbox](https://img.shields.io/badge/Workbox-0d0d0d?style=flat-square&logo=googlechrome&logoColor=00FF41) ![TanStack](https://img.shields.io/badge/TanStack_Query_v5-0d0d0d?style=flat-square&logo=reactquery&logoColor=00FF41) ![Zod](https://img.shields.io/badge/Zod-0d0d0d?style=flat-square&logo=zod&logoColor=00FF41)

</details>

<details>
<summary><b><code>📁 Legal-Lens/</code></b> &nbsp;—&nbsp; AI-Powered Legal Research Platform (RAG)</summary>

<br/>

```bash
$ cat Legal-Lens/README.md
```

> RAG pipeline making statutory research accessible to everyone.

```
ARCHITECTURE
├── model/      Llama 3.3 70B via Groq · LangChain orchestration
├── retrieval/  Pinecone Vector DB · 1,000+ chunked legal documents
├── frontend/   Next.js 14 + TypeScript
└── backend/    MongoDB persistence · optimized API response caching
```

**Key metrics:** Sub-150ms query latency · **92% top-k retrieval accuracy** · ~85% reduction in research time

![Next.js](https://img.shields.io/badge/Next.js_14-0d0d0d?style=flat-square&logo=nextdotjs&logoColor=00FF41) ![TypeScript](https://img.shields.io/badge/TypeScript-0d0d0d?style=flat-square&logo=typescript&logoColor=00FF41) ![Pinecone](https://img.shields.io/badge/Pinecone_VectorDB-0d0d0d?style=flat-square&logo=pinecone&logoColor=00FF41) ![MongoDB](https://img.shields.io/badge/MongoDB-0d0d0d?style=flat-square&logo=mongodb&logoColor=00FF41) ![Llama](https://img.shields.io/badge/Llama_3.3_70B-0d0d0d?style=flat-square&logo=meta&logoColor=00FF41) ![LangChain](https://img.shields.io/badge/LangChain-0d0d0d?style=flat-square&logo=langchain&logoColor=00FF41) ![Vercel](https://img.shields.io/badge/Vercel-0d0d0d?style=flat-square&logo=vercel&logoColor=00FF41)

</details>

<details>
<summary><b><code>📁 Dengue-Spot/</code></b> &nbsp;—&nbsp; Real-Time Disease Surveillance Platform</summary>

<br/>

```bash
$ cat Dengue-Spot/README.md
```

> Community-driven public health platform with live geo-tagged risk mapping.

```
ARCHITECTURE
├── realtime/   Socket.io bi-directional chat + live alert broadcasting
├── cv/         Roboflow pipeline — auto-classifies mosquito breeding sites
├── maps/       Leaflet.js + indexed MongoDB geospatial queries
└── security/   RBAC + Rate Limiting + IP Banning + OAuth 2.0 + JWT
```

![MongoDB](https://img.shields.io/badge/MongoDB-0d0d0d?style=flat-square&logo=mongodb&logoColor=00FF41) ![React](https://img.shields.io/badge/React-0d0d0d?style=flat-square&logo=react&logoColor=00FF41) ![Socket.io](https://img.shields.io/badge/Socket.io-0d0d0d?style=flat-square&logo=socketdotio&logoColor=00FF41) ![Python](https://img.shields.io/badge/Python-0d0d0d?style=flat-square&logo=python&logoColor=00FF41) ![Roboflow](https://img.shields.io/badge/Roboflow_CV-0d0d0d?style=flat-square&logo=roboflow&logoColor=00FF41) ![Leaflet](https://img.shields.io/badge/Leaflet.js-0d0d0d?style=flat-square&logo=leaflet&logoColor=00FF41) ![JWT](https://img.shields.io/badge/JWT_Auth-0d0d0d?style=flat-square&logo=jsonwebtokens&logoColor=00FF41)

</details>

---

## `$ cat /etc/tech-stack`

<div align="center">

<img src="https://skillicons.dev/icons?i=cpp,python,ts,js,bash&theme=dark" />
&nbsp;&nbsp;
<img src="https://skillicons.dev/icons?i=react,nextjs,tailwind,vite,html,css&theme=dark" />
&nbsp;&nbsp;
<img src="https://skillicons.dev/icons?i=nodejs,express,graphql&theme=dark" />

<br/><br/>

<img src="https://skillicons.dev/icons?i=postgres,mongodb,redis,supabase&theme=dark" />
&nbsp;&nbsp;
<img src="https://skillicons.dev/icons?i=pytorch,tensorflow&theme=dark" />
&nbsp;&nbsp;
<img src="https://skillicons.dev/icons?i=docker,githubactions,nginx,linux,git,postman&theme=dark" />

<br/><br/>

![TanStack Query](https://img.shields.io/badge/TanStack_Query-0d0d0d?style=flat-square&logo=reactquery&logoColor=00FF41)
![Zustand](https://img.shields.io/badge/Zustand-0d0d0d?style=flat-square&logo=react&logoColor=00FF41)
![Framer Motion](https://img.shields.io/badge/Framer_Motion-0d0d0d?style=flat-square&logo=framer&logoColor=00FF41)
![Radix UI](https://img.shields.io/badge/Radix_UI-0d0d0d?style=flat-square&logo=radixui&logoColor=00FF41)
![PWA](https://img.shields.io/badge/PWA_%2B_Workbox-0d0d0d?style=flat-square&logo=pwa&logoColor=00FF41)
![Zod](https://img.shields.io/badge/Zod-0d0d0d?style=flat-square&logo=zod&logoColor=00FF41)
![REST API](https://img.shields.io/badge/REST_API-0d0d0d?style=flat-square&logo=fastapi&logoColor=00FF41)
![WebSockets](https://img.shields.io/badge/WebSockets_%2F_Socket.io-0d0d0d?style=flat-square&logo=socketdotio&logoColor=00FF41)
![JWT](https://img.shields.io/badge/JWT_Auth-0d0d0d?style=flat-square&logo=jsonwebtokens&logoColor=00FF41)
![OAuth2](https://img.shields.io/badge/OAuth_2.0-0d0d0d?style=flat-square&logo=auth0&logoColor=00FF41)
![PL/pgSQL](https://img.shields.io/badge/PL%2FpgSQL-0d0d0d?style=flat-square&logo=postgresql&logoColor=00FF41)
![Prisma](https://img.shields.io/badge/Prisma_ORM-0d0d0d?style=flat-square&logo=prisma&logoColor=00FF41)
![Llama 3.3 70B](https://img.shields.io/badge/Llama_3.3_70B-0d0d0d?style=flat-square&logo=meta&logoColor=00FF41)
![RAG Pipelines](https://img.shields.io/badge/RAG_Pipelines-0d0d0d?style=flat-square&logo=openai&logoColor=00FF41)
![Pinecone](https://img.shields.io/badge/Pinecone_VectorDB-0d0d0d?style=flat-square&logo=pinecone&logoColor=00FF41)
![LangChain](https://img.shields.io/badge/LangChain-0d0d0d?style=flat-square&logo=langchain&logoColor=00FF41)
![HuggingFace](https://img.shields.io/badge/HuggingFace-0d0d0d?style=flat-square&logo=huggingface&logoColor=00FF41)
![Gemini](https://img.shields.io/badge/Google_Gemini-0d0d0d?style=flat-square&logo=google&logoColor=00FF41)
![Roboflow](https://img.shields.io/badge/Roboflow_CV-0d0d0d?style=flat-square&logo=roboflow&logoColor=00FF41)
![DigitalOcean](https://img.shields.io/badge/DigitalOcean-0d0d0d?style=flat-square&logo=digitalocean&logoColor=00FF41)
![Vercel](https://img.shields.io/badge/Vercel-0d0d0d?style=flat-square&logo=vercel&logoColor=00FF41)
![SSH Deploy](https://img.shields.io/badge/SSH_Zero--Downtime-0d0d0d?style=flat-square&logo=gnubash&logoColor=00FF41)

</div>

---

## `$ ./leaderboard.sh --competitive`

<div align="center">

<a href="https://codeforces.com/profile/aditya2005">
  <img src="https://codeforces-readme-stats.vercel.app/api/card?username=aditya2005&theme=dark&show_icons=true&border_color=00FF41&title_color=00FF41&icon_color=00FF41&text_color=c9d1d9&bg_color=0d0d0d" alt="Codeforces Stats"/>
</a>

<br/><br/>

```
┌──────────────────┬──────────────────┬──────────────────────────────────┐
│  PLATFORM        │  RATING          │  HIGHLIGHT                       │
├──────────────────┼──────────────────┼──────────────────────────────────┤
│  Codeforces      │  2131 — Master   │  56th India · Top 0.8% global    │
│  LeetCode        │  2360+ — Guard.  │  #169/30K · Top 0.4% global      │
│  CodeChef        │  2132 — 5★       │  335th India                     │
│  Problems        │  2000+           │  CF · LC · CSES · VJudge · HR    │
│  Best Finish     │  45 / 20,000+    │  Top 0.003% — CF Round 1068      │
└──────────────────┴──────────────────┴──────────────────────────────────┘
```

</div>

---

## `$ neofetch --github`

<div align="center">

<!--
  ════════════════════════════════════════════════════════════
  GITHUB STATS — HOW TO FIX PERMANENTLY (takes 3 minutes)

  The public github-readme-stats.vercel.app hits rate limits
  because millions of users share the same GitHub API token.

  FIX:
  1. Go to: github.com/anuraghazra/github-readme-stats
  2. Click "Fork" (top right)
  3. Go to vercel.com → "Add New Project" → import your fork
  4. In Environment Variables add:  PAT_1 = <your GitHub PAT>
     (generate at: github.com/settings/tokens → classic token
      scope: just check "public_repo" — no other permissions needed)
  5. Click Deploy. Copy your URL (e.g. my-stats.vercel.app)
  6. Replace "github-readme-stats.vercel.app" below with your URL

  Until you do that, the workflow (readme-update.yml) generates
  static SVG snapshots into your `output` branch as fallback.
  ════════════════════════════════════════════════════════════
-->

<!-- Stats + Languages — replace github-readme-stats.vercel.app with YOUR self-hosted URL -->
<img height="175em"
  src="https://github-readme-stats.vercel.app/api?username=Aditgm&show_icons=true&count_private=true&include_all_commits=true&theme=chartreuse-dark&hide_border=false&border_color=00FF41&bg_color=0d0d0d&title_color=00FF41&icon_color=00FF41&text_color=c9d1d9&ring_color=00FF41&cache_seconds=21600"
  alt="GitHub Stats"/>
&nbsp;
<img height="175em"
  src="https://github-readme-stats.vercel.app/api/top-langs/?username=Aditgm&layout=compact&langs_count=8&theme=chartreuse-dark&hide_border=false&border_color=00FF41&bg_color=0d0d0d&title_color=00FF41&text_color=c9d1d9&cache_seconds=21600"
  alt="Top Languages"/>

<br/><br/>

<!--
  ════════════════════════════════════════════════════════════
  STREAK STATS — HOW TO FIX PERMANENTLY (takes 3 minutes)

  demolab.com is a community Heroku server — goes down sometimes.

  FIX:
  1. Go to: github.com/DenverCoder1/github-readme-streak-stats
  2. Fork it. Switch your fork to the `vercel` branch (important!)
  3. Deploy to vercel.com → add env var:  TOKEN = <your GitHub PAT>
     (same PAT as above works fine)
  4. Copy your URL and replace "streak-stats.demolab.com" below.
  ════════════════════════════════════════════════════════════
-->

<!-- Streak Stats — replace streak-stats.demolab.com with YOUR self-hosted URL -->
<img
  src="https://streak-stats.demolab.com?user=Aditgm&theme=dark&hide_border=false&border=00FF41&background=0d0d0d&ring=00FF41&fire=00FF41&currStreakLabel=00FF41&sideLabels=c9d1d9&currStreakNum=c9d1d9&sideNums=c9d1d9&dates=555555&stroke=00FF41"
  alt="GitHub Streak Stats"/>

<br/><br/>

<!-- Activity Graph — this one is generally reliable -->
<img
  src="https://github-readme-activity-graph.vercel.app/graph?username=Aditgm&bg_color=0d0d0d&color=00FF41&line=00FF41&point=ffffff&area=true&area_color=003300&hide_border=false&border_color=00FF41&custom_title=%5BAditgm%5D%20contribution%20log"
  alt="Activity Graph"/>

</div>

---

## `$ git log --all --oneline --graph`

<div align="center">

<!--
  Pac-Man graph is generated by the readme-update.yml workflow.
  Run the workflow ONCE from Actions tab → it creates the `output` branch.
  After that it auto-runs every 24h. SVG file names are EXACTLY as below.
-->

<picture>
  <source media="(prefers-color-scheme: dark)"
          srcset="https://raw.githubusercontent.com/Aditgm/Aditgm/output/pacman-contribution-graph-dark.svg">
  <source media="(prefers-color-scheme: light)"
          srcset="https://raw.githubusercontent.com/Aditgm/Aditgm/output/pacman-contribution-graph.svg">
  <img alt="Pac-Man Contribution Graph"
       src="https://raw.githubusercontent.com/Aditgm/Aditgm/output/pacman-contribution-graph-dark.svg"/>
</picture>

<br/>

```
$ git log --format="%h %s" --since="1 year ago" | head -52
```

<img src="https://ghchart.rshah.org/00FF41/Aditgm" alt="GitHub Contribution Chart"/>

</div>

---

## `$ cat /var/log/achievements.log`

<div align="center">

```
[2024] Amazon ML Summer School ............ SELECTED · Top 5% of 60,000+
[2024] GirlScript Summer of Code .......... Contributor · Node.js / Python
[2024] Codeforces Round 1068 Div.2 ........ 45 / 20,000+ · Top 0.003%
[2024] LeetCode Weekly Contest 462 ........ #169 / 30,000+
[LIVE] Codeforces ......................... Master · 2131 · 56th India
[LIVE] LeetCode ........................... Guardian · 2360+ · Top 0.4%
[LIVE] CodeChef ........................... 5★ · 2132 · 335th India
[LIVE] Topics ............................. Graphs · DP · SegTree · Flows · FFT
```

</div>

---

<div align="center">

```
╔══════════════════════════════════════════════════════════════╗
║                                                              ║
║   Open to SDE Internship opportunities                       ║
║   $ ping arajsinha4@gmail.com --message "let's build" ▮     ║
║                                                              ║
╚══════════════════════════════════════════════════════════════╝
```

<img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&size=12&duration=4000&pause=1200&color=00FF41&background=00000000&center=true&vCenter=true&width=600&lines=%24+logout+%23+session+terminated+%C2%B7+github.com%2FAditgm" />

[![](https://visitcount.itsvg.in/api?id=Aditgm&icon=6&color=0)](https://visitcount.itsvg.in)

</div>
