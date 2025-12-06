# Course Notes: Topological Sorting

<iframe width="560" height="315" src="https://www.youtube.com/embed/VHyN-8L6kPw?si=KkNk-KwaWUg5OmQr" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>


## Introduction

**Topological Sorting** is a way to line up tasks or events in the correct order when some tasks depend on others.  

> Imagine planning a project, cooking a complicated recipe, or deciding which classes to take first. Topological sorting helps you figure out what needs to come before what.  

In computer science, it is used to work with **directed graphs** and ensures all dependencies are respected. It's a handy tool whenever tasks must happen in a specific sequence.

---

## Real-World Example

- Have you ever followed a recipe where some steps must happen before others?  
  - Example: You must boil pasta before mixing it with sauce.
- This concept of **dependency** is key to understanding topological sorting.

---

## Outline

In this lesson, we will cover:

1. What topological sorting is.
2. How it works with a simple example.
3. Why it is useful in computer science and everyday life.

---

## Key Concepts

Before diving in, we need to understand:

- **Graphs:** Collections of nodes and arrows (edges).  
- **Dependencies:** The idea that one task must happen before another.

---

## Formal Definition

A **topological sort** is a **linear ordering of nodes in a directed acyclic graph (DAG)** such that for every arrow from node `U` to node `V`, `U` appears before `V` in the ordering.  

- **Simpler terms:** If one task depends on another, the dependent task must come later in the list.  
- **Important:** Topological sorting only works on **acyclic graphs**.  
  - Cycles like `Task A → Task B → Task A` make ordering impossible.

---

## How It Works: Step-by-Step Example

Suppose we have a DAG with 5 nodes and links between them:

1. **Find a node with no dependencies** → Node `A`.  
   - Place `A` at the beginning and remove its links.
2. **Repeat the process**:  
   - Next node with no dependencies → Node `B`.  
   - Place `B` after `A` and remove its links.
3. **Continue** until all nodes are placed.  

✅ Done! We have completed a topological sort.

---

## Applications of Topological Sorting

Topological sorting is widely used wherever tasks have dependencies:

- **Course scheduling** – deciding the order of classes.
- **Project planning** – organizing tasks based on prerequisites.
- **Software development** – building modules in the correct sequence.
- **Social networks & recommendation systems** – managing order of actions.
- **Everyday activities** – cooking or assembling furniture.

Understanding topological sorting helps to organize complex systems safely and efficiently.

---

## Summary

- Orders tasks with dependencies.
- Works only on **directed acyclic graphs (DAGs)**.
- Appears in **course scheduling, project planning, software development**, and more.
- Multiple valid solutions exist as long as all dependencies are respected.

> Topological sorting is not just theoretical—it’s something we use every day without realizing it.

---

## Questions

Feel free to ask questions about:

- How topological sorting works.
- Different ways to implement it.
- Applications in real-life and computer science.

