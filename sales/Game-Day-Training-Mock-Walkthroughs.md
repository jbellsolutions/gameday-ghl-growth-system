# Game Day Training Mock Walkthroughs

## Purpose
Use these scenarios in coaching calls to show exactly how each role uses Claude Code in real workflows.

## Scenario 1: Front Desk - Reactivation Reply

### Situation
A lapsed patient responds to an SMS reactivation message with: "I'm interested, but not sure TRT is right for me now."

### Prompt
```text
You are a Game Day front desk assistant. Draft a short, empathetic reply that:
1) acknowledges concern,
2) offers a low-friction consult,
3) includes booking link CTA,
4) avoids medical claims.
```

### Expected Output
- 2-4 sentence response
- Reassuring tone, clear CTA
- No diagnosis language

### Rules
- Never give medical advice
- Never discuss protected health info in shared channels

## Scenario 2: Clinic Ops - Weekly KPI Triage

### Situation
Location A has strong lead volume but low booked consults this week.

### Prompt
```text
Compare last 7 days for Location A and B. Identify top 3 conversion leaks and propose one fix per leak for next week.
```

### Expected Output
- Ranked leak list
- Fixes tied to workflow stage
- Owner-ready action list

### Rules
- Use only reported KPI data
- Separate facts from assumptions

## Scenario 3: Owner - Decision Memo

### Situation
Tony needs a one-page decision memo: hire another integrator or improve current workflow first.

### Prompt
```text
Write a one-page decision memo with: current KPI baseline, expected impact of hiring vs optimization, recommendation, and 30-day test plan.
```

### Expected Output
- Executive memo format
- Recommendation with rationale
- Clear 30-day checkpoint metrics

### Rules
- Include downside risks
- Do not guarantee outcomes

## Scenario 4: AI Integrator - Daily Operating Loop

### Situation
Monday morning operating check across all active campaigns.

### Prompt
```text
Generate today's operating checklist for AI Integrator:
- speed-to-lead health,
- reactivation queue,
- no-show rescue,
- review requests,
- blocked tasks.
Then draft escalation notes for anything below target.
```

### Expected Output
- Actionable checklist
- Escalation section
- End-of-day reporting template

### Rules
- Timebox actions
- Log every change made in workflows

## Scenario 5: Marketing - Expert Series Distribution

### Situation
New Expert Series source video is ready.

### Prompt
```text
Turn one source video into a 2-week distribution plan: 4 LinkedIn posts, 1 newsletter, 3 short-form video scripts, and 2 nurture emails. Keep tone authoritative and simple.
```

### Expected Output
- Calendarized content plan
- Asset list per channel
- Reuse path for GHL nurture

### Rules
- Maintain voice consistency
- Avoid repetitive hooks and generic claims

## Coaching Call Rubric
- Accuracy: output follows role constraints.
- Safety: no compliance violations.
- Clarity: instructions and outputs are easy to execute.
- KPI linkage: every activity maps to a measurable outcome.
