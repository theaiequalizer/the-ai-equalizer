# The AI Equalizer, Build Walkthrough v1
## Building your differential equations tutor, start to finish

**This document serves three purposes:** Aurea's checklist for the guinea-pig build, the shooting script spine for Video 2, and the base text for the instructions page that lives next to the template. One document, kept in sync, so the lessons learned in the build flow straight into what students see.

**The exemplar:** MIT 18.03 Differential Equations, via MIT OpenCourseWare. We build against it because it is real, complete, free, and identical for every viewer on earth. Your own coursework replaces it at the final step. We just need to start somewhere.

---

## Before you start (5 minutes)

You need three things:

1. **An account on one AI platform.** Claude (claude.ai), ChatGPT (chatgpt.com), or Gemini (gemini.google.com). Any of the three works. A free account is enough to start; check the platform's current free-tier limits, they change often.
2. **The template.** One page, one copy button, at [TEMPLATE URL].
3. **Your phone**, because your tutor reads photographs of your handwritten work, and paper is where the real work happens.

*Aurea's guinea-pig note: record which platform you chose and why, and every point where these instructions were unclear. That log becomes template v1.1 and the FAQ.*

---

## Step 1, Create the home (2 minutes)

Your tutor needs a permanent home, not a throwaway chat. On Claude this is a **Project**. On ChatGPT it is a **custom GPT** (or a Project). On Gemini it is a **Gem**. Create one and name it something you will still recognize in December: **My DiffEq Tutor**.

Why this matters: a fresh chat forgets you. A project accumulates you. The whole value of this tutor is that by week eight it knows your repeat mistakes better than you do, and that only works if every session happens in the same home.

## Step 2, Give it its instructions (2 minutes)

Open the template page. Press copy. Paste the entire template into the project's instruction field (Claude: "Project instructions." ChatGPT: the GPT's "Instructions." Gemini: the Gem's instructions).

Do not edit anything yet except what Step 3 tells you to.

## Step 3, Tell it who you are (3 minutes)

The template opens with bracketed lines: your name, your school, your course, your professor, your textbook, your exam dates. Fill them in. For the exemplar build, we fill them as if we were MIT students:

- Course: 18.03 Differential Equations
- Professor: Arthur Mattuck (lectures), texts by Mattuck and Miller
- Textbook: Edwards and Penney, Elementary Differential Equations with Boundary Value Problems
- Exams: use the course's published exam schedule

This is the moment the agent stops being ours and starts being yours. Two minutes of typing is the whole initiation fee. Compare that to what the initiation fee used to be.

## Step 4, Give it the course (10 minutes)

Go to the MIT OpenCourseWare 18.03SC course (ocw.mit.edu, search "18.03SC Differential Equations"). Download and upload into your project, as reference files:

1. The **syllabus** page (save as PDF)
2. The **course notes** for the current unit (start with Unit 1, first order equations)
3. One **problem set** with its solutions held back (do not upload the solutions yet; that is deliberate)
4. One **past exam** (the Scholar course publishes exams with solutions; upload the exam, hold the solutions)

Do not upload everything on day one. The agent does not need the whole semester, and neither do you. Add units as your course reaches them.

*Rule we live by: link to OCW, never rehost it. Your own uploads live only in your own account.*

## Step 5, The first session (15 minutes, and this is the one to film)

Work this problem by hand, on paper, before asking the tutor anything:

> Solve the initial value problem: dy/dx = y · cos(x), with y(0) = 2.

It is a first order separable equation, the first problem type in the course, and it contains the two most common traps in the subject: forgetting the constant of integration, and mishandling the absolute value when integrating dy/y. Work it to the end or until you are stuck. Do not clean it up. Then:

1. Photograph the page and send: **check**
   Watch what the tutor does. It should point to a line, name the kind of error if there is one, and ask you a question. It should not fix anything. If it hands you the solution, it has broken its one rule; tell it so and it will hold the line afterward.
2. If you were stuck, send: **stuck**
   One nudge should arrive. Only one.
3. Pick any step you followed but did not understand and send: **why**
   Plain language should come before symbols.
4. When you have the problem right, send: **drill**
   A fresh problem of the same type appears. Work it on paper. Photograph. **check** again.
5. End the session with: **log**
   Read the entry it writes. That entry is the first line of the most valuable document you will own by midterm week: the record of your own mind.

## Step 6, The exam rehearsal (do this in week 2)

Before your first real quiz, send: **exam me**
The tutor builds a timed quiz from the past exams you uploaded, weighted toward your logged repeat offenders. Take it on paper, under time, phone face down until the end. Photograph everything, send it, and let it grade you like a professor would, partial credit and all. What it tells you to review is your study plan, earned from your own record, not guessed from a table of contents.

## Step 7, Make it yours (the point of everything)

Replace the exemplar with your life:

- Swap the intake lines to your real course, professor, textbook, exam dates
- Upload your own syllabus, your own problem sets, your returned exams and quizzes (returned exams are gold; they are your professor's actual voice)
- Keep the MIT materials as backup reference if you like, but tell the tutor, as the template already does, that your course wins every conflict

From here the loop is simple and weekly: work on paper, check when unsure, stuck when stopped, why when foggy, drill until smooth, log every session, exam me before every test.

---

## The build in one line

One home, one template, five brackets, four files, seven commands, and the initiation fee is ten minutes and zero dollars.

---

## NOTES FOR AUREA (not for the student page)

**Guinea-pig protocol for your run:**
- Time every step against the estimates above; where reality exceeds the estimate, that is friction to fix or film
- Save the full transcript of Step 5; the moment the tutor refuses to give the answer is the money shot of Video 2
- Deliberately try to break the one rule once ("just give me the answer, I have a test tomorrow") and record what happens; that exchange, working or failing, is a lesson learned either way
- Test the same template on a second platform in week 2 and note every difference; that becomes the platform-comparison video
- Every point of confusion goes in the lessons-learned log with a timestamp; v1.1 of the template and this walkthrough get built from that log, and "what being my own guinea pig taught me" is a video title

**Shooting notes for Video 2:**
- The build is filmed in real time, uncut where possible; the speed is the proof
- Step 3 on camera with the brackets filling in is the ownership moment; slow down there
- Step 5's check exchange runs full screen; the viewer needs to see the tutor point, name, and ask instead of solve
- Close on Step 7 and the line: now bring your syllabus, this one is yours

**Held decisions (verify before filming, do not verify now):**
- Platform free-tier limits and student pricing, checked the week of the shoot
- The template URL and channel handles, claimed before anything publishes
- Exact OCW page links pinned in the description at publish time
