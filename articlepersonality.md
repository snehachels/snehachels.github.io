# Article Personality Guide — Sneha Chelimilla Portfolio

> Reference this document every time a new article is written or an existing one is updated.
> Target audience: hiring managers and recruiters for PM, Senior PM, AI PM, and Product Operations Manager roles.

---

## Who Reads These Articles

**Primary readers:**
- Hiring managers at AI/tech companies, management consulting firms, high-growth startups
- Recruiters screening for Product Manager, Senior PM, and Product Operations roles

**What they're looking for in 90 seconds:**
1. Did this PM own real business outcomes, or just ship features?
2. Do they understand users, data, AND business strategy?
3. Can they write clearly and think rigorously?
4. Are they honest about trade-offs and failures (signals seniority)?

---

## Mandatory 5-Part Storytelling Framework

Every past project article must follow this structure with explicit labeled sections.
Every blog/career article should follow it loosely.

### 1. Problem Statement
- Open with the **business context**, not the product
- State who was affected and quantify the cost of the problem
- Good: "Invoice reconciliation took 4–5 days. At Vorto's volume, that was 200+ analyst-hours per month sitting in categorization, not analysis."
- Bad: "The finance team had manual processes."
- **PM signals:** strategic thinking, user empathy, business acumen

### 2. Research & Discovery
- **Name** the methodology: interviews, data analysis, competitive research, shadowing, A/B testing, surveys
- **Quantify** the research: "50+ user interviews across 6 departments over 3 months"
- **State what changed** because of the research — what assumption was wrong, what direction shifted
- Include the method-grid component to make discovery work tangible
- **PM signals:** discovery methodology, data-driven decisions, user research skills

### 3. Solution & Process
- Reference **PM artifacts**: PRD, roadmap decision, sprint structure, acceptance criteria
- Explain **what was cut** from scope and why (shows prioritization judgment)
- Name **who was in the room**: engineering, design, finance, operations — and what disagreements got resolved
- Include process-flow component for multi-phase work
- Include artifact-card components for deliverables
- **PM signals:** execution, cross-functional leadership, product craft, PLM governance

### 4. Impact & Metrics
- Always include a **Before/After comparison** using the ba-grid component
- Use the stat-strip for headline numbers at the top of the article
- Quantify across 3 dimensions:
  - **User outcomes**: adoption rate, NPS, WAU, satisfaction
  - **Business outcomes**: revenue, cost savings, efficiency
  - **Operational outcomes**: time saved, error rate, velocity
- Use "within X months/weeks" to show speed of impact
- **PM signals:** data-driven mindset, business impact ownership, KPI tracking

### 5. Reflection
- Name a **specific decision that was wrong** or suboptimal
- Name a **specific trade-off** made: what was sacrificed for what
- Say what you would do differently and why
- This section separates senior PMs from junior ones — be honest
- **PM signals:** growth mindset, intellectual honesty, seniority

---

## PM Skills Checklist (include at least 4 per past project)

- [ ] Product discovery methodology named and quantified
- [ ] User research evidence (interviews, data, testing)
- [ ] Roadmap decision explained with trade-offs
- [ ] PRD or spec artifact referenced
- [ ] Cross-functional stakeholder coordination described (who, how many)
- [ ] Prioritization framework or rationale stated
- [ ] A/B test or validation method mentioned
- [ ] Metric ownership demonstrated (KPI defined, tracked, owned)
- [ ] Launch or rollout process described
- [ ] Post-launch iteration cycle shown

## Product Operations Skills Checklist

- [ ] PLM (Product Lifecycle Management) framework built or operated
- [ ] Standardized process or governance established
- [ ] Feedback loop design described (how learnings flowed back into product)
- [ ] Data quality or model health management mentioned
- [ ] Cross-team operating cadence established
- [ ] Tooling or platform decision made (build/buy, migration)
- [ ] Onboarding or adoption program designed
- [ ] Capacity/throughput improvement quantified

---

## Visual Components (HTML/CSS)

Use these components consistently. CSS is defined in each article's `<style>` block.

### `stat-strip` — Headline metrics (mandatory for past projects)
4-column grid of big numbers at the top. Use for the most impressive 4 outcomes.
```html
<div class="stat-strip">
  <div class="stat-item"><div class="num">X%</div><div class="label">outcome label</div></div>
</div>
```

### `ba-grid` — Before/After comparison (mandatory for past projects)
Side-by-side two-column grid. Red left column (before), green right column (after).
Each item should be concrete and specific — a state, not a vague concept.
```html
<div class="ba-grid">
  <div class="ba-col ba-before">
    <div class="ba-label">Before</div>
    <ul><li>Specific state</li></ul>
  </div>
  <div class="ba-col ba-after">
    <div class="ba-label">After</div>
    <ul><li>Specific improved state</li></ul>
  </div>
</div>
```

### `method-grid` — Research methodology (recommended for discovery sections)
3-column grid showing methods, counts, and scope. Makes PM discovery work tangible.
```html
<div class="method-grid">
  <div class="method-card">
    <div class="m-num">50+</div>
    <div class="m-label">User Interviews</div>
    <div class="m-detail">Ops, Finance, Engineering, IT</div>
  </div>
</div>
```

