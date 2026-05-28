English | [中文](./README.md)

---

# Vibe Coding Guide for Beginners skills

> Build a personal website from scratch and learn how to collaborate effectively with AI.

## What is Vibe Coding? A Beginner's Explanation

If this is your first time hearing the term, the following should help.

### 1. What does "Vibe Coding" mean?

"Vibe" means atmosphere or feeling. "Coding" means programming. Together, the plain meaning is: **you don't write code — you tell AI what you want in plain language, and AI writes the code for you.**

It's like describing your ideal home renovation to a designer. You don't need to know how to draw blueprints, but you do need to say "I want warm tones, wooden floors, and large floor-to-ceiling windows." In Vibe Coding, AI is the person drawing the blueprint for you.

### 2. Do I need to know how to code?

No. But you need to be willing to do three things: **clearly describe what you want, tell good from bad, and iterate repeatedly.**

These sound simple, but each takes practice. Many people get stuck at the first step — they have a vague picture in their head but can't put it into words. A big part of this guide helps you build exactly that skill.

### 3. What can I build with Vibe Coding?

Websites, mini-programs, automation scripts, personal blogs, admin dashboards… essentially any software product you see in daily life can be built to some degree with Vibe Coding. It might not be perfect, but it will **work**.

This guide uses "building a personal website" as your first project because it's the most beginner-friendly — you see results as you go, and you can use it immediately.

### 4. How is it different from "asking ChatGPT a question"?

Asking ChatGPT is a one-off interaction — you ask, it answers, done.

Vibe Coding is an ongoing collaboration — you open an AI coding tool and go back and forth with AI for hours or even days, building a project from scratch together. You don't just ask one question and leave. You follow up, tweak, adjust, debug — like working with a partner.

### 5. Why do I need a "method"? Can't I just chat with AI?

You can. But you'll likely run into the same problem: **everything goes smoothly at first, then you hit a wall halfway through.**

The reason is usually not that AI got dumber — it's that you gave it too much at once. AI has limited context, like a person who can only remember the last 20 minutes of conversation. If you ask it to build an entire website in one go, it will definitely miss things.

That's why **method matters** — knowing how to break down tasks, how to push forward step by step, and how to not panic when things go wrong. These are the real thresholds of Vibe Coding.

### 6. What tools do I need? Does it cost money?

Here are the mainstream AI coding agents available today:

| Tool | Description |
|---|---|
| **Claude Code** | Currently the best all-around coding agent, with VS Code plugin support |
| **Cursor** | Graphical interface, great for those not comfortable with the command line |
| **GitHub Copilot** | Deep VS Code integration, suited for users with some dev experience |
| **Codex (OpenAI)** | By OpenAI, cloud-based |

**Recommended starter setup: Claude Code + Chinese LLMs**

Claude Code's official model isn't easily accessible in China, but it supports third-party model integration. You can pair it with Chinese models like DeepSeek, GLM, MiniMax, and others — affordable, with better Chinese comprehension, and low entry cost.

For installation guides, we recommend this tutorial by Khazix, which walks beginners through setup step by step:  
https://mp.weixin.qq.com/s/AA2NHww4jUBuAfi10EYICw

You don't need to buy any paid courses. Free resources online are more than sufficient to get started.

### 7. How does this guide help me?

This guide doesn't teach you how to code — it teaches you **how to collaborate with AI**.

It uses "building a personal website" as your first hands-on project, broken into 7 steps. Each step tells you: what to do, how to talk to AI, what to check when done, and what ability this step is training.

Follow through once, and you'll walk away with not just a website, but a repeatable method you can apply to any future project.

### 8. A Note from the Author

One last thing: don't feel like Vibe Coding has a high barrier to entry. Like learning anything new, the best way to start is to just take the first step.

There are many tutorials out there — most are thorough, but also lengthy. Our suggestion: you don't need to finish every resource before getting your feet wet. Learn the basics, then jump into a small project. Look things up when you hit a snag. Learning with a problem in hand sticks better than memorizing theory upfront.

**Learn by doing, do by learning.** That's the rhythm we've found works best for getting into Vibe Coding. Of course, if you prefer to study systematically before diving in, that's perfectly fine too — go at your own pace.

We hope this guide helps you take that first step.

## What This Is

A hands-on Vibe Coding playbook that uses **building a personal website** as a complete case study. By the time you finish the project, you'll naturally understand:

- How to clearly communicate what you want to AI
- How to break a project into AI-digestible steps
- How to troubleshoot without panicking when AI writes buggy code
- How to assess your current skill level and what to practice next

**This guide does not teach specific technologies — it teaches methodology.** Switch frameworks or AI tools, and the approach still works.

## Who This Is For

- First-timers using AI to build a project, not sure where to start
- People who've tried AI but find it "hit or miss" and can't explain why
- Anyone wanting to systematize their AI collaboration workflow

## How to Use

Work through 7 milestones in order. Each milestone includes:

| Section | What It Covers |
|---|---|
| **What to Do** | The goal and expected output for this step |
| **Conversation Template** | Copy-paste prompts you can send directly to your AI |
| **Confirmation Checklist** | Things to verify before moving on |
| **Pause and Reflect** | What you learned and which core skills you're building |

## Installation & Usage

### Method 1: Install as a Skill (Recommended — auto-activates)

Copy and send this to your AI coding agent (works with Claude Code, Cursor, Copilot, Codex, etc.):

```
Install a skill from https://github.com/gulugulu123A/vibe-coding-guide-skills, then walk me through starting from Milestone 0.
```

