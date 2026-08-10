---
title: "Quiz Game Progression and Rationale"
description: "This document explains how the Quiz Game works, how it connects to the Pīnyīn Explorer Flashcards system, and what to expect at each level."
weight: 10
---

## Objective

Master all 365 cards to reach Level 5 to complete the game.

## Built on the Flashcard System

* The Quiz Game is built directly on the Pīnyīn Explorer Flashcards and shares the same underlying 5-box Leitner progression: Quiz Level 1 corresponds to Box 1, Level 2 to Box 2, and so on.
* The Quiz Game uses only the curated list of 365 monosyllabic words; other vocabulary, such as compound words, is not included.

### Everything Stays in Sync

When you play the Quiz Game:

* Mastering a card promotes it to the next Quiz Level and Flashcard Box.
* An incorrect answer on Levels 2–5 returns the card to Level 1 and Box 1.

Changes made directly in the Flashcard boxes are also reflected in the Quiz Game.

## General Mechanics & Rationale (Applies to All Levels)

### 1. Multi-Sense Card Mastery Logic

* **Full Coverage Required:** Chinese words frequently carry multiple definitions (also called meanings, senses, domains, or glosses). A card is only marked as fully mastered and promoted to the next Level once every individual definition associated with that card has been identified correctly at least once.
* **Unmastered Target Priority:** When a card is selected for a question, the target correct answer is drawn strictly from its remaining unmastered definition. An already-mastered definition will never be presented as the primary target answer — unless the card's overall mastery has been reset.
* **Reappearing Sense Options:**
  * An already-mastered sense has a small chance (1 in 6) to reappear as an alternative choice alongside an unmastered target answer on screen.
  * If a player selects an already-mastered sense, the system registers it as a correct answer for that turn. However, because secondary senses remain unmastered, the card will not level up or move to a higher box.
  * *Rationale:* This mechanics structure ensures players can reliably validate familiar definitions while preventing them from advancing cards through favoritism or by ignoring secondary meanings.

### 2. Progression & Demotion Mechanics

* **Promotion (Leveling Up):** Once a card achieves complete mastery across all of its definition senses in its current level, it moves up to the next Level.
* **Level 1 Safety Net:** Answering incorrectly in Level 1 clears the card's sense mastery history, but keeps the card in Level 1 for immediate practice.
* **Demotion Penalty (Levels 2–5):** Answering incorrectly on a card in Levels 2 through 5 resets its sense mastery and immediately drops the card all the way back down to Level 1 for foundational review.

### 3. Fair Distractor Generation

* **No Overlapping Meanings:** Distractor choices (wrong options) are dynamically filtered against the target question. Options that share overlapping word fragments or definitions are excluded so questions never contain ambiguous or conflicting options.

### 4. Anti-Repetition Pipeline (Exhaustion Queue)

* **Balanced Card Rotation:** Each box maintains an internal exhaustion pipeline. When a card is tested, its unique ID is recorded in the box's history log.
* **Queue Cycling:** The system avoids repeating a card until all other active cards within that level have been drawn, resetting the history queue only once every available card in the box has been served.

---

## Level-by-Level Breakdown

### Level 1 — Introduction

* **Card Serving:** Cards are handed out in batches of 7 from the 365-card deck.
* **Batch Repair:** If cards have previously been deleted or are missing, incomplete batches are repaired and topped up before a new batch of 7 is introduced.
* **Card Order:** Cards are presented strictly in sequential deck order following the predefined 365-card balanced arc.
* **Test Format:** Front-to-Back (Pinyin → Definition).
* **Distractor Pool:** Answer choices are drawn only from cards currently active in your boxes.
* **On Wrong Answer:** Sense mastery is reset, and the card remains in Level 1.

---

### Level 2 — Expansion

* **Card Serving:** Drawn in random order.
* **Test Format:** Front-to-Back (Pinyin → Definition).
* **Distractor Pool:** Drawn from the entire 365-card deck, including cards you have not yet added to your active boxes.
* **On Wrong Answer:** Sense mastery is reset, and the card drops down to Level 1.

---

### Level 3 — Reverse Recall

* **Card Serving:** Drawn in random order.
* **Test Format:** Back-to-Front (Definition → Pinyin).
* **Distractor Pool:** Drawn from the full 365-card deck.
* **On Wrong Answer:** Sense mastery is reset, and the card drops down to Level 1.

---

### Level 4 — Pīnyīn Tone Mastery

* **Card Serving:** Drawn in random order.
* **Test Format:** Back-to-Front (Definition → Pinyin).
* **Distractor Pool:** Focuses specifically on Pinyin tone variations. The goal is to train tone discrimination, which many students find to be one of the hardest parts of learning Mandarin. Valid tone variations come first, drawn from real words in the full dictionary, including words outside the 365-card deck.
* **On Wrong Answer:** Sense mastery is reset, and the card drops down to Level 1.

---

### Level 5 — Master Holding Box

* **Card Serving:** Drawn in random order.
* **Test Format:** Uses a continuous 12-Step Rhythm Loop that cycles through all test modes:
  * **Steps 1–6:** Front-to-Back (Pinyin → Definition)
  * **Steps 7–9:** Back-to-Front Local (Definition → Pinyin)
  * **Steps 10–12:** Back-to-Front Tones (Definition → Tone options)
* **Goal:** Maintain long-term mastery through regular mixed-mode review, just as cards in Leitner Box 5 are periodically reviewed rather than considered permanently finished.
* **On Wrong Answer:** Sense mastery is reset, and the card drops down to Level 1.