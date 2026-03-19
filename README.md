# AI_LAB_ASSIGNMENT-3_SE24UCSE035
CODES FOR THE AI ASSIGNMENT 3
# 🚀 AI Assignment: Search Algorithms & UGV Path Planning

## 📌 Overview

This project implements and analyzes three important AI search problems:

1. **Dijkstra’s Algorithm (Uniform Cost Search)** for Indian cities
2. **UGV Navigation in Static Obstacle Grid**
3. **UGV Navigation in Dynamic Obstacle Environment**

Each part demonstrates how intelligent agents find optimal paths under different conditions.

---

# 🔷 1. Dijkstra’s Algorithm (India Road Network)

## 🧩 Description

Dijkstra’s Algorithm is used to find the **shortest path from a source city to all other cities** in a weighted graph where edge costs represent road distances.

## ⚙️ Approach

* Graph represented using **adjacency matrix**
* Each node represents a **city**
* Edge weights represent **road distances**
* Select node with **minimum distance repeatedly**

## 🧠 Key Idea

Uniform Cost Search expands the **lowest cost node first**, ensuring optimal paths.

## ▶️ Output

* Minimum distance from source city to all other cities

## 📍 Applications

* GPS navigation systems
* Transport optimization
* Network routing

---

# 🔷 2. UGV Navigation (Static Obstacles)

## 🧩 Description

An Unmanned Ground Vehicle (UGV) must navigate a **grid (e.g., 70x70 km)** avoiding known obstacles to reach a goal using the shortest path.

## ⚙️ Approach

* Grid representation:

  * `0` → Free cell
  * `1` → Obstacle
* Algorithm used: **Breadth-First Search (BFS)**
* Movement allowed in 4 directions:

  * Up, Down, Left, Right

## 🧠 Key Idea

Since all moves have equal cost, BFS guarantees the **shortest path**.

## 🎯 Features

* Obstacle density can be:

  * Low
  * Medium
  * High (random generation)

## 📊 Measures of Effectiveness (MoE)

* Path length
* Time taken
* Nodes explored
* Success rate

## 📍 Applications

* Military ground robots
* Warehouse automation
* Autonomous vehicles

---

# 🔷 3. UGV Navigation (Dynamic Obstacles)

## 🧩 Description

In real-world environments, obstacles are **not static** and may appear unexpectedly. The UGV must adapt and still reach the goal optimally.

## ⚙️ Approach

* Use **A* Algorithm**
* Combine:

  * `g(n)` → Cost from start
  * `h(n)` → Heuristic (Manhattan distance)
* When obstacle appears:

  1. Update environment
  2. Recalculate path

## 🧠 Key Idea

A* improves efficiency using heuristics and supports **dynamic replanning**.

## 🔁 Advanced Method

* **D* Algorithm**

  * Incremental replanning
  * Used in real-world robotics (e.g., Mars rovers)

## 📊 Measures of Effectiveness (MoE)

* Replanning time
* Adaptability
* Path optimality
* Collision avoidance

## 📍 Applications

* Military battlefield robots
* Self-driving vehicles
* Rescue robots

---

# 🏁 Conclusion

* **Dijkstra’s Algorithm** is ideal for known, weighted graphs
* **BFS** works efficiently for uniform-cost grid navigation
* **A*/D*** are essential for dynamic and real-time environments

These algorithms form the foundation of **intelligent path planning systems** in AI and robotics.

---

# 📚 References

* Artificial Intelligence: A Modern Approach – Russell & Norvig
* Open-source map datasets (for city distances)
* Robotics path planning research papers

---
