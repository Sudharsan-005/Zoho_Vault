---
title: "Player Progress Dashboard"
type: dashboard
tags:
  - zoho/dashboard
---

# 🚀 Zoho Placement Training - Player Dashboard

Welcome to your central tracking hub for **Zoho Placement Preparation**. Use this dashboard to monitor solved questions, track weak topics, and prepare effectively for Round 2 and Round 3.

---

## 📊 Overall Progress Summary

| Metric | Target | Current Count | Status |
| :--- | :---: | :---: | :---: |
| **Round 2 Questions (C / DSA)** | 50 | 0 | 🟡 In Progress |
| **Round 3 Questions (App Dev / System Design)** | 20 | 0 | 🟡 In Progress |
| **Total Questions Solved** | 70 | 0 | 🔴 Not Started |

---

## 📂 Quick Access Navigation

- 📄 **[[Instructions]]** — Read workflow & usage guide
- 📝 **[[Question_Template]]** — Template for creating new questions
- 💡 **[[Solution_Template]]** — Template for writing solutions
- 📁 **[[Round_2_Questions/]]** — Browse Round 2 Question files
- 📁 **[[Round_2_Solutions/]]** — Browse Round 2 Solution files
- 📁 **[[Round_3_Questions/]]** — Browse Round 3 Question files
- 📁 **[[Round_3_Solutions/]]** — Browse Round 3 Solution files

---

## 🧩 Round 2: Core Coding & Data Structures

> **Focus Areas:** Arrays, Strings, Matrices, Pointers, Recursion, Bit Manipulation, Linked Lists, Stacks & Queues.

| # | Question Title | Topic | Difficulty | Question Link | Solution Link | Status |
| :-: | :--- | :--- | :---: | :---: | :---: | :---: |
| 1 | *Sample: Array Rotation* | Arrays | Medium | [[Round_2_Questions/Sample_Array_Rotation\|Question]] | [[Round_2_Solutions/Solution_Sample_Array_Rotation\|Solution]] | 🟡 In Progress |
| 2 | | | | | | |
| 3 | | | | | | |
| 4 | | | | | | |
| 5 | | | | | | |

---

## 🏗️ Round 3: Advanced Coding & Application Development

> **Focus Areas:** Complex Problem Solving, Console Applications (e.g., Railway Reservation, ATM, Snake Game, Shopping Cart), Object-Oriented Design.

| # | Application / Scenario | Domain | Complexity | Question Link | Solution Link | Status |
| :-: | :--- | :--- | :---: | :---: | :---: | :---: |
| 1 | *Sample: Railway Reservation System* | OOP / App Dev | Hard | [[Round_3_Questions/Sample_Railway_System\|Question]] | [[Round_3_Solutions/Solution_Sample_Railway_System\|Solution]] | 🟡 In Progress |
| 2 | | | | | | |
| 3 | | | | | | |

---

## ⚡ Automated Dataview Scanners (Obsidian Plugin)

> [!NOTE]
> If you have the **Dataview** plugin enabled in Obsidian, the queries below will automatically scan and list all questions in your vault!

### All Round 2 Unsolved Questions
```dataview
TABLE category, difficulty, status, target_date
FROM "Round_2_Questions"
WHERE status != "Solved"
SORT priority DESC
```

### Completed Solutions Log
```dataview
TABLE language, time_complexity, space_complexity, date_solved
FROM "Round_2_Solutions" OR "Round_3_Solutions"
WHERE status = "Accepted" OR status = "Optimized"
SORT date_solved DESC
```