### `process-flow` — Multi-phase execution (recommended)
Vertical timeline with numbered phases. Use for articles with distinct execution stages.
```html
<div class="process-flow">
  <div class="pf-step">
    <div class="pf-meta">Phase 1 · Month 1–3</div>
    <h4>Discovery</h4>
    <p>What happened and what you found.</p>
  </div>
</div>
```

### `artifact-row` + `artifact-card` — PM deliverables (recommended)
Shows concrete PM work product. Makes the role tangible to non-PMs.
```html
<div class="artifact-row">
  <div class="artifact-card">
    <div class="artifact-icon">📋</div>
    <div class="artifact-info">
      <div class="artifact-type">PRD</div>
      <div class="artifact-name">Feature Name</div>
      <div class="artifact-detail">X pages · Y stakeholder sign-offs</div>
    </div>
  </div>
</div>
```

### `phase-label` — Section phase indicator (optional)
Small colored badge before a section heading to orient the reader.
```html
<div class="phase-label">Phase 1: Discovery</div>
```

---

## SEO & Recruiter-Friendly Patterns

### Meta Description Template
```
[Role context] — [specific achievement with number]. A PM case study covering [skill 1], [skill 2], and [skill 3] at [company/context].
```

### Page Title Format
```
[Specific Project Name] | PM Case Study | Sneha Chelimilla
```

### H2 Header Patterns That Recruiters Scan
Structure H2s to answer "what did this PM do?" not just "what happened?"
- ✅ "How I Defined the Product Vision Through 50+ Stakeholder Interviews"
- ✅ "The Prioritization Decision That Changed the Product Direction"
- ❌ "Research Phase"
- ❌ "What Happened Next"

### Required Keywords (weave naturally — never stuff)

**Product Management:**
product roadmap, feature prioritization, PRD, user research, A/B testing, product discovery, product strategy, go-to-market, sprint planning, cross-functional leadership, stakeholder management, OKRs, KPIs, product lifecycle management

**AI/Data Products:**
AI product management, ML product development, LLM workflows, data strategy, analytics platform, model accuracy, AI automation, data observability, process automation, AI-driven, machine learning

**Product Operations:**
product operations, PLM governance, operational excellence, process standardization, launch readiness, feedback loops, capacity planning, product-led growth

**Industry Context:**
supply chain, enterprise software, SaaS, B2B, automotive, Fortune 500, startup, scale-up, management consulting

---

## Tone & Voice

**Direct and specific.** No vague language.
- ❌ "we improved efficiency"
- ✅ "we reduced invoice processing time from 4–5 days to same-day"

**First-person and owned.** "I" for decisions you made; "we" for team execution.
- ❌ "the team decided to prioritize"
- ✅ "I prioritized X over Y because Z"

**Intellectually honest.** Acknowledge what didn't work. Recruiters can spot sanitized portfolios.

**Business-fluent.** Frame outcomes in terms of business value, not technical achievement.
- ❌ "we deployed a classification model with 90% F1 score"
- ✅ "AI classification at 90% accuracy cut processing time 5x and freed the finance team for analysis"

**Engineer-grounded.** Use technical vocabulary naturally but always translate to impact.

---

## Paragraph Length
- Opening paragraph: 2–3 sentences (hook for scanning)
- Body paragraphs: 3–5 sentences, one idea per paragraph
- Callout boxes: 1–3 sentences, key insight only

---

## Article Length Targets
| Type | Words | Read Time |
|---|---|---|
| Past Project deep-dive | 1,800–2,500 | 8–10 min |
| Side Project | 1,200–1,800 | 6–8 min |
| Blog / Career | 900–1,400 | 4–6 min |

---

## Quality Gate (before publishing)

### Content
- [ ] All 5 framework sections present
- [ ] At least 4 PM skills from checklist evidenced
- [ ] Reflection includes a specific mistake or trade-off (not just "I learned a lot")
- [ ] At least one number that shows business impact

### Visuals
- [ ] stat-strip with 4 headline metrics (past projects)
- [ ] ba-grid Before/After visual (past projects)
- [ ] method-grid or process-flow for discovery/execution

### SEO & Meta
- [ ] Meta description follows template with role keywords
- [ ] Page title follows format
- [ ] H2s are specific and action-oriented

### Navigation
- [ ] Back link points to correct section (past-projects, side-projects, blog)
- [ ] Footer back link matches top bar back link

---

## Article Type Reference

### Past Project articles (`blog/`)
Full case study format. All 5 sections mandatory. Full visual suite.
Current examples: mercedes-ai-division.html, vorto-ai-field-notes.html

### Side Project articles (`blog/`)
More personal, less formal. Framework loosely followed. Focus on what you built, why, and what you learned.
Current examples: llm-prd-builder.html

### Blog / Career articles (`blog/`)
Narrative-driven. Framework optional. Focus on insight and voice.
Current examples: engineer-to-pm.html
