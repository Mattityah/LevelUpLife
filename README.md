# LevelUp Life

> *What gets tracked, evolves.*

---

I built this for myself.

Not as a portfolio piece. Not to ship a product.
As a response to a real problem I was living — the absence of a mirror that reflects who you're actually becoming, day by day.

Real life has poor feedback architecture. Progress is invisible. Loops are long. The things that truly matter — the consistency, the inner work, the small daily choices — leave no visible trace. Meanwhile, everything designed to capture your attention rewards you instantly, superficially, endlessly.

LevelUp Life is my answer to that.

---

## What it is

A personal development app built around one idea: **make your growth visible to yourself.**

Not a productivity tool. Not a habit tracker. Not a to-do list.

A mirror. A map. A living record of who you're choosing to be.

It applies the feedback mechanics of video games — XP, levels, streaks, neural node evolution — to the things that actually move the needle in a human life: presence, self-knowledge, physical care, relationships, skill-building, meaningful work.

The character you build inside the app is a reflection of the character you're building in the real world.

---

## Why I built it

I'm self-taught. Reflexive by nature. Obsessed with understanding how growth actually happens — not in theory, but in the texture of a real day.

I wanted to replace the apps I was using for the wrong reasons. The ones designed to exploit attention rather than cultivate it. I wanted something that felt like a companion to the version of me that's trying — not an audience for a performance.

I wanted a place to log what I did, notice what I'm avoiding, break big goals into understandable steps, and see — actually see — the shape of my days over time.

So I built it.

---

## Core philosophy

**Presence over performance.**
This app isn't for showing progress to anyone. It's for witnessing your own.

**Process over results.**
The feed shows what you did, not what you achieved. The neural map grows from repetition, not from milestones.

**Substitution over restriction.**
The goal isn't to eliminate what doesn't serve you through willpower. It's to replace it with something that actually resonates — something gamified enough to be engaging, honest enough to be real.

**Self-knowledge as foundation.**
Gratitude logs, daily notes, bitácora entries with timestamps. The app accumulates a record of your inner life. Over time, patterns emerge. You start to see yourself.

---

## Features

### The experience
- **Card stack** — your life in swipeable cards. No menus, no friction. Your favorite category front and center.
- **Contextual greeting** — morning / afternoon / night / *are you up late?* — with your name and a rotating phrase
- **Neural network** — a D3.js visualization where your tasks exist as living nodes. Pending → forming → active → myelinated. The map grows as you do.
- **Bitácora** — a timestamped journal. Multiline, freeform, organized by day. A letter to your future self.
- **Habit tracker** — daily, specific days, or X times per week. Weekly strip, 14-day contribution grid, streak per habit.
- **AI Planner** — describe a task, answer a few questions, get a step-by-step plan built around your actual availability.

### The system
- 5 life categories: Mind, Body, Skills, Relationships, Work — fully customizable
- XP + leveling system with titled progression
- Daily streaks with best-streak tracking
- Full Firebase sync — real-time across all your devices
- Google Auth — one tap, no passwords
- PWA — installable on iOS and Android

---

## Stack

| Layer | Tech |
|-------|------|
| Frontend | HTML + CSS + Vanilla JS |
| Visualization | D3.js — force simulation + Canvas |
| Auth | Firebase Auth (Google Sign-In) |
| Database | Firebase Firestore (realtime sync) |
| Fonts | Geist 300/400/500 + Instrument Serif |
| Hosting | GitHub Pages |

No frameworks. No build steps. One file.

---

## Try it

**[mattityah.github.io/LevelUpLife](https://mattityah.github.io/LevelUpLife)**

Sign in with Google. Create your first tasks. Complete them. Watch your character grow.

---

## Roadmap

**Phase 2 — Community**
A social feed where users share process, not results. The neural map as proof-of-work. Built on real backend (PHP + MySQL).

**Phase 3 — Ecosystem**
Integration with fitness trackers, language apps, meditation platforms — all feeding into one identity map. AI suggestions based on your actual activity history.

---

## Author

Built by **Mattia** — self-taught, from scratch, with intention.

*2025*

---

*The best version of you already exists. This app helps you find the path there — one logged day at a time.*
