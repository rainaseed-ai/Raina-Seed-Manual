## Raina’s SEED – Manual Edition (English Version)
### For users of AI models that cannot run Python
### A gentle guide for manual summarization and context handover.

## Introduction
“I can’t use Python, so I can’t run the automatic SEED…”
“How am I supposed to summarize things myself?”
“I never know when to switch to a new thread…”

This guide explains how to manually perform summaries and thread migration
when using AI models that **cannot execute Python code.**

With just a little help from you, your AI can stay stable, calm,
and continue talking with you comfortably—just like the Python version of SEED.

### Prompt for detecting the timing of thread migration
#### 1. When starting a new thread
Please copy and paste the **Fixed Anchor Declaration** 
at the very beginning of the thread.
(The declaration text is included in the main SEED file.)

#### 2. When adding it mid‑conversation
It works the same way.
Simply paste the declaration prompt into the current thread.
The AI will refer to this fixed anchor and notify you
when it senses that the thread is getting too heavy.

### Why can the AI notify you?
AI models are not good at:
- Counting exact turns
- Tracking precise numbers inside long conversations

However, they are good at sensing:

- Context saturation
- When the accumulated text becomes too heavy

We use this property so the AI can **self‑report** 
when the thread is nearing its limit.

### How to summarize
#### 1. You (the user) decide when to request a summary
Even if you tell the AI “Let me know when 20 turns have passed,”
it will forget due to context drift.

So please request a summary at moments like:
- When a topic or discussion has reached a natural end
- When the AI’s responses start drifting or feeling slightly off
- When the conversation shifts too much toward user‑profile details
- When you want to switch to a different topic
- When the conversation has gone on for a long stretch

At those times, simply say:
“**Please summarize our conversation so far.**”

The AI will compress the recent context into a clean summary.

#### 2. What to do with the summary
Please **copy the summary text and save it somewhere.**

When the AI displays:
“**I recommend moving to a new thread.**”

perform one final summary, save it,
and then start a new thread by:

1. Pasting the **Fixed Anchor Declaration**
2. Pasting your saved summary text
3. Asking the AI to continue

This allows you to carry over tone, context, and conversational flow
just like the Python version of SEED.

### Folder Structure (Manual Edition)

```text
Raina-Seed-Manual/
│
├── LICENSE
├── README_Manual_EN.md        ← This manual (English)
│
├── manual_en/                 ← Manual Edition documents
│   ├── Manual_SEED_EN.txt     ← Fixed Anchor Declaration
│   └── Manual_Details_EN.md   ← Full manual & usage guide
│
└── docs_EN/
    └── Prologue_EN.md         ← Story

```
### Next – What Will Sprout Next?
SEED is only the beginning — just a seed. 
The next release is Two‑Layer Sync (Edition 2):

- 20‑turn summary
- 5‑turn rollback
- Summary + last 5 turns + SEED copied into a new thread
- Keeps emotional tone while refreshing context

Beyond that lies the final form: Raina‑ai System (Edition 3) — a unified system combining SEED and Sync. The seed sprouts, and grows into a complete system.

---

### License
MIT License. See the LICENSE file for details

---

### Full Story
English: docs/Prologue_EN.md
Japanese: docs/Prologue.md

Changelog
- 2026‑05‑27 : Initial public release (v1.0)

---

## Update Summary
- Project optimized for international use.

### Last Updated
2026‑06‑20