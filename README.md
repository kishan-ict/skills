<!-- ═══════════════════════════════════════════════════════════════════════════ -->
<!--                     CURATED & MAINTAINED BY KISHAN                        -->
<!--                   https://github.com/kishan-ict                           -->
<!-- ═══════════════════════════════════════════════════════════════════════════ -->

<div align="center">

```
╔═══════════════════════════════════════════════════════════════╗
║                                                               ║
║    ███████╗██╗  ██╗██╗██╗     ██╗     ███████╗                ║
║    ██╔════╝██║ ██╔╝██║██║     ██║     ██╔════╝                ║
║    ███████╗█████╔╝ ██║██║     ██║     ███████╗                ║
║    ╚════██║██╔═██╗ ██║██║     ██║     ╚════██║                ║
║    ███████║██║  ██╗██║███████╗███████╗███████║                ║
║    ╚══════╝╚═╝  ╚═╝╚═╝╚══════╝╚══════╝╚══════╝                ║
║                                                               ║
║          for Real Engineers.  No vibe coding.                 ║
║                                                               ║
╚═══════════════════════════════════════════════════════════════╝
```

<h1>🧠 AI Agent Skills — For Real Engineering</h1>

<p align="center">
  <strong>Composable. Lightweight. Model-agnostic. Battle-tested.</strong><br/>
  <em>Claude Code skills curated & maintained in my personal .claude directory</em>
</p>

---

