# Wild West Flip (Browser-Based Card Strategy Game)

This repository contains a standalone HTML/JS implementation of **Fliptown**, downsized and simplified. **Fliptown** is a flip and write game made by Steven Aramini and published by Write Stuff Games, check out the game kickstarter [here](https://www.kickstarter.com/projects/writestuffgames/fliptown). This adaptation is called **Wild West Flip**.

The project includes:

* Simplified game logic implemented in vanilla JavaScript
* Dynamic UI rendering for the board, trackers, mine, poker dashboard, and final scoring
* Animated robbery checks and sheriff arrest evaluation
* Automatic end-of-game resolution
* Fully self-contained HTML file that can be hosted anywhere

---

## 🎮 Game Overview

This simplified adaptation version of **Fliptown** recreates the core mechanics of the flip and write game:

* Draw 3 cards each turn
* Select one as your **poker card** (builds a 5‑card final hand)
* Use the values/suits of the other two cards to perform map actions:

  * **♠ Robbery** — Risk-based checks with rewards on success
  * **♥ Trail** — Select trail nodes with rewards
  * **♣ Town** — Straightforward marking
  * **♦ Mine** — Explore branching mine chambers and earn tools
  * **💀 Grave** — Emergency action with penalties

After all 5 poker cards are chosen, the game ends with:

1. **Revealing the hidden card** (set aside at the start)
2. **Sheriff Arrest Check** (dice roll vs hidden card value)
3. **Score Calculation** (formal scoring sheet included in UI)

---

## 📁 Files Included

* `index.html` — Main HTML file containing **all game code** (HTML, CSS, JS)

---

## 🧩 Key Features

### ✔ Full Game Flow

* Turn handling
* Bonus action resolution
* Resource tracking (Money, Gold, Stars, Wanted)
* Tools and mine progression

### ✔ Auto End‑Game

Once 5 poker cards are saved:

* Hidden card is revealed
* Sheriff roll plays automatically
* Score summary is shown

### ✔ Fixes Applied

This version includes important fixes:

* Hidden card now correctly reveals at the end
* Sheriff comparison triggers every time
* Missing DOM elements added (`pokerRewardText`, `scoreSection`)
* End‑game flow made fully automatic

---

## ▶️ How to Run

No build tools required.

### **Just open the HTML file in any browser:**

```
./index.html
```

---

## 🛠 Development Notes

### Structure

The script is fully self-contained:

* **CSS:** Inline `<style>`
* **JavaScript:** Inline `<script>` (no modules or imports)

### No Dependencies

This page uses **zero external libraries** — no jQuery, no frameworks.
Everything is built with vanilla DOM manipulation and dynamic rendering.

---

## 📌 Roadmap (Optional Enhancements)

Potential improvements for future versions:

* update the town (clubs) action
* sheriff arrest is not based on a dice roll, but the wanted level
* daily deck of card configuration, so user can compare their score
