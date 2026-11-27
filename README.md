### Chekuri Satyanarayana Raja Varma

AI/ML engineering student (B.Tech CSE, AI & ML, GITAM University) building full-stack web applications, local-first AI tools and automation software.

I work mostly on privacy-preserving desktop and browser tools, role-based web platforms, and applied algorithms: search, optimisation, constraint satisfaction and classical ML.

**Domains:** Full-stack web · Local LLM tooling · Desktop and browser automation · Applied AI algorithms · Web application security

[Portfolio](https://rajavarma.site) · [Repositories](https://github.com/chsrajavarma8?tab=repositories)

---

#### Languages

<img src="https://skillicons.dev/icons?i=py,ts,js,html,css,java,c,cpp,powershell" alt="Python, TypeScript, JavaScript, HTML, CSS, Java, C, C++, PowerShell" />

SQL: PostgreSQL (PL/pgSQL migrations, RLS policies), SQLite

#### Stack

| Area | Technologies |
|---|---|
| Frontend | <img src="https://skillicons.dev/icons?i=react,nextjs,vite,tailwind" alt="React, Next.js, Vite, Tailwind CSS" /><br/>shadcn/ui (Radix), React Hook Form, Zod, Chrome Extensions (Manifest V3) |
| Backend | <img src="https://skillicons.dev/icons?i=nodejs,express,fastapi" alt="Node.js, Express, FastAPI" /><br/>Socket.IO, Mongoose, Next.js Server Actions, Python `http.server` |
| Databases | <img src="https://skillicons.dev/icons?i=postgres,supabase,mongodb,sqlite" alt="PostgreSQL, Supabase, MongoDB, SQLite" /> |
| AI / ML | <img src="https://skillicons.dev/icons?i=sklearn,opencv" alt="scikit-learn, OpenCV" /><br/>Ollama (local LLMs), Pandas, NumPy, Matplotlib, NetworkX |
| Desktop | PySide6 (Qt), Win32 APIs (global hotkeys, clipboard, text capture), PyInstaller |
| Cloud / DevOps | <img src="https://skillicons.dev/icons?i=vercel,docker,githubactions,linux" alt="Vercel, Docker, GitHub Actions, Linux" /><br/>Docker Compose, Vercel serverless functions, Supabase CLI migrations |
| Security | JWT and cookie sessions, bcrypt, Helmet, rate limiting, Postgres Row Level Security, Content Security Policy, SRI, HIBP k-anonymity |
| Testing | Vitest, Testing Library, Supertest, mongodb-memory-server, pytest, `unittest` |
| Tools | <img src="https://skillicons.dev/icons?i=git,github,vscode,figma" alt="Git, GitHub, VS Code, Figma" /> |

---

#### Selected Projects

**[LocalWrite](https://github.com/chsrajavarma8/localwrite)**: A Windows writing assistant that runs entirely against a local Ollama server. A global hotkey captures the selected text in any application, and the correction is shown as a word-level diff in a popup that never takes focus. Before pasting the result back, it checks that the original window and selection haven't changed, and it restores the clipboard afterwards. Text is never persisted or logged, and requests bypass system proxies.<br/>
`Python` `PySide6` `Ollama` `Win32 API` `PyInstaller` `pytest`

**[Hackathon Platform](https://github.com/chsrajavarma8/zing)** · [demo](https://zing-lemon.vercel.app): A configurable hackathon system with a public site, team registration, a participant portal and a role-based admin panel (super admin, event admin, reviewer). There is no public sign-up: users join through invitation links. Access control is enforced in Postgres with Row Level Security, the schema is managed through numbered SQL migrations, and the scheduler is dispatched by `pg_cron`. Signed storage uploads and admin CSV exports are handled by route handlers.<br/>
`TypeScript` `Next.js 16` `Supabase` `PostgreSQL` `shadcn/ui` `Tailwind CSS v4` `Zod`

**[Token Kitchen](https://github.com/chsrajavarma8/token)** · [demo](https://token-psi-lime.vercel.app): A real-time order-token system with Owner and Chef roles and a `NEW → IN_PROCESS → COMPLETED` workflow, updated live over Socket.IO. Orders are written in MongoDB transactions, which require a replica set. Authentication uses PINs with JWTs in strict same-site cookies, behind Helmet and rate limiting. The Docker Compose deployment runs the app as a non-root user and uses a least-privilege database user.<br/>
`React` `Vite` `Tailwind` `Express` `MongoDB` `Socket.IO` `Docker` `Vitest` `Supertest`

**[JARVIS Mark 85 Recovery](https://github.com/chsrajavarma8/jarvis-mark85-recovery)**: An AI algorithms lab that chains three solvers, each feeding its result into the next, with automatic replanning:
- Uniform Cost Search (`heapq`) for power routing
- Simulated Annealing for resource allocation
- A backtracking CSP scheduler with MRV, degree heuristic and forward checking

A JSON API built on `ThreadingHTTPServer` serves a React and htm frontend with no build step. There are 19 unit, integration and API tests.<br/>
`Python` `React` `matplotlib` `NetworkX` `unittest`

**[Mailer](https://github.com/chsrajavarma8/mailer)**: A bulk SMTP mailer built only on the Python standard library, with a local web dashboard, a CLI and a single-file `.exe`. It detects the CSV delimiter and email column automatically and fills `{{placeholder}}` templates. Temporary 4xx failures are retried with exponential backoff, while permanent 5xx failures are not. A rolling 24-hour quota is enforced, campaigns can resume without sending anyone a duplicate, and the stored credentials are encrypted. CI runs the tests on Windows and Ubuntu with Python 3.9 and 3.13.<br/>
`Python` `SMTP` `GitHub Actions` `PowerShell`

**[WhatsApp Web Campaign Extension](https://github.com/chsrajavarma8/WhatsApp-Web-campaign-extension)**: A Manifest V3 Chrome extension that sends personalised messages one at a time to consenting contacts listed in a CSV. It is built from a service worker, content scripts and a DOM selector layer, and uses `chrome.alarms` to keep start-to-start pacing across worker restarts. It also includes a CSV parser that handles quoted fields and multiple encodings, plus drafts, templates and CSV export. Permissions are limited to `storage`, `alarms` and `web.whatsapp.com`.<br/>
`JavaScript` `Chrome Extensions API` `Node.js`

**[Secure Password Checker](https://github.com/chsrajavarma8/secure-password-checker)** · [demo](https://secure-password-checker.vercel.app): A client-side password analyser and generator.
- **Strength:** zxcvbn estimates, with crack times for online and offline attacks.
- **Breach check:** Have I Been Pwned queries with k-anonymity (SHA-1 prefix) and padded responses.
- **Generator:** `crypto.getRandomValues` with rejection sampling.
- **Hardening:** a strict CSP (`default-src 'none'`), a dependency vendored and pinned with SRI, and no `innerHTML`.

`JavaScript` `Web Crypto API` `CSP`

---

#### Open-Source Contributions

| Repository | Pull request | Status |
|---|---|---|
| [usememos/memos](https://github.com/usememos/memos) | [#6482](https://github.com/usememos/memos/pull/6482): feat(web): add a split view with a memo list beside the open memo | Open |
| [twbs/bootstrap](https://github.com/twbs/bootstrap) | [#43117](https://github.com/twbs/bootstrap/pull/43117): Combobox: add `showChips` option to render multiple selections as chips | Closed |
| [twbs/bootstrap](https://github.com/twbs/bootstrap) | [#43116](https://github.com/twbs/bootstrap/pull/43116): Fix alert text centering and CSS Grid docs | Closed |

---

#### GitHub Activity

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://github-readme-stats.vercel.app/api?username=chsrajavarma8&show_icons=true&include_all_commits=true&hide_border=true&disable_animations=true&bg_color=0d1117&title_color=e6edf3&text_color=8b949e&icon_color=8b949e&ring_color=e6edf3" />
  <img height="165" src="https://github-readme-stats.vercel.app/api?username=chsrajavarma8&show_icons=true&include_all_commits=true&hide_border=true&disable_animations=true&bg_color=ffffff&title_color=1f2328&text_color=59636e&icon_color=59636e&ring_color=1f2328" alt="GitHub stats" />
</picture>
<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://github-readme-stats.vercel.app/api/top-langs/?username=chsrajavarma8&layout=compact&langs_count=8&hide_border=true&disable_animations=true&bg_color=0d1117&title_color=e6edf3&text_color=8b949e" />
  <img height="165" src="https://github-readme-stats.vercel.app/api/top-langs/?username=chsrajavarma8&layout=compact&langs_count=8&hide_border=true&disable_animations=true&bg_color=ffffff&title_color=1f2328&text_color=59636e" alt="Most used languages" />
</picture>

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://streak-stats.demolab.com?user=chsrajavarma8&hide_border=true&disable_animations=true&background=0d1117&ring=e6edf3&fire=e6edf3&currStreakNum=e6edf3&sideNums=e6edf3&currStreakLabel=8b949e&sideLabels=8b949e&dates=6e7681&stroke=30363d" />
  <img src="https://streak-stats.demolab.com?user=chsrajavarma8&hide_border=true&disable_animations=true&background=ffffff&ring=1f2328&fire=1f2328&currStreakNum=1f2328&sideNums=1f2328&currStreakLabel=59636e&sideLabels=59636e&dates=8c959f&stroke=d0d7de" alt="Contribution streak" />
</picture>

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://github-readme-activity-graph.vercel.app/graph?username=chsrajavarma8&hide_border=true&bg_color=0d1117&color=8b949e&title_color=e6edf3&line=e6edf3&point=8b949e&area=true&area_color=30363d" />
  <img src="https://github-readme-activity-graph.vercel.app/graph?username=chsrajavarma8&hide_border=true&bg_color=ffffff&color=59636e&title_color=1f2328&line=1f2328&point=59636e&area=true&area_color=d0d7de" alt="Contribution activity graph" />
</picture>

---

#### Current Focus

- **Local LLM tooling:** offline inference with Ollama and system-wide text integration on Windows ([LocalWrite](https://github.com/chsrajavarma8/localwrite)).
- **Browser automation:** Manifest V3 extension architecture and resilient DOM automation ([campaign extension](https://github.com/chsrajavarma8/WhatsApp-Web-campaign-extension)).
- **Upstream contributions:** frontend features for open-source web applications ([memos#6482](https://github.com/usememos/memos/pull/6482)).
- **Secure backend design:** Postgres RLS, invitation-only auth flows and transactional data models.
