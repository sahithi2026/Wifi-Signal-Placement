# 📡 WiFi Signal Placement System

A project that demonstrates the use of **Greedy** and **Dynamic Programming (DP)** algorithms to optimally place WiFi routers in a building floor grid with obstacles (walls).

---

## 👥 Team Members
- B.Harshitha
- D.Sahithi
- S.Humaira Tasneem
- R.Monika
- K.Anushika

---

## 🎯 Problem Statement
Given an N×N grid where some cells are walls (obstacles), place the **minimum number of WiFi routers** so that every open cell is covered within a given signal radius R.

This is a real-world optimization problem — similar to placing cell towers, security cameras, or streetlights efficiently.

---

## 🧠 Algorithms Used

### ⚡ Greedy Algorithm
- At each step, scan the entire grid
- Place a router at the uncovered cell that covers the **maximum number of uncovered neighbors**
- Repeat until all open cells are covered
- **Fast** but may not always find the globally optimal solution
- Time Complexity: **O(N⁴)** | Space Complexity: **O(N²)**

### 🧠 Dynamic Programming (DP)
- Use **flood-fill (BFS)** to detect disconnected regions separated by walls
- Treat each region as an **independent sub-problem**
- Solve each sub-problem by finding minimum routers needed
- More **optimal** than Greedy, especially with wall obstacles
- Time Complexity: **O(N⁴)** | Space Complexity: **O(N²)**

---

## 🖥️ Features
- Interactive grid — draw walls by clicking/dragging
- Adjustable grid size (8×8 up to 15×15)
- Adjustable signal radius (1 to 5 cells)
- Visual comparison between Greedy and DP
- Shows router count and coverage percentage
- Works on mobile and desktop

---

## 🚀 How to Use
1. Open the live demo link below
2. Draw walls on the grid to simulate room obstacles
3. Click **"⚡ Greedy"** to run the Greedy algorithm
4. Click **"🧠 DP Placement"** to run the DP algorithm
5. Compare the number of routers placed by each algorithm

---

## 🌐 Live Demo
👉 [Click here to open the project] Hosted by team member (https://humaira-tasneem.github.io/wifi-signal-placement)

---

## 🛠️ Tech Stack
- HTML5
- CSS3
- JavaScript (Vanilla)
- Canvas API for grid rendering
- No external libraries needed

---

## 📊 Algorithm Comparison

| Feature | Greedy | Dynamic Programming |
|---|---|---|
| Speed | Fast | Slightly slower |
| Optimality | Local optimum | Better optimality |
| Wall handling | Basic | Region-aware |
| Best for | Simple grids | Complex layouts |

---

## 📅 Submission
- **Course:** CCC Algorithm Project
- **Deadline:** April 30, 2026
- **Status:** ✅ Completed
