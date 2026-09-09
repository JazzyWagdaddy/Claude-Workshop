# Hands-On Lab: Prompting Basics, Projects, Skills, Connectors, and Custom Instructions

**Duration:** 30 minutes (10-minute prompting warm-up + 20-minute feature lab)
**Format:** Live, inside claude.ai
**Audience:** New learners, no prior Claude experience needed

## What you walk away with

You write and refine real prompts, then set up all four personalization features yourself, in order. You leave with a prompting habit and a decision framework for which feature to reach for on the job.

## Before you start (not counted in the 30 minutes)

Get these ready before the clock starts:

- A Claude account. Free, Pro, Max, Team, or Enterprise all work for this lab.
- Code execution turned on. Go to Settings > Capabilities and confirm it's enabled. Part 2, Station 3 needs it.
- One real file on your laptop you can upload. A template, a policy doc, a past deliverable. Anything you'd normally attach to an email.
- One real task from this week you can use as a live example. A job description to review, an email to draft, a report to summarize.
- Notifications off. You need 30 uninterrupted minutes.

---

# Part 1: Prompting Basics (10 minutes)

**Goal:** Learn what separates a vague prompt from a useful one, hands-on, before touching any of the advanced features.

## Warm-up: vague vs. specific (3 minutes)

**Steps**

1. Open a new chat.
2. Type this exact prompt: "Write me an email."
3. Read what comes back.
4. Now type: "Write a 100-word email to a client named Sarah. Tell her the project is delayed by one week. Keep the tone apologetic but confident."
5. Compare the two responses side by side.

**What to notice:** The first answer guessed at everything: the audience, the length, the reason for the email, the tone. The second one didn't have to guess. Specific input produces a useful output on the first try.

**Reflection question:** Think of something you asked Claude for recently that came back generic. What detail was missing?

## Give Claude a role and a format (4 minutes)

**Steps**

1. Pull up the real task you brought to this lab.
2. Write a prompt with three parts: who Claude should act as, what you need, and what shape the answer should take. Example: "Act as a hiring manager. Review this job description for clarity. Give me feedback as a numbered list of 5 items, most important first."
3. Swap in your own task using that same three-part structure.
4. Run it.

**What to notice:** The role and the format did most of the work. You never had to explain what "good feedback" means. Telling Claude who to act as and how to shape the answer did that for you.

**Reflection question:** Which part was hardest to write: the role, the task, or the format? That's usually the part people skip when a prompt falls flat.

## Iterate, don't restart (3 minutes)

**Steps**

1. Look at the response from the exercise above.
2. Instead of writing a new prompt from scratch, reply directly to what's on screen. Try one of these: "Make this shorter," "Give me three more examples like the second one," or "Assume the reader has never used Excel."
3. Send it and compare the new answer to the first one.

**What to notice:** You didn't retype your original request. Claude kept the context of the conversation. Refining beats restarting almost every time.

**Reflection question:** When a first answer isn't quite right, what's your instinct: retype from zero, or push back on what you got? Which one will you reach for now?

## Quick reference: the anatomy of a good prompt

- **Task:** what you actually want
- **Context:** who it's for, why it matters, what's already true
- **Format:** length, structure, tone
- **Role (optional):** who Claude should act as

---

# Part 2: Projects vs. Skills vs. Connectors vs. Custom Instructions (20 minutes)

## The four features in one line each

| Feature | What it does | Where it applies |
|---|---|---|
| Custom Instructions | Standing preferences that shape every response | Every conversation, everywhere |
| Projects | A workspace with files and instructions for one ongoing subject | Only inside that project |
| Skills | A reusable procedure Claude loads when a task calls for it | Anywhere Claude runs |
| Connectors | A live link to an outside app or data source | Any chat where you turn it on |

## Station 1: Custom Instructions (4 minutes)

**Goal:** Set a standing preference and watch it apply without asking.

**Steps**

