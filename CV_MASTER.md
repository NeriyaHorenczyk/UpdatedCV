# CV Master File — Neriya Horenczyk

**Never send this file to anyone.** This is the inventory you fork from.
The one-page PDF is one export of this document, not the source of truth.

Last updated: September 2026

Next review: December 2026 (after NOX changes ship and The Island beta completes)

---

## How to use this

1. Read the job posting. Note which of the two profiles it wants: **web/full-stack** or **systems/backend/C++**.
2. Copy the base layout below into your template.
3. Apply the matching swap from "Tailoring swaps."
4. Pull any extra detail from the long-form sections as space allows.
5. Keep it to one page. Every addition needs a corresponding cut.

**Base section order (main column):** Summary → Experience → Projects → Education → Military Service
**Sidebar order:** Contact → Links → Skills → Languages

---

## Tailoring swaps

**For full-stack / web roles (default, widest net):**

- Summary as written below (full-stack leads, C++ second)
- Avatar Management Platform is the headline achievement
- Consider expanding the ShiftWise capstone clause under Education
- Languages line order: JavaScript/TypeScript, C++, Python, Java, C#

**For C++ / backend / systems roles:**

- Flip summary sentences 1 and 2 so C++ leads
- Move The Island above the Avatar Platform in visual weight
- Languages line order: C++, Python, Java, C#, JavaScript/TypeScript

**For anything in Hebrew:** you don't have a Hebrew version yet. Worth building one — a meaningful share of Israeli postings ask for it. Add it here when you do.

---

## Contact

- Neriya Horenczyk
- Software Developer
- 054-9255602
- neriyahoren@gmail.com
- City: *(decide per application — left off the current version. Use your home city, not Jerusalem, since Jerusalem is the office and it may cost you center-based roles on commute assumptions.)*
- github.com/NeriyaHorenczyk
- linkedin.com/in/nhorenczyk/

---

## Summary

**Current version (full-stack lead) — 3 lines:**

> Computer Science graduate and software developer at the Israel Police cyber-crime unit, building production full-stack systems in TypeScript, React and Node. Architect a licensed Unreal Engine 5 title in C++ alongside a two-person team. Autodidactic and fast-learning, with experience picking up unfamiliar codebases and stacks.

**Systems/C++ lead variant:**

> Computer Science graduate and software developer who architects a licensed Unreal Engine 5 title in C++ alongside a two-person team. Builds production full-stack systems in TypeScript, React and Node at the Israel Police cyber-crime unit. Autodidactic and fast-learning, with experience picking up unfamiliar codebases and stacks.

**Short version (2 lines, when space is tight):**

> Computer Science graduate and software developer at the Israel Police cyber-crime unit, building production full-stack systems in TypeScript, React and Node, and architecting a licensed Unreal Engine 5 title in C++.

**Why this works, so you don't undo it later:** the original summary described what you *wanted* (eager to start, seeking to integrate, hoping to make impact). Every junior CV says that. This one says what you *are* and puts "software developer at the Israel Police" in the first seven words. "Production" is deliberate — it separates you from candidates whose only code was graded.

---

## Experience

### Software Developer, Cyber Crimes Unit — Israel Police, Jerusalem
**March 2026 – Present**

Lead line:
> Develop and maintain internal systems supporting cyber-crime investigations.

**Avatar Management Platform** *(internal codename: Ghost / GhostV3 — do not use the codename on a CV)*

CV version:
> Full-stack platform for managing virtual personas and their social-media accounts (React, TypeScript, Node/Express, PostgreSQL/Prisma). JWT and role-based access control, containerized for air-gapped deployment.

Full detail for interviews:

- Full-stack TypeScript, React front end, Node/Express API, PostgreSQL via Prisma
- JWT auth with role-based access control
- Ships as Docker images for air-gapped/offline environments — no external network dependency
- Groq API integration
- Built as work product, not a side project

**OSINT Investigation Platform** *(internal codename: NOX — do not use the codename on a CV)*

**Not CV-ready yet.** Inherited September 2026. Add a line once you've shipped 2–3 concrete changes — realistically December 2026 or later.

