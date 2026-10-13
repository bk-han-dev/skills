---
name: Brief To Video Creator By BK Han
description: Use when making a video (promo, story, explainer) from a rough idea. Interview to a production brief, then storyboard, clip prompts, generation and final cut, packaged as reusable agent skills.
---
# Brief To Video Creator

Video pipeline (White Tiger Ridge example): Idea -> Brief (idea-to-brief) -> Storyboard & references (a sheet per character) -> Prompts (brief-to-video skill, timed shots e.g. 14 clips) -> Video clips (same cast throughout, clip engines generate up to ~30 s per clip) -> Final cut with captions.

Method from "Build Your Own Creative Agent Skills" (AICON 2026 masterclass by Tianyu Xu, 8 Oct 2026, *SCAPE, Singapore). Teach AI your taste; keep the work yours.

## 1. Mindset (AIBLE)
- Foundation = Adapt (change your mind fast). Engine = Innovate + Leverage (agent skills live here). Moat = Brand + Execute (your taste stays yours).
- A skill is NOT a custom GPT: it is a file-based folder (SKILL.md) that the agent loads on its own when the task matches. No manual prompting.

## 2. Build the folder
```
my-skill/
  SKILL.md        # required: name, description (when to use / triggers), steps, outputs, checks
  references/     # optional: guides, examples, templates for the AI to read
  scripts/        # optional: small Python checks/automations
  assets/         # optional: design templates, images
```

## 3. Start with idea-to-brief (the hinge)
1. IN: rough idea, brain dump, voice note, or one line.
2. RUN: short 5W1H interview (who, what, when, where, why, how). Ask only what's missing, a few questions at a time.
3. OUT: a 500-1,000 word production brief with fixed sections (assets, acts, lighting, story, or equivalents).
Files: references/question-bank.md, references/brief-template.md (exact sections by heading), references/example-brief.md (the gold standard), scripts/brief_lint.py (checks structure before the next phase).
Get the brief right once and every downstream skill (deck, website, video story) inherits your taste.

## 4. Chain downstream skills
- Slides: Content + Context (brief) + Design System (style decided once) x AI Engine (writes HTML) = final deck, no slide tool needed.
- Styles: code-drawn aesthetics (e.g. pixel art, Bauhaus, synthwave) via code, no image model required.
- Video: Idea -> Brief -> Storyboard & references -> Prompts (brief-to-video skill) -> Clips -> Final cut with captions.
- Same pattern extends to headless pipelines (3D, games).

## 5. Cost check
Estimate the compute burn before producing (per second of finished video, images, LLM). Remember human time (about 3-8 h per finished minute), software and licensing on top.

## 6. Portability
A skill is one plain folder; Agent Skills is an open standard read by Claude, ChatGPT, Codex and Gemini. Zip tip: Claude wants the folder inside the zip; Gemini wants SKILL.md at the top.

## Rules
- Draft only. Nothing is published, sent, or changed without the owner's approval.
- Confirmation lists: number each item, end with an "All" option.
- Don't claim to have coined terms already in use (e.g. "liveBook" is Manning's).