Your agent will clone it into its skills directory. After that, whenever your request involves building a website, the agent will detect the metadata in `SKILL.md` and activate this skill automatically.

### Method 2: Manual terminal install

```bash
# Clone into your agent's skills directory (Claude Code example path)
git clone https://github.com/gulugulu123A/vibe-coding-guide-skills.git ~/.claude/skills/vibe-coding-guide-skills
```

Restart your AI coding tool, or activate manually:

```
/skill vibe-coding-guide-skills
```

### Method 3: Use as documentation (without installing as a skill)

```bash
git clone https://github.com/gulugulu123A/vibe-coding-guide-skills.git
cd vibe-coding-guide-skills
```

Open this directory with your preferred AI tool and say:

> Reference the docs in this directory and guide me through building a personal website starting from Milestone 0.

## Table of Contents

- [Milestone 0: Three Questions Before You Start](./references/00-check.md)
- [Milestone 1: Get a Page Running](./references/01-mvp.md)
- [Milestone 2: Map Out Your Content Structure](./references/02-blueprint.md)
- [Milestone 3: Ship Module by Module](./references/03-modules.md)
- [Milestone 4: Visual Polish — The Iteration Method](./references/04-polish.md)
- [Milestone 5: Debugging Mindset](./references/05-debug.md)
- [Milestone 6: Ship It and Document It](./references/06-ship.md)
- [Final Chapter: Where You Stand on the Vibe Coding Map](./references/07-reflect.md)

## Core Philosophy

> Skills can be supplemented by AI. Collaboration methods cannot. The essence of Vibe Coding isn't "letting AI write code" — it's knowing how to make AI produce what you want.

This guide weaves together three frameworks:

1. **Six Foundational Traits** (curiosity, reliability, fact-checking obsession, cross-disciplinary thinking, tolerance for uncertainty, low ego + high drive) — these determine whether you'll go far in the AI era
2. **Ten Levels of AI Proficiency** (Lv.0 Observer → Lv.10 One-Person Army) — to help you see where you are and where to go next
3. **Content Creation Three-Step Method** (gather info → find an angle → create) — building a website, like writing, is about storytelling. The angle matters more than execution.

## A Final Word

AI is evolving at breakneck speed. When you finish building a project with this guide, you will be genuinely amazed by what AI can do — that's normal. Everyone has that moment the first time.

But here's something more important: **don't become over-reliant on AI.**

The ability to keep learning and thinking deeply is more valuable than ever in the AI era. When AI levels the playing field on execution, a hundred people using the exact same AI tools will still produce outputs a hundred times apart in quality.

The gap doesn't come from the tools. Not from the techniques. Not from whose Skill file is fancier. **It comes from what's inside a person's head.** Their understanding of the world. Their taste. Their value system. Their sense of what is good. These are things AI cannot give you.

The endgame of tool democratization is not the democratization of people — it's the opposite.

AI doesn't stop evolving. It's not a skill you learn once and put aside. It evolves, and your relationship with it evolves too. So in this chaotic era, figure out who you want to become — and move forward. Don't look back.

Always stay curious.

## Recommended Skills

These are battle-tested skills we used during the actual build. Each is an independent open-source project — **entirely optional, not a dependency of this guide**.

### `frontend-design`
- **What it does**: Generates high-quality, distinctive frontend interfaces that avoid generic AI aesthetics
- **Pros**: Unique visual output; built-in design language references
- **Cons**: Can generate too much code; may be overkill for simple pages

### `ui-ux-pro-max`
- **What it does**: 50+ design styles, 161 color palettes, 57 font pairings, 99 UX guidelines
- **Pros**: Acts as a portable design consultant; covers 10 tech stacks
- **Cons**: Steep initial learning curve; some styles lean Western-centric

### `gsap-core` + `gsap-react`
- **What it does**: Professional JS animation engine — scroll-driven, spring easing, timeline orchestration
- **Pros**: Does what CSS can't (staggered reveals, 3D tilt, spring modals); excellent performance
- **Cons**: Learning curve; plugins like ScrollTrigger need separate registration; some advanced plugins are paid

### `shadcn/ui`
- **What it does**: Source-level open-source component library — buttons, modals, forms, menus
- **Pros**: Code lands in your project, not node_modules; full control; active community
- **Cons**: React/Vue only; requires Tailwind CSS to configure

### `neat-freak`
- **What it does**: Post-session doc audit, CLAUDE.md sync, stale memory cleanup
- **Pros**: Prevents documentation rot; ensures the next AI session picks up correctly; OCD-level rigor
- **Cons**: Cleanup process can be time-consuming; may require multiple confirmation rounds

## Acknowledgements

Thanks to the following open-source projects and communities:

- **[frontend-design](https://github.com/anthropics/claude-code/tree/main/plugins/frontend-design)** — Frontend design skill
- **[ui-ux-pro-max](https://github.com/nextlevelbuilder/ui-ux-pro-max-skill)** — UI/UX design intelligence skill
- **[GSAP](https://github.com/greensock/gsap-skills)** — Professional JavaScript animation library
- **[shadcn/ui](https://ui.shadcn.com)** — Open-source component library
- **[neat-freak](https://github.com/KKKKhazix/khazix-skills/tree/main/neat-freak)** — Documentation and memory cleanup skill
- **WeChat Official Account [数字生命卡兹克]** — The foundational methodology of this guide draws from Khazix's deep insights on six AI-era traits, ten proficiency levels, and the three-step content creation framework, with thanks for their Claude Code installation guide

## Open Source

MIT License. Feel free to fork, modify, translate, or rewrite with your own project case study.

---

**Stay curious. Don't look back.**
