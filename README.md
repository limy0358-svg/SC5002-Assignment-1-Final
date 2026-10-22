# SC5002 Artificial Intelligence Fundamentals & Applications 
## Lab Assignment Report & Implementation

**Student Name:** Lim Yu Hng 

**Matriculation ID:** U2520459A 

**Course:** SC5002 - Artificial Intelligence Fundamentals & Applications 

**Submission Date:** October 2026 

--- 

📌 Project Overview 

This repository contains the completed Google Colab notebook and documentation for the SC5002 Lab Assignment. 

The project covers two primary areas: 
1. **Part 1: Classical Search & Problem Solving**: Evaluating Breadth-First Search (BFS) and A* Search on a directed state graph, and solving the 8-Puzzle problem using depth g(n) and misplaced tiles heuristic h(n).
2. **Part 2: Applied Machine Learning with AI Copilot**: Implementing Linear and Ridge Regression models on the California Housing dataset using 5-Fold Cross-Validation and analyzing regularized alpha tuning (α = 0.1, 10, 1000).

### Part 1: Classical Search Algorithms

* **Task 1.1 (Graph Search)**:
  * Breadth-First Search (BFS) Path: `S -> F -> G` (Total Cost = 9)
  * A\* Search Path: `S -> B -> D -> G` (Optimal Cost = 7)
* **Task 1.2 (8-Puzzle Problem)**:
  * Reached goal state `[1 2 3 | 8 _ 4 | 7 6 5]` in **5 optimal moves** (f(n) = 5).

### Part 2: Machine Learning Model Performance

Evaluated using 5-Fold Cross-Validation R² scores on 1,000 sampled California Housing records:

| Model                 | Regularization Penalty (α) | Mean 5-Fold R² Score | Key Finding                                  |
| --------------------- | -------------------------- | -------------------- | -------------------------------------------- |
| **Linear Regression** | N/A                        | **0.5872**           | Unconstrained baseline fit                   |
| **Ridge Regression**  | α = 0.1                    | **0.5872**           | Minimal penalty constraint                   |
| **Ridge Regression**  | α = 10.0                   | **0.5865**           | Balanced fit; shrinks large weights          |
| **Ridge Regression**  | α = 1000.0                 | **0.3541**           | Severe underfitting due to over-penalization |


