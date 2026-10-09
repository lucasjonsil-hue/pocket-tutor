# Pocket Tutor

A personal tutor for Claude that drills you to mastery from **your own class notes** — one question at a time.
Any subject. It learns how you learn and gets better the more you use it.

- **Flash learning** — rapid one-line questions, Correct/Incorrect, one-line why, next.
- **Recheck list** — anything you miss comes back later in a new scenario.
- **Game mode** — say "game mode" on low-energy nights: hearts, streaks, bosses, a career ladder.
- **Pen mode** — write answers on paper, send a photo, get graded.

It's for *learning*, not doing your homework for you.

---

## Install (pick one)

### A. Claude app (Pro plan) — easiest
1. Download **[pocket-tutor-skill.zip](pocket-tutor-skill.zip)** from this repo (click it → Download).
2. In Claude: **Settings → Capabilities → Skills → Upload skill** → pick the zip.
3. Make sure the skill is toggled **on**.

### B. Claude Code — one line
Mac / Linux:
```bash
git clone https://github.com/lucasjonsil-hue/pocket-tutor /tmp/pocket-tutor && mkdir -p ~/.claude/skills && cp -r /tmp/pocket-tutor/skills/pocket-tutor ~/.claude/skills/
```
Windows (PowerShell):
```powershell
git clone https://github.com/lucasjonsil-hue/pocket-tutor $env:TEMP\pocket-tutor; New-Item -ItemType Directory -Force "$HOME\.claude\skills" | Out-Null; Copy-Item -Recurse "$env:TEMP\pocket-tutor\skills\pocket-tutor" "$HOME\.claude\skills\"
```

### C. Free plan — Claude Project
1. Create a Project called **Pocket Tutor**.
2. Open [`skills/pocket-tutor/SKILL.md`](skills/pocket-tutor/SKILL.md), copy everything, paste it into the Project's instructions.
3. Chat inside that Project.

---

## First run

Say: **"set me up"**

It asks what classes you're taking, then you drop in your syllabus, notes and slides (messy is fine).
It builds one folder per class and starts quizzing you.

Then just say things like:
- "quiz me" · "flash mode" · "quiz me on what I got wrong" · "game mode" · "add a class"

Want to set up folders by hand instead? Copy [`starter/Pocket Tutor`](starter/Pocket%20Tutor) to your Documents folder.

---

## Privacy

Your notes, grades and progress stay in **your** files/Project. Nothing comes back to this repo.
Don't commit your own class files if you fork it.
