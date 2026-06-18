# Brain Dump Action Planner

## Overview

Brain Dump Action Planner transforms unstructured notes, meeting transcripts, brainstorming sessions, voice memos, and stream-of-consciousness thoughts into a structured project dashboard.

The skill organizes information without making assumptions, filling gaps, or generating missing details. All names, dates, numbers, ownership assignments, terminology, and decisions are preserved exactly as provided.

The output is a modern, responsive HTML dashboard designed for project management, meeting reviews, knowledge organization, and action tracking.

---

## Core Principles

### Preserve Source Accuracy

* Never invent information.
* Never infer ownership.
* Never estimate deadlines.
* Never resolve conflicts automatically.
* Never predict outcomes.
* Preserve wording exactly when possible.

### Missing Information

Whenever information is unavailable, display:

Not specified

---

## Supported Input Types

### Brain Dumps

* Personal notes
* Idea collections
* Planning sessions
* Thought organization

### Meeting Notes

* Team meetings
* Client meetings
* Project reviews
* Workshops

### Transcripts

* Interview transcripts
* Meeting transcripts
* Voice memo transcripts
* Call recordings

### Merge Mode

* Multiple note files
* Multiple meeting summaries
* Combined transcripts
* Cross-source planning documents

---

## Output Format

The skill generates a complete self-contained HTML artifact.

Requirements:

* Starts with `<style>`
* Mobile responsive
* Modern dashboard layout
* Interactive sections
* Visual hierarchy
* Tables
* Cards
* Status badges
* Collapsible content

No Markdown should appear in the final artifact.

---

## Dashboard Sections

### 1. Summary

Provides a concise overview of the content.

Contents:

* Main topic
* Purpose
* Overall outcome

---

### 2. Key Takeaways

Displays major insights and highlights.

Examples:

* Important decisions
* Strategic conclusions
* Notable discoveries
* Critical updates

---

### 3. Action Items

Presented as an interactive table.

Columns:

| Field    | Description            |
| -------- | ---------------------- |
| Task     | Exact task description |
| Owner    | Responsible individual |
| Deadline | Due date               |
| Status   | Current progress       |

If information is missing:

Not specified

---

### 4. Open Questions

Captures unresolved topics.

Examples:

* Pending approvals
* Unanswered questions
* Research items
* Clarifications needed

---

### 5. Risks / Blockers

Tracks:

* Dependencies
* Obstacles
* Resource constraints
* External risks

---

### 6. Conflicts

Displays inconsistencies such as:

* Contradictory deadlines
* Multiple owners
* Conflicting decisions
* Mismatched requirements

Conflicts must never be automatically resolved.

---

### 7. Additional Notes

Stores supporting information that does not fit into other sections.

Examples:

* Context
* References
* Miscellaneous discussion points

---

### 8. Source Information (Merge Mode)

Lists all merged sources.

Examples:

* Meeting Notes A
* Brainstorm Session B
* Transcript C

---

## Status Badges

Supported badges:

🔴 High Priority

🟠 Medium Priority

🟢 Low Priority

⚠️ Conflict

❓ Open Question

✅ Completed

⏳ Pending

---

## Transcript Mode

Additional sections included:

### Speaker Summary

Summarizes discussion by speaker.

### Decisions by Speaker

Lists decisions associated with each speaker.

### Action Items by Speaker

Groups actions according to speaker ownership.

### Attribution Notes

Used when ownership or responsibility is unclear.

Speaker labels must remain exactly as provided.

---

## Merge Mode

Additional sections included:

### Duplicate Items

Highlights duplicate tasks, decisions, or notes found across sources.

### Conflict Resolution Review

Displays conflicts discovered during merging.

No automatic resolution is permitted.

### Source Notes

Shows origin of each merged item.

---

## UI Design Requirements

The generated dashboard should resemble:

* Notion
* ClickUp
* Linear
* Airtable
* Asana

Design characteristics:

* Responsive layout
* Dashboard cards
* Modern typography
* Soft shadows
* Hover effects
* Collapsible sections
* Status indicators
* Clean spacing
* Strong visual hierarchy

---

## Example Workflow

Input:

* Meeting transcript
* Voice memo
* Brainstorm notes

Processing:

1. Extract decisions
2. Extract action items
3. Extract open questions
4. Extract blockers
5. Identify conflicts
6. Organize supporting notes

Output:

A complete HTML dashboard containing structured project information with no invented data.

---

## Compliance Rules

Always:

* Preserve exact names
* Preserve exact dates
* Preserve exact numbers
* Preserve exact ownership
* Preserve exact terminology

Never:

* Assume ownership
* Create deadlines
* Resolve conflicts automatically
* Infer missing information
* Generate fictional content

If a value does not exist:

Display:

Not specified

---

## Final Output Requirement

Generate only a complete HTML artifact beginning with:

<style>

and ending with a valid HTML dashboard structure.

No explanations.
No markdown wrappers.
No commentary.
Only the HTML artifact.
