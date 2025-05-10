# Day11-50-days-coding-challenge
# 🚀 Day 11 – 50 Days of Coding Challenge

## ✅ Problems Solved

### 1. Trailing Zeroes in Factorial
- **Problem Statement:**  
  Given an integer `n`, return the number of trailing zeroes in `n!`.
- **Examples:**  
  - Input: `n = 3` → Output: `0`  
  - Input: `n = 5` → Output: `1`  
  - Input: `n = 0` → Output: `0`
- **Insight:**  
  Trailing zeroes in `n!` are produced by the number of times **5** is a factor in the numbers from 1 to `n`.  
  For each 5, 25, 125... divide `n` by powers of 5 and add the result.
- **Formula:**  
  ```cpp
  while (n > 0) {
      n /= 5;
      count += n;
  }
Time Complexity: O(log₅ n)

Space Complexity: O(1)

2. Remove N-th Node From End of List
Problem Statement:
Given a linked list, remove the n-th node from the end in one pass and return the head.

Examples:

Input: [1,2,3,4,5], n = 2 → Output: [1,2,3,5]

Input: [1], n = 1 → Output: []

Input: [1,2], n = 1 → Output: [1]

Approach:

Use a dummy node to handle edge cases.

Move a fast pointer n+1 steps ahead.

Move both fast and slow pointers until fast reaches the end.

Remove the node after slow.

Time Complexity: O(n)

Space Complexity: O(1)

🔍 Concepts Practiced
Factorial-based mathematical patterns

Power counting using integer division

Linked list node removal using two-pointer technique

Edge case handling (head removal)

💻 Tools & Language
Language: C++

IDE: VS Code

Version Control: Git & GitHub

