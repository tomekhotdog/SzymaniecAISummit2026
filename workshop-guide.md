# Workshop Facilitator's Guide
## "Plan the Next Szymaniec Family Holiday"

**Duration:** 45 minutes (11:00 – 11:45)
**Format:** Live collaborative session with Claude Code
**Output:** A structured holiday planning document across multiple files

---

## Before You Start

- Have Claude Code open and ready
- Create a fresh `holiday-planning/` directory
- Have GitHub Pages ready to show the final result
- Reference the template structure in this repo's `holiday-planning/` folder

---

## Flow

### 1. Set the Stage (5 mins)

Quick intro:
> "I'm going to show you how I've been using Claude. We're going to plan a holiday together — shout out ideas, I'll type, and watch how it structures our thinking."

Open Claude Code, start a fresh session in the `holiday-planning/` folder.

**Kick off by prompting Claude to set up the project structure:**

> "We're going to plan a family holiday together. Set up a project structure with separate markdown files for:
> - 01-brief.md — requirements and constraints
> - 02-people.md — preferences matrix for each person
> - 03-destinations.md — candidate locations
> - 04-comparison.md — trade-off analysis table
> - 05-recommendation.md — final recommendation and next steps
> - index.md — summary linking everything together
>
> Start with 01-brief.md and help me gather requirements by asking the right questions."

This shows Claude creating the file structure from the start — family sees the project taking shape immediately.

---

### 2. Gather the Brief (5 mins)

Prompt Claude with something like:
> "We're planning a family holiday. Help me gather requirements by asking the right questions. Save the brief to 01-brief.md"

Claude will likely ask about:
- When? (dates, duration)
- Who's going? (6 adults — any mobility/accessibility needs?)
- Budget? (per person, total)
- Vibe? (relaxing vs adventure vs culture)
- Hard constraints? (flights from UK, visa requirements)

**Family participates here** — everyone shouts out answers. You type them in. Claude organises.

**Output:** `01-brief.md` — A structured "Holiday Brief"

---

### 3. People Preferences via WhatsApp (10 mins)

**This section demonstrates Claude generating questions, then synthesizing async responses.**

**Step 1: Generate the questionnaire**

> "Generate a very concise questionnaire (5-6 questions max) to gather each person's holiday preferences. Keep it short enough to answer quickly on WhatsApp. Include questions about: must-haves, deal-breakers, activity preferences, accommodation style."

Claude generates something like:
```
1. What's your ONE must-have for this holiday?
2. What's a deal-breaker (something you'd hate)?
3. Beach, city, countryside, or mix?
4. Active adventure or relaxing downtime?
5. Any dietary or accessibility needs?
```

**Step 2: Send to family WhatsApp group**

Copy the questions, send to the group. Everyone replies (give them 3-4 mins).

**Step 3: Paste all responses into Claude**

> "Here are everyone's responses. Summarise the common themes, note any conflicts, and create a preferences matrix. Save to 02-people.md"

Paste the WhatsApp replies. Claude synthesizes the chaos into structure.

**What this demonstrates:**
- Claude generating fit-for-purpose questions
- Handling messy, real-world input (WhatsApp messages)
- Synthesizing multiple perspectives into a coherent summary

**Output:** `02-people.md` — Preferences matrix (table format)

---

### 4. Create Specialist Agents (5 mins)

**This section demonstrates creating purpose-built agents with specific expertise.**

> "Help me create two agents for this project:
> 1. A 'Research Agent' that can look up destinations, flights, costs, weather, etc.
> 2. A 'Family Expert Agent' that has access to all our gathered preferences and can answer questions about what the family wants.
>
> Generate the system prompts I should use when creating these agents."

Claude will generate prompts like:

**Research Agent prompt:**
```
You are a travel research assistant. Your job is to find specific,
factual information about destinations, flights, accommodation,
costs, weather, and activities. Always cite sources when possible.
Focus on practical details relevant to a family of 6 adults
travelling from the UK.
```

**Family Expert Agent prompt:**
```
You are an expert on the Szymaniec family's holiday preferences.
You have access to the following information:
[Paste contents of 01-brief.md and 02-people.md]

Answer questions about what the family wants, identify potential
conflicts, and suggest compromises. Always reference specific
family members' stated preferences.
```

**What this demonstrates:**
- Creating specialized agents for different tasks
- Giving agents specific context and roles
- The concept of "memory" via injected context

---

### 5. Generate Options (10 mins)

> "Based on this brief and preferences, suggest 4 destination options with reasoning. Save to 03-destinations.md"

**Optional: Use the Research Agent here** to look up real details for each destination.

Claude proposes options. Family reacts ("Ooh Portugal", "Not Croatia again").

You can push back live:
> "Dad's not keen on long flights. What about options under 3 hours from London?"

Shows Claude adapting to new constraints.

**Output:** `03-destinations.md` — Options list with reasoning

---

### 6. Trade-off Analysis (5 mins)

> "Create a comparison table: destinations as rows, key criteria as columns. Rate each. Save to 04-comparison.md"

Criteria might include:
- Cost
- Flight time
- Weather in [month]
- Food scene
- Things to do
- Accessibility

Family debates the ratings. You update in real-time.

**Output:** `04-comparison.md` — Comparison table

---

### 7. Recommendation & Wrap-up (5 mins)

> "Based on our discussion, write a recommendation with reasoning. Include next steps. Save to 05-recommendation.md"

Then:
> "Create an index.md that summarises the whole project and links to all the files"

**Final flourish:** Push to GitHub Pages — "And now it's a shareable website."

**Output:**
- `05-recommendation.md` — Final recommendation
- `index.md` — Summary linking everything together

---

## Key Moments to Highlight

| Moment | What it demonstrates |
|--------|---------------------|
| Claude asks clarifying questions | "It thinks about what it needs to know" |
| Questionnaire generated | "It creates tools for gathering info" |
| WhatsApp chaos → structured table | "It handles messy real-world input" |
| Agent prompts generated | "You can create specialists for different tasks" |
| Files being created | "It's building a project, not just chatting" |
| You push back and it adapts | "It's a conversation, not a one-shot" |
| Comparison table | "Michal, this is your spreadsheet brain but faster" |
| README links everything | "Structure emerges from conversation" |
| Final doc on GitHub | "And now it exists in the real world" |

---

## Talking Points for Different Audiences

**For Michal (Accountant):**
> "Notice how it structures the comparison? You could do this for any client decision — investment options, tax strategies, business structures."

**For Ola (Solicitor):**
> "Think about client intake. You could gather all the facts, have it structured, identify what's missing — before you even start drafting."

**For Maria (Strategy Consultant):**
> "This is basically a strategy engagement compressed into 45 minutes. Stakeholder input, options analysis, recommendation."

**For Dad (Physicist):**
> "It's hypothesis-driven. We stated constraints, generated options, tested against criteria, reached a conclusion."

**For Mum:**
> "You just tell it what you want and it organises everything. No clicking through menus."

---

## If Things Go Wrong

- **Claude goes off-track:** Just say "No, let's go back to X" — show that you can redirect
- **Family gets distracted:** That's fine! The messiness makes the "organised output" more impressive
- **Technical issues:** Have the example files ready as backup (in this repo)

---

## Files Created During Workshop

```
holiday-planning/
├── index.md            ← Summary linking everything (for GitHub Pages)
├── 01-brief.md         ← Requirements gathered
├── 02-people.md        ← Preferences matrix
├── 03-destinations.md  ← Candidate locations
├── 04-comparison.md    ← Trade-off table
└── 05-recommendation.md ← Final recommendation
```
