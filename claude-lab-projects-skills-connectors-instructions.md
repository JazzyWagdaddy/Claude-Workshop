# Hands-On Lab - Projects vs. Skills vs. Connectors vs. Custom Instructions


## What you walk away with

You set up all four personalization features yourself, in order, and you leave with a decision framework for which one to reach for on the job.

## Before you start 

Get these ready before the clock starts:

- A Claude account for this lab.
- Code execution turned on. Go to Settings > Capabilities and confirm it's enabled. Station 3 needs it.
- One real file on your laptop you can upload. A template, a policy doc, a past deliverable. Anything you'd normally attach to an email.
- Notifications off. You need 20 uninterrupted minutes.

## The four features in one line each

| Feature | What it does | Where it applies |
|---|---|---|
| Custom Instructions | Standing preferences that shape every response | Every conversation, everywhere |
| Projects | A workspace with files and instructions for one ongoing subject | Only inside that project |
| Skills | A reusable procedure Claude loads when a task calls for it | Anywhere Claude runs |
| Connectors | A live link to an outside app or data source | Any chat where you turn it on |

---

## Exercise 1: Custom Instructions 

**Goal:** Set a standing preference and watch it apply without asking.

**Steps**

1. Click your profile icon in the bottom left and open Settings.
2. Go to Profile and find "Instructions for Claude"
3. Write two sentences: one about your role, one about how you want Claude to respond. Example:
    ```
   I run onboarding for a 40-person sales team. Keep answers under 150 words and skip the caveats.
    ```
4. Save it.
5. Start a brand-new chat, not inside a project, and ask something generic, like "how do I run a good 1:1?"

**What to notice:** Claude answered in your style without you asking. That's the whole feature. It now applies to every future chat, not just this one.

Make a few more iterations to your Custom Instructions based upon your role and persona.  Don't forget to save the changes and open a new chat to check out the results.

**Reflection question:** Would this same preference cause a problem in a totally different context, like a legal memo? If yes, it's too broad for Custom Instructions. That's your signal to use a Project or a Style instead.

---

## Exercise 2: Projects 

**Goal:** Build a workspace that already knows a specific subject before you type a word.

**Steps**

1. Click Projects in the left sidebar.
2. Click "+ New Project."
3. Name it something specific. Not "Work." Try "Q4 Client Onboarding."  Note that you can share this project across the company, or use it just for your purposes.  Click "Create Project".
4. Open the project and set Project Instructions. Tell Claude who it's working for, in this one context only.  The idea: instead of re-explaining your role, tone, or rules in every new chat, you write them once in the project's instructions field, and every conversation started inside that project automatically inherits them — alongside any files you've uploaded to the project's knowledge base.
5. Upload the file you prepared earlier.
6. Start a new chat inside the project and ask a question that depends on that file.  Be creative and use the T-C-O framework.

**What to notice:** Claude used the file without you attaching it to the chat. Every new chat inside this project starts already briefed. Chats outside the project don't carry any of this.

**Reflection question:** Custom Instructions applied everywhere. Project Instructions only applied inside this one project. What's a recurring subject in your own work that deserves its own Project?

---

## Exercise 3: Skills 

**Goal:** Watch Claude load a procedure on its own, only when the task calls for it.

### Load an Existing Skill

**Steps**

1. Click "Customize" in the left sidebar, then the Skills tab.
2. Click the "+" button, then "Browse skills."
3. Install the /learn skill by clicking the '+' button.  Click the "X" in the upper right corner several times to close the windows.
4. Open a new chat and type "/".  You will see all the skills available to your session.  Highlight or type "learn" followed by a topic of your choosing, such as "bitcoin" or "basketball".

**What to notice:** You never said "use the skill." Claude matched the task and loaded it automatically. It works the same way whether you're in a Project or a plain chat.

### Create Your Own Skill
1. Choose something you or your team does the same way every time — formatting meeting notes into action items, writing a weekly status update, converting a transcript into a client-ready summary. The narrower the task, the more useful the skill. Avoid vague goals like "write better emails."
2. Write down what "good" looks like - Grab a real example of the task done well — an input and the output you'd want from it. This becomes the reference Claude uses to understand the pattern you're teaching it, and it's the single biggest factor in whether the skill actually works.
```
create a skill to make all my responses sound like they are coming from <insert your favorite TV character like Tony Soprano or That 70's Guy>
```
```
I want a skill that turns raw meeting notes into a table of action items with owners and due dates. Here's an example of notes and the table I'd want back.
```
3. Paste your example. Claude will turn this into a SKILL.md file — the instruction file every skill needs — without you writing any YAML or code.
4. Check the name and description Claude gave it - Every skill has a short name and a one-line description. Claude reads that description to decide when to use the skill, so it needs to say exactly what the skill is for — "Formats raw meeting notes into an action-item table with owners and due dates" works; "helps with meetings" is too vague and won't trigger reliably.
5. Test it on a fresh example - Start a new chat and hand Claude a different set of notes than the one you used to build the skill. Confirm the skill actually fires and the output matches the pattern you taught. If it doesn't trigger, the description usually needs to be more specific.
6. Refine one thing at a time - If the output is close but not quite right, tell Claude what to fix and ask it to update the skill. Change one instruction, re-test, and repeat — don't try to fix five issues in the same edit, or you won't know which change worked.

**Reflection question:** A Skill holds procedural knowledge, the how of a task. A Project holds background knowledge, the what and who of a subject. Where's the line for something you do the same way every week, like formatting a status report?

---

## Exercise 4: Connectors 

**Goal:** Give Claude access to a live outside source instead of a file you handed it.

**Steps**

1. Click "Customize," then the Connectors tab.
2. Click the "+" button, then "Browse connectors."
3. Pick one you actually use, like Google Drive, Gmail, or Slack, and click "Connect." Complete the sign-in.
4. Ask a question that requires current data, not a document. Example: "What's on my calendar tomorrow?" or "Find my most recent email from [name]."

**What to notice:** Claude didn't summarize a file you gave it. It pulled the actual current record. That's the core difference: Connectors read live systems. Projects and Skills only work with content you've directly provided.

**Note for Free plan users:** You get one custom connector. Pre-built connectors don't count against that limit, so start there if you're on Free.

---

## Wrap-up: the decision framework (2 minutes)

Ask these questions in order. Stop at the first "yes."

1. **Does this need to apply to every conversation, regardless of topic?** Use Custom Instructions.
2. **Is this an ongoing subject with its own files and context?** Use a Project.
3. **Is this a repeatable task I want done the same way, anywhere I work?** Use a Skill.
4. **Do I need Claude to see live, current data instead of a document I give it?** Use a Connector.

**The mistake to watch for:** People stuff formatting and tone rules into every new Project's instructions, then wonder why every Project feels like starting from zero. A preference that applies everywhere belongs in Custom Instructions once, not copied into each Project.

---


