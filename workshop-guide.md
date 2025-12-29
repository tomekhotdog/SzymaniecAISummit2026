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
> - README.md — summary linking everything together
>
> Start with 01-brief.md and help me gather requirements by asking the right questions."

This shows Claude creating the file structure from the start — family sees the project taking shape immediately.

---

### 2. Gather the Brief (10 mins)

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

### 3. People Preferences (5 mins)

> "Create a preferences matrix showing what each person wants from the holiday. Save to 02-people.md"

Go around the room. What does Mum want? Dad? Ola? Michal? Maria?

**Output:** `02-people.md` — Preferences matrix (table format)

---

### 4. Generate Options (10 mins)

> "Based on this brief and preferences, suggest 4 destination options with reasoning. Save to 03-destinations.md"

Claude proposes options. Family reacts ("Ooh Portugal", "Not Croatia again").

You can push back live:
> "Dad's not keen on long flights. What about options under 3 hours from London?"

Shows Claude adapting to new constraints.

**Output:** `03-destinations.md` — Options list with reasoning

---

### 5. Trade-off Analysis (10 mins)

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

### 6. Recommendation & Wrap-up (5 mins)

> "Based on our discussion, write a recommendation with reasoning. Include next steps. Save to 05-recommendation.md"

Then:
> "Create a README.md that summarises the whole project and links to all the files"

**Final flourish:** Push to GitHub Pages — "And now it's a shareable website."

**Output:**
- `05-recommendation.md` — Final recommendation
- `README.md` — Summary linking everything together

---

## Key Moments to Highlight

| Moment | What it demonstrates |
|--------|---------------------|
| Claude asks clarifying questions | "It thinks about what it needs to know" |
| Structured brief appears | "It organised our chaos" |
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
├── README.md           ← Summary linking everything
├── 01-brief.md         ← Requirements gathered
├── 02-people.md        ← Preferences matrix
├── 03-destinations.md  ← Candidate locations
├── 04-comparison.md    ← Trade-off table
└── 05-recommendation.md ← Final recommendation
```