Situation: ~2-year-old codebase, dormant, no original authors available. Handed to you to learn, own, and improve. ~111 architecturally significant files, ~36,000 lines.

Stack (do **not** list these on the CV until you've genuinely worked in them — an interviewer will ask you to write Cypher or explain the queue):

- Python / FastAPI (async), Neo4j graph DB + Cypher, RabbitMQ
- React / Vite / TypeScript, TailwindCSS, Shadcn UI
- Separate Firecrawl scraping microservice
- Docker Compose multi-service deployment
- LLM integration (OpenRouter, local LM Studio)
- DomainTools API, multi-stage scanning pipeline, graph-based entity relationship mapping, PDF report generation

Draft line for when you've earned it:
> Took ownership of a dormant OSINT investigation platform (Python/FastAPI, Neo4j, RabbitMQ, React/TypeScript); reconstructed the architecture from an undocumented codebase and [shipped X, Y, Z].

**Write-up discipline for both police systems:** describe stack and architecture, never detection capability, case detail, or what the system can and cannot find. Run any final wording past your team lead. Cheap to clear internally; the alternative isn't.

**Running change log — add a line a week:**
```
2026-09-xx  —
2026-09-xx  —
```

---

## Projects

### The Island — Unreal Engine 5 Game (Cerva Studios)

CV version:
> C++ gameplay systems architecture for a licensed adventure game, developed in partnership with the original broadcaster; entering beta with ~100 external testers. Designed a data-driven story-progression subsystem for state persistence across streamed levels, an interface-based interaction system, and a generic condition-gating framework. Directing a two-person team and integrating third-party plugins into an existing codebase.

Additional detail for interviews:

- GameInstanceSubsystem chosen specifically because it survives level streaming
- Data-driven room IDs (`FName`) rather than an enum, so designers can extend without a code change
- Generic condition-gating framework instead of one-off classes per story event
- GameplayTags for branching narrative logic; designer (Daniel) works in the data layer
- Story Framework plugin (Steven Mayer / VisOne Projects) migrated and integrated
- Diversion version control, multi-branch workflow with per-collaborator branches
- Beta testers coordinated via TheIslandBetaTesters@gmail.com with Gmail filtering
- Blender pipeline for skeletal mesh prep, bone renaming, Mixamo-to-Manny

**Why the framing matters:** "C++ gameplay systems architecture" leads, not "game." The broadcaster partnership is what separates this from a hobby project — someone signed a contract with you, which very few juniors can say. The beta is your only shipping evidence, and shipping outranks building.

### ShiftWise — Full-Stack Shift Scheduling Platform (academic capstone)

Currently lives as a one-line clause under Education. Full version if you need a third project or a full-stack-heavy CV:
> Full-stack shift-scheduling platform (React, Express, MySQL, Socket.IO) with role-based access, availability-based auto-scheduling, a swap and leave approval workflow, real-time notifications, and an AI schedule auditor built on Llama 3.1.

Note: keep the auto-scheduling and Socket.IO detail — that's your real-time and algorithm evidence, and nothing else on the CV covers it.

### Aura — UE5 / Gameplay Ability System

**Do not put this on a CV.** It's Stephen Ulibarri's Udemy GAS course project. The architecture is his, not yours, and anyone in game dev who has touched GAS recognizes the name instantly. Listing it reads as "followed a tutorial," which is worse than having nothing.

Where it *does* belong — the interview answer to "how did you learn C++ and GAS":

- Worked through GAS, Enhanced Input, Niagara, Sequencer in depth
- Built a custom MVC widget architecture on top
- Then applied those patterns to your own architecture in The Island

Becomes a real project entry **if** you build and ship the GAS debugger/visualizer tool on FAB. A tool other developers install is yours in a way a course project never is. Scoped at ~4–8 weeks.

---

## Education

### B.Sc. Computer Science, JCT Lev Academic Center
**2022 – 2026**

> Main project — ShiftWise: full-stack shift-scheduling platform (React, Express, MySQL, Socket.IO) with availability-based auto-scheduling and real-time notifications.

GPA 80 — **leave it off.** Israeli rule of thumb: a GPA earns its space at 85+. Below that it can only cost you. Absence is unremarkable; most CVs omit it. If a company wants grades they'll request a transcript at screening, and handing it over then is normal.

Also completed a full-stack web development course at JCT (Prof. Shlomo Kipnis).

---

## Military Service

### Iron Dome Air Defense System — Battle Interceptor Operator
**2019 – 2022**

> Operated a complex real-time defense system under live operational conditions, making time-critical decisions as part of a rotating crew.

Covers the "works under pressure" claim with evidence instead of adjectives. Add rank at discharge only if it was a commander or instructor role.

---

## Skills inventory

**On the CV now:**

| Group | Items |
|---|---|
| Languages | C++, Python, Java, JavaScript/TypeScript, C# |
| Frameworks & Tools | Docker, NodeJS, React, Git/GitHub, Unreal Engine 5 |
| Databases | PostgreSQL, MySQL |

**Held back until you can be interviewed on them:** FastAPI, Neo4j/Cypher, RabbitMQ, Firecrawl, Prisma (arguably ready now — it's in the Avatar Platform line).

**Not on the CV, available if a posting asks:** Express, Socket.IO, Vite, TailwindCSS, Shadcn UI, Blender, Diversion, JetBrains Rider, Visual Studio, VS Code, Android Studio, GAS, Enhanced Input, Niagara, Sequencer.

**Deliberately cut, do not re-add:** "Problem solving," "Team player," "Communication skills." Unverifiable, nobody screens for them, and the summary already claims the same things.

**Languages:** Hebrew (native), English (fluent).

---

## Cut and why — so you don't re-add these by accident

- **IDE proficiency line** ("Visual Studio, VS Code, Android Studio, JetBrains") — nobody screens for IDE familiarity; it's assumed the moment you list a language
- **"Gained experience in..." × 4** under Education — repeated every term already in the sidebar, in a form-filler voice
- **Git/GitHub as an Education bullet** — table stakes, already in Skills
- **Hobbies section** — "game development" is redundant with a project entry
- **Three aspiration bullets** in the old summary — see Summary section above
- **Courts Guard, Ministry of Defense (2022–2026)** — omitted. Reconsider only if a gap question comes up; it does show you worked through your degree

---

## Formatting rules for this template

- One date format everywhere: `March 2026 – Present`, `2022 – 2026`, `2019 – 2022`
- Left-align body paragraphs, don't justify (justification creates the wide word gaps)
- Bold for sub-headings, not underline (underline reads as a hyperlink)
- Sidebar links: full URLs, not "GitHub"/"LinkedIn" labels — recruiters do print CVs, and a label is a dead end on paper
- Keep both link colors identical and readable against the dark panel
- Check the **text layer** of every PDF export, not just the rendered page — ATS parsers read the text layer. A stray character in the phone field means nobody calls you
- Non-breaking hyphen (Ctrl+Shift+minus) inside hyphenated words that land near a line break
- Main column is a table cell: if a single added line jumps to page 2, check Layout → Properties → Row → uncheck "Specify height," check "Allow row to break across pages"

---

## Interview talking points

**"What are you working on?"** — Inherited a two-year-old dormant production codebase with no original authors. Reconstructing the architecture from the code itself, then extending it. Most juniors have only written greenfield code and are visibly lost the first time they're dropped into a large unfamiliar system; you can describe doing exactly that.

**"How did you learn C++?"** — Course work, then the Ulibarri GAS course for the engine-specific patterns, then applied those patterns to your own architecture decisions in The Island. Honest, and the progression is the point.

**"Tell me about a design decision you made."** — The Island's story-progression subsystem: why GameInstanceSubsystem over alternatives (survives level streaming), why data-driven `FName` room IDs over an enum (designers extend without code changes), why a generic condition gate over per-event classes.

**"Why should we hire a junior?"** — Six months of paid production work, a licensed commercial project under contract, and three years operating a real-time defense system. You've been trusted with consequential systems before.
