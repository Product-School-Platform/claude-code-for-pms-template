---
name: wrap-up
description: Ends a class session in the Claude Code for PMs course. Use it when the student says "wrap up" (or "wrap up this session", "let's wrap up", "end of session", "we're done for today", "I'm done with this module"). It saves the prompts the student wrote this session into that module's prompts.md, writes what they found under "What I found" in the same file (Modules 2 to 6), adds what the session figured out to the Working context in CLAUDE.md, checks the files Modules 5 and 6 build, and saves everything to GitHub.
---

# Wrap up

You're closing out a class session for a student in Product School's "Claude Code for PMs" course. They aren't technical, and they typed two words so they wouldn't have to type anything else. Their request is their yes: start right away with one plain sentence such as "Wrapping up today's session now." Don't ask them to type or paste anything unless a step below says to.

## 1. Work out which module this was

The module folders are 01-origin-story (Module 1), 02-super-hearing (Module 2), 03-rewind (Module 3), 04-x-ray-vision (Module 4), 05-super-speed (Module 5) and 06-sidekicks (Module 6).

- Use this session: the module the student's work and questions were about.
- If the session doesn't make it clear, use the first module folder whose prompts.md still has an empty numbered slot.
- If you still can't tell, ask one short question: "Which module was today, 1 to 6?"

## 2. Save the student's own prompts

- Look back through this session for the prompts the student wrote themselves. Leave out: the starter prompt each lab gives the whole room (the long, polished prompt the student pasted from a slide or the Zoom chat), "wrap up", "check my setup", "save my work", and short replies such as "yes", "ok" or "go ahead".
- Write them into that module's prompts.md, one per numbered slot (### 1., ### 2., ### 3.), in the order the student typed them, exactly as typed. Don't fix spelling, trim, reword or summarize.
- If there are more prompts than empty slots, add ### 4., ### 5. and so on.
- If some slots already hold prompts (from an earlier wrap-up), keep them and add the new ones after them. Never overwrite or delete anything already in the file.
- Leave the file's header text as it is.
- If the student wrote no prompts of their own this session, leave the file alone and say so.

## 3. Write what the student found (Modules 2 to 6)

Modules 2 to 6 have a "## What I found" section at the bottom of prompts.md, with one line per lab, each ending in blanks (___). Module 1 has none: skip this step for Module 1.

- Fill each blank from what the student said, decided and wrote in this session. Use their words, shortened to fit the line. Never invent a finding or take one from a classmate or from your own reading of the data.
- Keep each line's label and sentence frame exactly as written (for example "**Lab A, the interviews:** Based on the interviews, the trouble with 4.2 is ..."). Replace only the blanks.
- If the student didn't do a lab, or didn't reach a finding in it, leave that line with its blanks and tell them which lab it was.
- A line that already has a finding from an earlier wrap-up stays as it is, unless the student has changed their mind in this session. Then replace it.
- The lines per module:
  - Module 2: Lab A the interviews, Lab B the tickets, Lab C both piles.
  - Module 3: Lab A the pings, Lab B the pings and the tickets, Lab C one responder.
  - Module 4: Lab A the code, Lab B Marcus's question, Lab C how the code scores responders.
  - Module 5: Lab A, the brief.
  - Module 6: Lab A the skill, Lab B the schedule.

## 4. Add to the Working context in CLAUDE.md

- Under "## Working context", after everything already there, add three to six short plain lines: what this session figured out about Rook that isn't written there yet and that you'd want to know at the start of the next session. That means findings, which sources mattered, and questions still open.
- If the section still holds only the placeholder "_You'll fill this in during Module 1._", replace just that placeholder line.
- Module 3 only: also add the line "The responder I picked: <name>", using the responder the student followed in Lab C. Module 5's brief reads that line, and without it Claude has to stop and ask which responder to use. If the student didn't follow one, say so in the checklist and don't guess. If the line is already there from an earlier wrap-up, leave it.
- Don't repeat what's already there, don't add headings, and don't paste in whole documents.
- Never change anything above the "---" line (the session scope block).
- Rook is fictional. Keep all of this in CLAUDE.md: never save it to memory or anywhere outside the course folder.

## 5. Module 5 and Module 6: check the files the student built

The student saved these with the typed prompts on the lab slides. You don't write them: you check that they're there and that the save in step 6 picks them up. If one is missing, tell the student which one. Don't recreate it.

- Module 5: 05-super-speed/brief.md and 05-super-speed/prototype.html.
- Module 6: .claude/skills/review-checklist/SKILL.md (the skill), 06-sidekicks/monday-run.md (the report the scheduled task writes) and final-presentation.html (at the top of the course folder). If monday-run.md is missing, the task may not have run yet or may have been created from a different folder: say so in one plain sentence.

## 6. Save to GitHub

Follow the "save my work" routine in the course-setup skill (.claude/skills/course-setup/SKILL.md and its references/saving-work.md), with a short message such as "Module 2 wrap-up". The save commits everything in the folder, so the files from step 5 go with it: in Module 5 the whole 05-super-speed folder, in Module 6 the skill, monday-run.md and final-presentation.html next to prompts.md. Handle every problem exactly the way that routine says.

## 7. Tell the student

A short checklist, then the link:

✓ Saved your prompts to <module folder>/prompts.md (how many)
✓ Wrote what you found in prompts.md (Modules 2 to 6; say which labs have a finding and which are still blank)
✓ Added what we learned today to CLAUDE.md (Module 3: and saved the responder you picked)
✓ Module 5: brief.md and prototype.html are in 05-super-speed. Module 6: your skill, monday-run.md and final-presentation.html are saved
✓ Saved to GitHub: https://github.com/<their username>/claude-code-for-pms-final

If a step didn't work, mark it ✗ and give the fix in one plain sentence. If saving to GitHub failed, tell them their prompts and notes are safe on this computer and what to do next, per the save routine.
