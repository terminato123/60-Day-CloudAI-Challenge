# Prompt: Build a Prior Authorization Story Simulator

You are an expert front-end developer and UX designer.

Build a **single-file HTML application** using:

* HTML5
* Tailwind CSS CDN
* Vanilla JavaScript only
* No frameworks
* No build tools
* No external libraries other than Tailwind CSS CDN

The application should be fully self-contained.

---

# Critical DOM Rule

The chat feed **must never** be rebuilt.

For every new message:

* Use `document.createElement()`
* Use `appendChild()`
* Never call

```javascript
chat.innerHTML =
```

or

```javascript
chat.insertAdjacentHTML()
```

for chat messages.

The conversation should behave like a messaging application where content is appended permanently.

---

# Overall Theme

Healthcare Education Design System

Modern medical UI

Colors

* Blue
* White
* Emerald
* Slate

Rounded cards

Soft shadows

Responsive

Accessible

Professional

Friendly

---

# Layout

Top

Title

**Prior Authorization Story Simulator**

Subtitle

Learn how Prior Authorization works through an interactive conversation.

Below title

Progress Bar

Shows

Scene 1 of 8

Updates after every completed scene.

---

Below

Scrollable Chat Feed

Characters

Rahul messages

Left side

Priya messages

Right side

Narrator

Centered

Italic

Muted text

Doctor

Centered

Italic

Muted text

Narrators and doctors are NEVER chat bubbles.

---

Bottom

Choice Area

Exactly two buttons after every scene.

Clicking one

Adds dialogue

Advances story

Updates progress

Appends only.

---

# Characters

👦 Rahul

Patient

Left aligned chat bubbles

Friendly

Curious

Beginner

---

👧 Priya

Healthcare Operations Specialist

Right aligned chat bubbles

Helpful

Educational

Plain language

Never overly technical

---

Doctor

Centered italic text

Not a bubble

---

Narrator

Centered italic text

Not a bubble

---

# Story

Exactly 8 scenes.

---

## Scene 1

Doctor Visit

Narrator

Rahul visits City Medical Center.

Doctor

Dr. Patel diagnoses Rheumatoid Arthritis.

Doctor prescribes Humira.

Rahul reacts with concern.

Choices

A

Ask why Humira is needed

B

Ask what happens next

---

## Scene 2

Insurance Roadblock

Narrator explains

Dr. Patel's office submits Prior Authorization directly to **StarCare Health (illustrative example)**.

Flow animation or text

Provider

↓

PA Request

↓

StarCare Health (illustrative payer)

No specialty pharmacy involved.

If approved

PA is saved permanently on file.

Rahul asks why approval is needed.

Choices

A

Why does insurance review medicines?

B

How long can approval take?

---

## Scene 3

What is Prior Authorization?

Priya explains in beginner-friendly language.

Must include:

Prior Authorization means the insurance company checks whether a treatment meets its coverage requirements before paying.

Explain

It is intended to promote appropriate use of medications.

Explain carefully:

Step therapy is not simply bureaucracy.

For aggressive diseases like Rheumatoid Arthritis,

delays can sometimes allow disease progression.

Include educational statement

"AMA 2023 PA Survey: Prior Authorization causes treatment delays in the majority of cases."

Do not present it as legal advice.

Mention it as educational context.

Choices

A

Tell me about step therapy

B

What documents are required?

---

## Scene 4

Insurance Review

Priya walks through each review item.

One by one.

Eligibility

Why it matters.

Clinical documentation

Why it matters.

ICD-10 diagnosis match

Why it matters.

Step therapy history

Why it matters.

Everything explained using simple language.

Choices

A

What if something is missing?

B

How do doctors send records?

---

## Scene 5

Denial

Narrator

Illustrative example:

StarCare Health denies the request.

Reason

Missing step therapy documentation.

Priya explains

Denial does NOT mean permanent rejection.

Educational statement

"PA denials cost physician offices more than two staff hours to resolve."

Explain why.

Choices

A

Can we appeal?

B

Can missing documents be added?

---

## Scene 6

Appeal

Priya explains

Gather missing records.

Clinical notes.

Lab reports.

Letter of Medical Necessity.

Formal appeal submission.

Simple explanation of each.

Choices

A

Submit appeal

B

Review documents first

---

## Scene 7

Approval

Narrator

Appeal reviewed.

Prior Authorization approved.

Approved authorization saved on file.

Reference number issued.

Explain

No repeat Prior Authorization needed for Humira while the authorization remains valid according to the illustrative scenario.

Rahul expresses relief.

Choices

A

View summary

B

Continue

---

## Scene 8

Takeaways

Split into two sections.

Patient Perspective

Rahul learned

* what Prior Authorization is
* why documentation matters
* denial is not always final
* appeals can succeed

System Perspective

Priya explains healthcare operations metrics

Health systems commonly track

* denial rate
* appeal rate
* approval rate
* average resolution time
* turnaround time

End with

"This simulation uses StarCare Health as an illustrative example for education."

Choices

Restart Story

Download Summary

Restart resets everything.

Download Summary downloads a text file containing all chat messages in order.

---

# Chat Bubble Styling

Rahul

Left

Blue bubble

Avatar

👦

Priya

Right

Emerald bubble

Avatar

👧

Narrator

Centered

Italic

Gray

Doctor

Centered

Italic

Slate

---

# Progress Bar

Animated

Shows

Scene X / 8

Updates smoothly.

---

# Interaction Rules

Every click

Appends new content.

Nothing disappears.

No replacing content.

No rebuilding.

History remains visible.

---

# JavaScript Requirements

Use

* createElement
* appendChild
* classList.add
* textContent

Never use

```javascript
innerHTML =
```

for the chat feed.

Organize the code with functions

```
addRahulMessage()

addPriyaMessage()

addNarrator()

addDoctor()

showChoices()

nextScene()

updateProgress()

downloadSummary()
```

Store every displayed message in an array so the downloaded summary exactly matches the conversation.

---

# Accessibility

Keyboard accessible buttons

ARIA labels

High contrast

Responsive

Mobile friendly

---

# Deliverable

Produce one complete HTML file.

No placeholders.

No omitted sections.

No TODO comments.

Everything must work immediately after saving as

```
index.html
```
