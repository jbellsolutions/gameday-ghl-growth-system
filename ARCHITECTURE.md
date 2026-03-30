# ARCHITECTURE — Game Day GHL Growth System

## Overview

This is a documentation and strategy repo, not a codebase. It contains the complete playbook for deploying three products to Game Day Men's Health franchises.

## Directory Layout

```
gameday-ghl-growth-system/
│
├── README.md                              # Public-facing overview
├── CLAUDE.md                              # AI agent context
├── ETHOS.md                               # Project values and constraints
├── ARCHITECTURE.md                        # This file
├── CHANGELOG.md                           # Version history
├── VERSION                                # Current version
├── WALKTHROUGH.md                         # Setup guide
├── llms.txt                               # LLM-readable project summary
│
├── GameDay-Internal-GamePlan-and-Launch.md # Master game plan (Phases 1-4)
│
├── ghl-system/                            # GHL Workflows (Product 1)
│   ├── snapshots/                         # Importable GHL workflow configs
│   └── templates/                         # SMS, email, voicemail copy
│
├── content-system/                        # Expert Series v3 (Product 3)
│   ├── expert-series-outputs/             # Content Multiplier samples
│   └── genius-tap-outputs/                # Ongoing monthly content samples
│
├── ai-integrator/                         # AI Integrator Program (Product 2)
│   └── (playbook, KPIs, training, daily checklist)
│
├── research/                              # Market research & competitive intel
│   ├── GameDay-Research-and-Game-Plan.md   # Comprehensive franchise research
│   ├── GameDay-Non-CRM-Business-Opportunities.md  # Expansion opportunities
│   ├── One-Pager-GameDay-Research.md      # Game Day research summary
│   └── One-Pager-DrVinocur-Research.md    # Dr. Vinocur profile
│
├── sales/                                 # Sales materials
│   ├── One-Pager-Strategy-Recommendation.md  # Do/don't decision doc
│   ├── One-Pager-GameDay-Strategy.md      # Game Day strategy
│   └── One-Pager-DrVinocur-Strategy.md    # Dr. Vinocur strategy
│
├── docs/                                  # Supporting documentation
│
└── .claude/                               # AI agent infrastructure
    ├── agi-1/                             # AGI-1 scores and iterations
    ├── healing/                           # Error patterns
    ├── learning/                          # Observations
    └── settings.json                      # Hook config
```

## Data Flow

```
┌─────────────────────────────────────────────────────────┐
│                    THE GAME DAY GAME PLAN                │
│                                                         │
│  ┌──────────┐  ┌───────────────┐  ┌──────────────────┐  │
│  │   GHL    │  │ AI Integrator │  │  Expert Series   │  │
│  │ Workflows│  │   Program     │  │      v3          │  │
│  └────┬─────┘  └──────┬────────┘  └────────┬─────────┘  │
│       │               │                    │             │
│       v               v                    v             │
│  Speed-to-Lead   Trained Person      Video Input         │
│  Reactivation    Runs GHL Daily      ──────────>         │
│  No-Show Recov.  KPIs + Coaching     32+ Assets          │
│  Reviews/Refs    $1K + $300/mo       (Content Multiplier)│
│  Newsletters                         52+/mo Ongoing      │
│       │               │             (Genius Tap)         │
│       └───────┬───────┘                    │             │
│               v                            v             │
│     GHL Campaigns <──── Content Feeds Into ──┘           │
│               │                                          │
│               v                                          │
│     Revenue Impact: $741K - $1.05M per location          │
└─────────────────────────────────────────────────────────┘

┌─────────────────────────────────────────┐
│     DR. VINOCUR (Standalone)            │
│                                         │
│  Expert Series v3 Only                  │
│  ──────────>                            │
│  Personal Brand Content Engine          │
│  100+ pieces/month                      │
│  3 Brand Pillars Unified                │
└─────────────────────────────────────────┘
```

## Integration Points

| System | Role | Connection |
|--------|------|------------|
| Go High Level | CRM + automation | Receives workflows, runs campaigns |
| Titan Genome Content Multiplier | Content engine | Produces 32+ assets from video input |
| Genius Tap Content System | Ongoing content | Produces 52+/month from extraction calls |
| GitHub | Version control | This repo + related repos |
| Speaker Agent Ops Dashboard | Monitoring | Repo health tracked in constants.ts |

## Related Repos

- `jbellsolutions/Titan-Genome-Content-Multiplier` — Powers the Expert Series
- `jbellsolutions/genius-tap-content-system` — Powers ongoing monthly content
- `jbellsolutions/speakeragent-ops` — Operations dashboard