1. Click your profile icon in the bottom left and open Settings.
2. Go to Profile and find "What preferences should Claude consider in responses?"
3. Write two sentences: one about your role, one about how you want Claude to respond. Example: "I run onboarding for a 40-person sales team. Keep answers under 150 words and skip the caveats."
4. Save it.
5. Start a brand-new chat, not inside a project, and ask something generic, like "how do I run a good 1:1?"

**What to notice:** Claude answered in your style without you asking. That's the whole feature. It now applies to every future chat, not just this one.

**Reflection question:** Would this same preference cause a problem in a totally different context, like a legal memo? If yes, it's too broad for Custom Instructions. That's your signal to use a Project or a Style instead.

## Station 2: Projects (5 minutes)

**Goal:** Build a workspace that already knows a specific subject before you type a word.

**Steps**

1. Click Projects in the left sidebar, or go to claude.ai/projects.
2. Click "+ New Project."
3. Name it something specific. Not "Work." Try "Q4 Client Onboarding."
4. Open the project and set Project Instructions. Tell Claude who it's working for, in this one context only.
5. Upload the file you prepared earlier.
6. Start a new chat inside the project and ask a question that depends on that file.

**What to notice:** Claude used the file without you attaching it to the chat. Every new chat inside this project starts already briefed. Chats outside the project don't carry any of this.

**Reflection question:** Custom Instructions applied everywhere. Project Instructions only applied inside this one project. What's a recurring subject in your own work that deserves its own Project?

## Station 3: Skills (5 minutes)

**Goal:** Watch Claude load a procedure on its own, only when the task calls for it.

**Steps**

1. Click "Customize" in the left sidebar, then the Skills tab.
2. Click the "+" button, then "Browse skills."
3. Install one Anthropic-built skill relevant to your work. Excel, Word, or PowerPoint creation are good starting points.
4. Go to any chat, inside or outside a Project, and ask for a task that skill covers. Example: "Build me a simple budget tracker in Excel."

**What to notice:** You never said "use the skill." Claude matched the task and loaded it automatically. It works the same way whether you're in a Project or a plain chat.

**Reflection question:** A Skill holds procedural knowledge, the how of a task. A Project holds background knowledge, the what and who of a subject. Where's the line for something you do the same way every week, like formatting a status report?

## Station 4: Connectors (4 minutes)

**Goal:** Give Claude access to a live outside source instead of a file you handed it.

**Steps**

1. Click "Customize," then the Connectors tab.
2. Click the "+" button, then "Browse connectors."
3. Pick one you actually use, like Google Drive, Gmail, or Slack, and click "Connect." Complete the sign-in.
4. Ask a question that requires current data, not a document. Example: "What's on my calendar tomorrow?" or "Find my most recent email from [name]."

**What to notice:** Claude didn't summarize a file you gave it. It pulled the actual current record. That's the core difference: Connectors read live systems. Projects and Skills only work with content you've directly provided.

**Note for Free plan users:** You get one custom connector. Pre-built connectors don't count against that limit, so start there if you're on Free.

## Wrap-up: the decision framework (2 minutes)

Ask these questions in order. Stop at the first "yes."

1. **Does this need to apply to every conversation, regardless of topic?** Use Custom Instructions.
2. **Is this an ongoing subject with its own files and context?** Use a Project.
3. **Is this a repeatable task I want done the same way, anywhere I work?** Use a Skill.
4. **Do I need Claude to see live, current data instead of a document I give it?** Use a Connector.

**The mistake to watch for:** People stuff formatting and tone rules into every new Project's instructions, then wonder why every Project feels like starting from zero. A preference that applies everywhere belongs in Custom Instructions once, not copied into each Project.

---

## Facilitator notes

- Part 1 works best when everyone brings a real task from their own week. A made-up example produces a weaker "aha" moment.
- Confirm code execution is on for every participant before Part 2, Station 3. It's the one prerequisite people forget.
- Free plan caps: 5 Projects, 1 custom connector. If your group is on Free, steer Station 4 toward pre-built connectors.
- Running short on time: cut Station 4 to a 2-minute group demo instead of hands-on, and protect the wrap-up. The decision framework is what people actually use back at their desks.
