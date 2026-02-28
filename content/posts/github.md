+++
date = '2026-02-26T16:00:00+05:00'
title = 'Setting Up GitHub on Linux and Pushing Code'
draft = false
+++

In this post, I explain how I set up GitHub on my Linux system and pushed my code step by step.

---
# Git & GitHub: The Ultimate Beginner's Guide

## First, Understand the Problem!

Imagine this situation:

You create a website.
- **Day 1:** It works perfectly.
- **Day 2:** You change something.

Now the website breaks.
You want to go back to yesterday's version...
**But you cannot.**

---

## What is Git?

**Definition:** Git is a tool that saves your project **step by step**.
It remembers:
- **what** you changed
- **when** you changed it
- **who** changed it

**Simple Meaning:** Git = Save history of your project.

**Real Life Example:** Think about a video game. Every time you pass a level, the game saves your progress. If you lose, you restart from the last save point.
**Git works the same way.** It saves your project so you can go back anytime.

---

## What is GitHub?

**Definition:** GitHub is a website where you upload your code.

**Simple meaning:**
- **Git** = Save on your Computer
- **GitHub** = Save on Internet

---

## Why we must Learn Git?
- Because in **real jobs**
- Developers work in **teams**
- Everyone pushes code **daily**
- Companies use Git
**Without Git → No professional development.**

---

## How Git Actually Works

There are only **3 simple steps**:
1. **Add**
2. **Commit**
3. **Push**

That's it.

---

## Git Commands Summary

| Command | What it does |
|---------|-------------|
| `git init` | Start tracking your project |
| `git status` | Check what changed |
| `git add .` | Add all files to staging |
| `git commit -m "message"` | Save changes with message |
| `git push` | Upload to GitHub |

---

## Practical Guide

### 1. Install Git
Go to: [https://git-scm.com](https://git-scm.com)
Download, Install, then check:
```bash
git --version