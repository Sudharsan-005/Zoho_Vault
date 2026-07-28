---
title: "Obsidian Vault Multi-Player User Guide"
type: guide
tags:
  - zoho/instructions
---

# 📖 Zoho Placement Vault — Multi-Player Guide & Instructions

 This vault is designed for **multiple players** to solve questions independently, maintain separate tracking dashboards, compare progress on a central leaderboard, and cross-link solution notes.

---

## 📁 Vault Structure Overview

```text

├── Round_2_Questions/                  # Shared Question bank 
├── Round_2_Solutions/                  # Solutions tagged by player (e.g. Solution_ArrayRotation_Sudharsan.md)
├── Round_3_Questions/                  # Shared Question bank LLD
├── Round_3_Solutions/                  # Solutions tagged by player (e.g. Solution_RailwaySystem_Sudharsan.md)
├── Templates/
│   ├── Question_Template.md           # Template for new shared questions
│   ├── Solution_Template.md           # Template for solutions (includes `solved_by`)
│   └── Player_Dashboard_Template.md   # Template to create a new player dashboard
├── Instructions.md                    # This guide
└── Plan for Implenetation.md          # Original planning outline
```

---

## 👥 Multi-Player Workflow

### 1. Setting Up a New Player Dashboard
When a new person joins the preparation group:
1. Go to `Templates/Player_Dashboard_Template.md`.
2. Copy the file (or use Obsidian's Template plugin) to create `Dashboards/Player_<Name>_Dashboard.md` (e.g., `Dashboards/Player_Rahul_Dashboard.md`).
3. Replace `{{player_name}}` with the person's name.
4. Add a row for the new player in **`Dashboards/Master_Dashboard.md`** under the **Players Directory & Leaderboard** table.

---

### 2. Adding a Shared Question
1. Create a note in `Round_2_Questions/` or `Round_3_Questions/` (e.g., `Two_Sum.md`).
2. Use **`Templates/Question_Template.md`**.
3. Under `## 👥 Solutions by Players`, list links for each player's potential solution:
   ```markdown
   - **Sudharsan:** [[Round_2_Solutions/Solution_Two_Sum_Sudharsan|Sudharsan's Solution]]
   - **Rahul:** [[Round_2_Solutions/Solution_Two_Sum_Rahul|Rahul's Solution]]
   ```

---

### 3. Solving a Question (For Any Player)
1. When **Sudharsan** solves `Two_Sum`, create `Round_2_Solutions/Solution_Two_Sum_Sudharsan.md`.
2. Apply **`Templates/Solution_Template.md`**.
3. Set the frontmatter fields:
   ```yaml
   question: "[[Two_Sum]]"
   solved_by: "Sudharsan"
   language: Java
   status: Accepted
   ```
4. Link back to your own dashboard: `[[Dashboards/Player_Sudharsan_Dashboard]]`.
5. Open your personal dashboard (`Player_Sudharsan_Dashboard.md`) and update your solution link and status (`Solved` / `Accepted`).

---

### 4. Tracking & Leaderboard Comparison
- **Personal Tracking:** Each player updates their own `Player_<Name>_Dashboard.md`.
- **Global Overview:** Open **`Dashboards/Master_Dashboard.md`** to view all registered players, compare solved counts, and navigate directly to any player's solutions.

---

## 💡 Recommended Obsidian Setup
1. **Enable Templates Plugin:**
   - `Settings` -> `Core Plugins` -> Enable `Templates`.
   - Set template folder to `Templates`.
2. **Dataview Plugin (Optional but recommended):**
   - Install `Dataview` community plugin to automatically populate solutions based on `solved_by = "Name"`.
