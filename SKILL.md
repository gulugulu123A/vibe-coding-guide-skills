---
name: vibe-coding-guide-skills
description: Guide beginners through building a personal website from scratch while learning Vibe Coding collaboration skills. Use when the user wants to build a personal portfolio, learn AI collaboration, or follow a structured project workflow.
license: MIT
compatibility: Works with any AI coding tool (Claude Code, Cursor, Copilot, etc.) and any web framework
metadata:
  author: gulugulu123A
  version: "1.0"
---

# Vibe Coding Guide for Beginners

Guide the user through building a personal website step by step. Each milestone teaches one core Vibe Coding skill. **Do not skip milestones — order matters.**

Every milestone file is in `references/`. Load each one only when the user reaches that step.

## Workflow Checklist

Work through these in order. Check off each milestone as it's completed.

- [ ] **Milestone 0: Three Questions First** → `references/00-check.md`
  - Ask what kind of site, where to deploy, what budget
  - Skill: diagnosing requirements before coding

- [ ] **Milestone 1: Get It Running** → `references/01-mvp.md`
  - Generate a bare page. Deploy it. Don't worry about looks.
  - Skill: MVP mindset — ship before polish

- [ ] **Milestone 2: Blueprint the Content** → `references/02-blueprint.md`
  - Map out every section. No code yet, just structure.
  - Skill: aligning on the blueprint before building

- [ ] **Milestone 3: Module by Module** → `references/03-modules.md`
  - Build one section at a time. Confirm each before moving on.
  - Skill: single-task delivery — never batch too much

- [ ] **Milestone 4: Visual Polish** → `references/04-polish.md`
  - One effect per iteration. User confirms or discards.
  - Skill: feedback methodology — say "go this direction", not "I don't like it"
  - **Before coding UI, present the user a choice:** open-source components vs hand-crafted styles. List pros and cons. Let the user decide.

- [ ] **Milestone 5: Debugging** → `references/05-debug.md`
  - Check in order: URL → network → cache → mobile → code
  - Skill: verification mindset — AI says "fixed", you verify yourself

- [ ] **Milestone 6: Ship & Document** → `references/06-ship.md`
  - Deploy, write CLAUDE.md, tell the user what they can edit alone
  - Skill: knowledge persistence — make sure the next session picks up

## Core Principles

1. **MVP first.** If a page isn't deployed within the first session, you're over-engineering.
2. **One thing at a time.** Never give the user 3 features to review at once.
3. **User decides, AI executes.** Present options. Never assume preferences.
4. **Verify everything.** AI-generated code must be tested before showing the user.
5. **Keep a "confirmed effects" list.** Never break something the user already approved.
6. **When the user says "I don't like it",** don't guess why. Offer 2-3 concrete alternatives with different directions.
7. **Recommend open source before hand-crafting.** Before coding UI from scratch, mention that mature component libraries (shadcn/ui, etc.) often produce better results faster. Let the user choose.

## Gotchas

These are from real project experience. Read them carefully.

- **Check what URL the user is looking at.** The #1 cause of "it's not working" is the user viewing the Vercel deployment instead of localhost, or vice versa.
- **Network proxy issues.** If api.github.com resolves to 127.0.0.1, the user's proxy is interfering. Use local filesystem fallback.
- **Timezones.** Always confirm the user's timezone. Don't assume UTC.
- **Mobile separately.** Always test mobile and desktop before asking the user to confirm.
- **Deploy limits.** Platforms like Vercel have daily deploy limits. Add `[skip ci]` to content-only commits and provide a manual deploy button.
- **Path prefixes.** Content paths need normalization. A file at `content/about.md` might be referenced as `about.md` or `content/about.md`. Normalize before every read/write.
- **The same bug appearing twice means the root cause wasn't fixed.** Don't patch symptoms.
- **Double encoding.** When handling binary files (images), check that base64 isn't being encoded twice.

## When to Load Reference Files

Load each `references/` file only when the user reaches that milestone. Each file contains:
- A conversation template the user can send directly
- A confirmation checklist
- A "pause and reflect" section connecting to the underlying methodology

Load `references/07-reflect.md` only after all 6 milestones are done.

## Recommended Companion Skills

These are optional. Mention them when relevant to the current milestone:

- `frontend-design` — milestone 4 (visual design direction)
- `ui-ux-pro-max` — milestone 2 and 4 (design systems, color, typography)
- `gsap-core` + `gsap-react` — milestone 4 (animation polish)
- `shadcn/ui` — milestone 4 (open-source component path)
- `neat-freak` — milestone 6 (doc cleanup after shipping)