[![MIT License](https://img.shields.io/badge/License-MIT-00C8FF?style=for-the-badge&logo=opensourceinitiative&logoColor=white)](./LICENSE)
[![Claude Code](https://img.shields.io/badge/Claude_Code-Compatible-FF2D9B?style=for-the-badge&logo=anthropic&logoColor=white)](https://claude.ai/code)
[![Skills Count](https://img.shields.io/badge/Skills-22+-7C3AED?style=for-the-badge&logo=bookstack&logoColor=white)]()
[![Maintained by](https://img.shields.io/badge/Maintained_by-kishan--ict-0D1117?style=for-the-badge&logo=github&logoColor=white)](https://github.com/kishan-ict)

---

> **📌 Attribution:** This repository is a curated personal copy of [`mattpocock/skills`](https://github.com/mattpocock/skills), licensed under MIT.  
> Skills content is original work by **Matt Pocock**. This fork is maintained by **[@kishan-ict](https://github.com/kishan-ict)** for personal use, learning, and customization.

</div>

---

## 🤔 Why This Exists

Developing real applications is hard. Frameworks like GSD, BMAD, and Spec-Kit try to help — but they take away your control and make bugs in the process hard to resolve.

These skills are different:

```
┌─────────────────────────────────────────────────────────────┐
│                                                             │
│   ✅  Small          →  Easy to read, easy to adapt        │
│   ✅  Composable     →  Mix & match what you need          │ 
│   ✅  Model-agnostic →  Works with Claude, Codex, etc.     │
│   ✅  Battle-tested  →  Based on decades of eng experience │
│   ✅  Open           →  MIT Licensed, hack away            │
│                                                             │
└─────────────────────────────────────────────────────────────┘
```

> _"Hack around with them. Make them your own. Enjoy."_

---

## ⚡ Quick Start

### Install via npx (Recommended)

```bash
# Pick individual skills you want
npx skills@latest add mattpocock/skills/<skill-name>

# Example: install the grilling + TDD skills
npx skills@latest add mattpocock/skills/grill-me
npx skills@latest add mattpocock/skills/tdd
```

### Manual Install

```bash
# Clone this repo
git clone https://github.com/kishan-ict/<your-repo-name>.git

# Copy skills to your .claude directory
cp -r skills/* ~/.claude/skills/
```

### First-time Setup

After installing, run this in your agent:

```
/setup-matt-pocock-skills
```

It will ask you 3 things:

```
┌──────────────────────────────────────────────────────────┐
│  Section A  →  Issue Tracker (GitHub / Linear / Local)   │
│  Section B  →  Triage Label Vocabulary                   │
│  Section C  →  Domain Docs Layout (CONTEXT.md / ADRs)    │
└──────────────────────────────────────────────────────────┘
```

---

## 🗺️ Skill Map

```
skills/
│
├── 🔧 engineering/
│   ├── /setup-matt-pocock-skills   ← Run this first!
│   ├── /grill-me                   ← Alignment interviews
│   ├── /to-prd                     ← Context → PRD
│   ├── /to-issues                  ← PRD → GitHub Issues
│   ├── /triage                     ← Issue state machine
│   ├── /tdd                        ← Red → Green → Refactor
│   ├── /diagnose                   ← Debug loop
│   ├── /improve-codebase-arch      ← Fight the ball of mud
│   ├── /zoom-out                   ← Get high-level context
│   ├── /ubiquitous-language        ← DDD glossary extractor
│   └── /git-guardrails             ← Safe git workflows
│
├── 📝 productivity/
│   ├── /write-a-skill              ← Build your own skills
│   ├── /edit-article               ← Polish writing
│   ├── /caveman                    ← 75% token reduction mode
│   └── /obsidian-vault             ← Notes management
│
└── 🛠️ general/
    └── [additional community skills]
```

---

## 📚 Skills Breakdown

### 🔴 Most Important — Start Here

---

#### `/grill-me` — Alignment Before You Build

```
┌─────────────────────────────────────────────────────────────┐
│  THE PROBLEM                                                │
│                                                             │
│  You think the agent knows what you want.                   │
│  You see what it built.                                     │
│  It didn't understand you at all.                           │
│                                                             │
│  THE FIX                                                    │
│                                                             │
│  /grill-me  →  Agent interviews you HARD                    │
│             →  Forces alignment BEFORE coding               │
│             →  Saves hours of rebuilding                    │
└─────────────────────────────────────────────────────────────┘
```

**When to use:** Every single time you start a new feature or change.

```bash
# In Claude Code
/grill-me
```

---

#### `/tdd` — Test-Driven Development Loop

```
RED  →  Write a failing test
 ↓
GREEN  →  Make it pass (minimal code)
 ↓
REFACTOR  →  Clean it up
 ↓
REPEAT  ↺
```

Builds features one **vertical slice** at a time. The agent knows exactly what makes a good test vs. a bad one.

---

#### `/diagnose` — Debug Loop

```
OBSERVE  →  What is the actual vs. expected behavior?
 ↓
HYPOTHESIZE  →  What could cause this?
 ↓
TEST  →  Verify hypothesis
 ↓
FIX  →  Apply the correct fix
 ↓
CONFIRM  ✅
```

---

### 🟡 Planning & Architecture

---

#### `/to-prd` — Conversation → PRD

No interview. No form-filling. Just synthesizes what you've already discussed into a full Product Requirements Document, then pushes it to your issue tracker.

```markdown
PRD Structure:
├── 🎯 Problem Statement
├── 💡 Proposed Solution
├── 📖 User Stories (long, exhaustive list)
├── 🏗️  Implementation Decisions
├── 🧪 Testing Decisions
└── 📌 Additional Notes
```

---

#### `/to-issues` — PRD → GitHub Issues

Breaks any plan, spec, or PRD into **independently-grabbable GitHub issues** using vertical slices.

```
PRD  ──→  Issue #1: [Feature A - Backend]
      ──→  Issue #2: [Feature A - Frontend]  
      ──→  Issue #3: [Feature B]
      ──→  Issue #4: [Tests]
```

Each issue can be picked up independently by a human or an AFK agent.

---

#### `/improve-codebase-architecture` — Rescue the Ball of Mud

> _"The best modules are deep. They allow a lot of functionality to be accessed through a simple interface."_

```
BEFORE  →  Complex, tangled, hard to change
AFTER   →  Deep modules, clean interfaces, testable in isolation
```

Run this **once every few days** on your codebase. Agents accelerate software entropy — this fights back.

---

#### `/ubiquitous-language` — Domain-Driven Design Glossary

```
Domain experts  →  speak one language
Developers      →  speak another language
               ↕
         MISALIGNMENT 😬

/ubiquitous-language  →  Extract shared vocabulary
                      →  Encode in CONTEXT.md
                      →  Agent speaks your domain
```

---

### 🟢 Utility Skills

---

#### `/caveman` — 75% Token Reduction Mode

```
NORMAL: "Could you please help me understand the implications 
        of refactoring the authentication module to use JWT?"

CAVEMAN: "jwt refactor auth module - good or bad?"
```

Same technical accuracy. 75% fewer tokens. Great for long sessions.

---

#### `/zoom-out` — High-Level Context

When the agent is too deep in the weeds, `/zoom-out` forces it to step back and give you the bigger picture of an unfamiliar code section.

---

#### `/write-a-skill` — Build Your Own Skills

Meta-skill. Use this to create new skills with proper structure, progressive disclosure, and bundled resources.

```markdown
Good skill description:
"Extract text and tables from PDF files, fill forms, merge documents. 
Use when working with PDF files or when user mentions PDFs."

Bad skill description:
"Helps with documents."
```

The description is **the only thing your agent sees** when deciding to load a skill. Make it count.

---

#### `/obsidian-vault` — Notes Management

Search, create, and manage notes in your Obsidian vault with wikilinks and index notes. Great for knowledge workers and researchers.

---

## 🔄 Recommended Workflow

```
NEW FEATURE REQUEST
      │
      ▼
 /grill-me ←── Align with the agent first
      │
      ▼
 /to-prd  ←── Turn context into a PRD
      │
      ▼
 /to-issues ←── Break PRD into issues
      │
      ▼
 /tdd ←── Build feature (red/green/refactor)
      │
      ▼
 /triage ←── Process new issues
      │
      ▼
 /improve-codebase-architecture ←── Run every few days
```

---

## 🧠 Philosophy

```
┌─────────────────────────────────────────────────────────────────┐
│                                                                 │
│   "These skills are designed to be small, easy to adapt,        │
│    and composable. They work with any model. They're based      │
│    on decades of engineering experience."                       │
│                                                                 │
│                                        — Matt Pocock            │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

The most common failure mode in AI-assisted development is **misalignment** — the communication gap between you and the agent. These skills are designed to close that gap, not widen it.

---

## 🛠️ Compatibility

| Tool | Status |
|------|--------|
| ✅ Claude Code | Fully supported |
| ✅ GitHub Copilot / Codex | Compatible |
| ✅ Any agent with AGENTS.md support | Compatible |
| ✅ Local markdown issue tracking | Supported |
| ✅ GitHub Issues | Supported |
| ✅ Linear | Supported |

---

## 📁 File Structure

```
.
├── skills/
│   ├── engineering/
│   │   ├── grill-me/SKILL.md
│   │   ├── tdd/SKILL.md
│   │   ├── to-prd/SKILL.md
│   │   ├── to-issues/SKILL.md
│   │   ├── triage/SKILL.md
│   │   ├── diagnose/SKILL.md
│   │   ├── improve-codebase-architecture/SKILL.md
│   │   ├── zoom-out/SKILL.md
│   │   ├── ubiquitous-language/SKILL.md
│   │   └── setup-matt-pocock-skills/SKILL.md
│   ├── productivity/
│   │   ├── write-a-skill/SKILL.md
│   │   ├── edit-article/SKILL.md
│   │   ├── caveman/SKILL.md
│   │   └── obsidian-vault/SKILL.md
│   └── git-guardrails/SKILL.md
├── README.md  ← You are here
└── LICENSE
```

---

## 📜 License & Credits

```
MIT License — Free to use, modify, and distribute.
```

**Original Author:** [Matt Pocock](https://github.com/mattpocock) — creator of `mattpocock/skills`  
All skill content, philosophies, and system design are his original work.

**Curated & Maintained by:** [Kishan](https://github.com/kishan-ict)  
This fork is maintained as a personal collection, customized for my own AI-assisted engineering workflow.  
No skill content has been modified from the upstream source.

---

<div align="center">

```
╔══════════════════════════════════════════════════════╗
║                                                      ║
║   Built different. Engineered with intent.          ║
║                                                      ║
║   — @kishan-ict  ×  mattpocock/skills               ║
║                                                      ║
╚══════════════════════════════════════════════════════╝
```

[![GitHub](https://img.shields.io/badge/GitHub-kishan--ict-0D1117?style=for-the-badge&logo=github&logoColor=white)](https://github.com/kishan-ict)
[![Upstream](https://img.shields.io/badge/Upstream-mattpocock%2Fskills-FF2D9B?style=for-the-badge&logo=github&logoColor=white)](https://github.com/mattpocock/skills)

_Star ⭐ the upstream repo to support Matt Pocock's work!_

</div>
