> **To install:** Open Claude Code in this folder and type `set this up for me` or `/walkthrough`

# Game Day GHL Growth System — Setup Walkthrough

## What This Repo Is

The complete playbook for deploying three products to Game Day Men's Health franchises: GHL Workflows, AI Integrator Program, and Expert Series v3 content engine. Built by Speaker Engine AI for Tony D'Agostino.

## Prerequisites

- GitHub CLI (`gh`) authenticated with access to `jbellsolutions` org
- Go High Level account (for workflow deployment)
- Claude Code (for content generation via Titan Genome + Genius Tap)
- Access to the related repos:
  - `jbellsolutions/Titan-Genome-Content-Multiplier`
  - `jbellsolutions/genius-tap-content-system`

## Getting Started

### 1. Clone the repo
```bash
git clone https://github.com/jbellsolutions/gameday-ghl-growth-system.git
cd gameday-ghl-growth-system
```

### 2. Read the game plan
Start with `GameDay-Internal-GamePlan-and-Launch.md` — this is the master doc that walks through all 4 phases: internal build, launch to Game Day, GitHub publish, and Dr. Vinocur engagement.

### 3. Explore the research
The `/research/` directory has the full market research:
- `GameDay-Research-and-Game-Plan.md` — Comprehensive franchise + GHL analysis
- `GameDay-Non-CRM-Business-Opportunities.md` — Additional revenue opportunities
- `One-Pager-GameDay-Research.md` — Quick reference summary
- `One-Pager-DrVinocur-Research.md` — Dr. Vinocur complete profile

### 4. Review the sales materials
The `/sales/` directory has pitch-ready one-pagers:
- `One-Pager-Strategy-Recommendation.md` — Do/don't decision doc with revenue projections
- Strategy docs for both Game Day and Dr. Vinocur

### 5. Start building
Follow Phase 1 in the game plan:
- Week 1: Build GHL workflows in test account
- Week 2: Run Expert Series on Game Day source material

## Key Commands

| Command | What It Does |
|---------|-------------|
| `cat GameDay-Internal-GamePlan-and-Launch.md` | Read the master game plan |
| `ls research/` | See all research docs |
| `ls sales/` | See all sales materials |
| `cat TODOS.md` | See current task list |
| `cat CHANGELOG.md` | See version history |

## Environment Variables

No environment variables needed for this repo. GHL credentials and API keys are managed in the GHL platform directly, not stored here (HIPAA compliance).

## Related Resources

- [Speaker Agent Ops Dashboard](https://github.com/jbellsolutions/speakeragent-ops)
- [Titan Genome Content Multiplier](https://github.com/jbellsolutions/Titan-Genome-Content-Multiplier)
- [Genius Tap Content System](https://github.com/jbellsolutions/genius-tap-content-system)
