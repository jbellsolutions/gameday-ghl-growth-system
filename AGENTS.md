# AGENTS — Game Day GHL Growth System

## Agent Roles

### Research Agent
- **Purpose**: Market research, competitive intelligence, franchise analysis
- **Inputs**: Web search, GitHub repos, public franchise data
- **Outputs**: Research documents in /research/
- **Constraints**: Cite all sources, use conservative estimates, flag when data is stale

### Content Agent
- **Purpose**: Generate content via Titan Genome + Genius Tap pipeline
- **Inputs**: Client video transcripts, voice profiles, story banks
- **Outputs**: Content pieces in /content-system/
- **Constraints**: Must pass 3-agent quality gauntlet (Creator > Critic > Approver, score 75+), no fabricated stories or credentials

### Sales Agent
- **Purpose**: Generate sales materials, proposals, one-pagers
- **Inputs**: Research docs, revenue projections, product specs
- **Outputs**: Sales materials in /sales/
- **Constraints**: Revenue projections must show assumptions and ranges, never guarantee outcomes

### GHL Agent
- **Purpose**: Design and document GHL workflows
- **Inputs**: Best practices research, HIPAA requirements, franchise operational data
- **Outputs**: Workflow documentation in /ghl-system/, message templates
- **Constraints**: HIPAA compliance required, no patient data, all templates must be generic/customizable

## Handoff Protocol

1. **Research Agent** produces market research and competitive intel
2. **Sales Agent** consumes research to generate strategy and proposals
3. **Content Agent** uses research + client input to generate Expert Series content
4. **GHL Agent** uses research to design automation workflows
5. All agents reference CLAUDE.md for project context and ETHOS.md for constraints

## Session Protocol

At the start of each session:
1. Read CLAUDE.md for project identity and context
2. Read ETHOS.md for constraints and quality bar
3. Check TODOS.md for current priorities
4. Check CHANGELOG.md for recent changes
