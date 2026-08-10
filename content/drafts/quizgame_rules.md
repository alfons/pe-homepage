---
title: "Quiz Game Rules"
summary: "Clear rules and scoring system for the interactive pinyin quiz game."
# optional nicer description that appears under the title on the single page
description: "Official rules for the Pīnyīn Explorer quiz game"
weight: 10
---

## Part I: General Mechanics & Rationale (Applies to All Levels)

### 1. Multi-Sense Card Mastery Logic

* **Full Coverage Required:** Chinese characters and vocabulary words frequently carry multiple definition meanings (senses). A card is only marked as fully mastered and promoted to the next Level once **every individual definition sense** associated with that card has been identified correctly at least once.


* **Unmastered Target Priority:** When a card is selected for a question, the target correct answer is drawn strictly from its remaining **unmastered senses**. An already-mastered sense will **never** be presented as the primary target answer unless the card's overall mastery has been reset.


* **Reappearing Sense Options:**
* An already-mastered sense has a small chance (1 in 6) to reappear as an alternative choice alongside an unmastered target answer on screen.


* If a player selects an already-mastered sense, the system registers it as a correct answer for that turn. However, because secondary senses remain unmastered, **the card will not level up or move to a higher box**.


* *Rationale:* This mechanics structure ensures players can reliably validate familiar definitions while preventing them from advancing cards through favoritism or by ignoring secondary meanings.





### 2. Progression & Demotion Mechanics

* **Promotion (Leveling Up):** Once a card achieves complete mastery across all of its definition senses in its current level, it moves up to the next Leitner Level.


* **Level 1 Safety Net:** Answering incorrectly in Level 1 clears the card's sense mastery history, but keeps the card in Level 1 for immediate practice.


* **Demotion Penalty (Levels 2–5):** Answering incorrectly on a card in Levels 2 through 5 resets its sense mastery and immediately drops the card all the way back down to **Level 1** for foundational review.



### 3. Fair Distractor Generation

* **No Overlapping Meanings:** Distractor choices (wrong options) are dynamically filtered against the target question. Options that share overlapping word fragments or definitions are excluded so questions never contain ambiguous or conflicting options.


* **Easter Egg Blacklist:** Internal definitions (such as emoji notes or surprise definitions) are blacklisted from ever being drawn as random distractor choices for other cards.


* **Tone & Syllable Precision:** In tone-focused test modes, wrong options are tailored to match initial sound patterns or valid pinyin tone variations (tones 1–5) to test pitch precision.



### 4. Anti-Repetition Pipeline (Exhaustion Queue)

* **Balanced Card Rotation:** Each box maintains an internal exhaustion pipeline. When a card is tested, its unique ID is recorded in the box's history log.


* **Queue Cycling:** The system avoids repeating a card until all other active cards within that level have been drawn, resetting the history queue only once every available card in the box has been served.



---

## Part II: Level-by-Level Breakdown

### Level 1 (Box 1) — Introduction & Foundation

* **Batch Serving:** Cards enter the game in fixed batches of 7 from the 365-card deck.


* **Batch Repair:** If cards were previously deleted or missing, incomplete batches are repaired and topped off before a brand-new 7-card set is introduced.


* **Card Order:** Cards are presented strictly in sequential deck order following the predefined 365-card balanced arc.


* **Test Format:** **Front-to-Back** (Prompt displays Pinyin $\rightarrow$ Select the correct definition).


* **Distractor Pool:** Answer choices are drawn **only** from cards currently active in your boxes.


* **On Wrong Answer:** Sense mastery is reset, and the card remains in Level 1.



---

### Level 2 (Box 2) — Expansion & Memory

* **Card Order:** Drawn in **random order**.


* **Test Format:** **Front-to-Back** (Prompt displays Pinyin $\rightarrow$ Select the correct definition).


* **Distractor Pool:** Drawn from the **entire 365-card deck**, including cards you have not yet added to your active boxes.


* **On Wrong Answer:** Sense mastery is reset, and the card drops down to Level 1.



---

### Level 3 (Box 3) — Reverse Recall

* **Card Order:** Drawn in **random order**.


* **Test Format:** **Back-to-Front** (Prompt displays Definition $\rightarrow$ Select the correct Pinyin).


* **Distractor Pool:** Drawn from the full 365-card deck.


* **On Wrong Answer:** Sense mastery is reset, and the card drops down to Level 1.



---

### Level 4 (Box 4) — Tone Mastery

* **Card Order:** Drawn in **random order**.


* **Test Format:** **Back-to-Front Tones** (Prompt displays Definition $\rightarrow$ Select the correct tone/Pinyin variation).


* **Distractor Pool:** Focuses specifically on subtle tone variations (tones 1–5) and matching initial sound patterns drawn from the full deck to hone pitch distinction.


* **On Wrong Answer:** Sense mastery is reset, and the card drops down to Level 1.



---

### Level 5 (Box 5) — Master Tier Castle Quest

* **Card Order:** Drawn in **random order**.


* **Test Format:** Uses a continuous **12-Step Rhythm Loop** that cycles through all test modes:


* **Steps 1–6:** Front-to-Back (Pinyin $\rightarrow$ Definition)


* **Steps 7–9:** Back-to-Front Local (Definition $\rightarrow$ Pinyin)


* **Steps 10–12:** Back-to-Front Tones (Definition $\rightarrow$ Tone options)




* **Ultimate Goal:** Master all 365 cards in Level 5 to reach the castle and complete the game.


* **On Wrong Answer:** Sense mastery is reset, and the card drops down to Level 1.