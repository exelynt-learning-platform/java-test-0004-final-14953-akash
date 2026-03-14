# java-test-0004-final-14953-akash
Final Project Assignment - This repository contains the complete final project code and documentation.

## Problem Statement

This assessment evaluates the candidate’s understanding of **matrix-style pattern generation and layered number logic using Java loops**.

The objective is to develop a Java program that prints a **concentric number square pattern**. The solution should demonstrate proper use of nested loops, logical number placement, and structured output formatting.

---

# Approach

1. **Define the pattern size**
   - Let `n = 4`.
   - The size of the square matrix will be `2 * n - 1`.

2. **Use nested loops**
   - Outer loop controls the rows.
   - Inner loop controls the columns.

3. **Determine the layer of the current cell**
   - For each position `(i, j)`, calculate its distance from the borders:
     - `top = i`
     - `left = j`
     - `right = size - 1 - j`
     - `bottom = size - 1 - i`

4. **Find the minimum distance**
   - The smallest value among these distances determines the layer.

5. **Calculate the number to print**
   - Print `n - minDistance`.

6. **Continue for the entire matrix**
   - This produces a symmetric concentric pattern.

---

# Time Complexity

**O(n²)**

---

# Space Complexity

**O(1)**
