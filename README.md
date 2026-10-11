<div align="center">

# 🧩 LeetCode Solutions in C++

**Consistency over shortcuts. Understanding over memorization.**

![Language](https://img.shields.io/badge/C%2B%2B-17-00599C?style=for-the-badge&logo=cplusplus&logoColor=white)
![Platform](https://img.shields.io/badge/Platform-LeetCode-FFA116?style=for-the-badge&logo=leetcode&logoColor=white)
![Solved](https://img.shields.io/badge/Solved-0-brightgreen?style=for-the-badge)
![Status](https://img.shields.io/badge/Status-Actively%20Practicing-blue?style=for-the-badge)

[**LeetCode Profile**](https://leetcode.com/u/mellifluentShiv/) · [**GitHub Profile**]([https://github.com/YOUR_USERNAME](https://github.com/shiv0xparanoid))

</div>

---

## 📖 About

A structured archive of my LeetCode solutions in **C++17**, organized by difficulty and then by topic. It documents my problem-solving journey, the patterns I pick up along the way, and the trade-offs behind each approach.

## 🎯 Goals

- 🧱 Strengthen data structures and algorithms fundamentals
- 🔁 Recognize recurring problem-solving patterns
- ⏱️ Sharpen time and space complexity analysis
- 🔍 Maintain a searchable archive for quick revision
- 📈 Track progress through consistent daily practice

## 🗂️ Repository Structure

```text
leetcode-cpp/
├── 🟢 Easy/
├── 🟡 Medium/
├── 🔴 Hard/
├── 🧠 Patterns/      # Reusable templates and cheat sheets
└── 📄 README.md
```

Solutions are organized by **difficulty first, topic second**, e.g. `Medium/SlidingWindow/longest-substring-without-repeating-characters.cpp`.

## 📊 Progress Tracker

| Difficulty | Solved | Progress |
|:-----------|:------:|:---------|
| 🟢 Easy    | 0 | `░░░░░░░░░░` 0% |
| 🟡 Medium  | 0 | `░░░░░░░░░░` 0% |
| 🔴 Hard    | 0 | `░░░░░░░░░░` 0% |
| **🏆 Total** | **0** | |

> *Counts are updated as solutions are added.*

## 🧠 Topics Covered

| | Topic | | Topic |
|:-:|:--|:-:|:--|
| ⬜ | Arrays & Strings | ⬜ | Trees & BSTs |
| ⬜ | Hashing | ⬜ | Graphs |
| ⬜ | Two Pointers | ⬜ | Greedy Algorithms |
| ⬜ | Sliding Window | ⬜ | Backtracking |
| ⬜ | Binary Search | ⬜ | Dynamic Programming |
| ⬜ | Linked Lists | ⬜ | Heaps & Priority Queues |
| ⬜ | Stacks & Queues | ⬜ | Bit Manipulation |

*Swap ⬜ for ✅ as each topic is covered.*

## 🔎 Pattern Cheat Sheet

| Pattern | Reach for it when... | Typical Complexity |
|:--|:--|:--|
| Two Pointers | Sorted input, pair/triplet search | O(n) |
| Sliding Window | Contiguous subarray or substring constraints | O(n) |
| Binary Search | Sorted or monotonic search space | O(log n) |
| Hash Map | Fast lookup, frequency counting, complements | O(n) |
| Monotonic Stack | Next greater/smaller element | O(n) |
| BFS / DFS | Traversal, shortest path in unweighted graphs | O(V + E) |
| Backtracking | Generate combinations, permutations, subsets | O(2ⁿ) / O(n!) |
| Dynamic Programming | Overlapping subproblems and optimal substructure | Varies |

## 💻 Solution Format

Every solution lives in a descriptively named file using the exact LeetCode function signature. For selected problems I also include a short write-up:

| Section | What it covers |
|:--|:--|
| 💡 **Approach** | The core observation and reasoning |
| ⚙️ **Complexity** | Time and auxiliary space |
| 🔑 **Key Insight** | What makes it work, or what I learned |

<details>
<summary><b>📝 Example file template</b></summary>

```cpp
/*
 * Problem : Two Sum
 * Link    : https://leetcode.com/problems/two-sum/
 * Topic   : Hashing
 *
 * Approach:
 *   Store each value's index in a hash map; for every element,
 *   check whether its complement has already been seen.
 *
 * Complexity:
 *   Time  : O(n)
 *   Space : O(n)
 *
 * Key Insight:
 *   Trade space for time by remembering what you've seen.
 */

class Solution {
public:
    vector<int> twoSum(vector<int>& nums, int target) {
        unordered_map<int, int> seen;
        for (int i = 0; i < (int)nums.size(); ++i) {
            auto it = seen.find(target - nums[i]);
            if (it != seen.end()) return {it->second, i};
            seen[nums[i]] = i;
        }
        return {};
    }
};
```

</details>

## 🛠️ Tech Stack

| | |
|:--|:--|
| **Language** | C++ |
| **Standard** | C++17 |
| **Platform** | LeetCode |

## 📌 Note

This is a personal learning and revision repository, so solutions may evolve as I discover more efficient approaches. Problem links are provided for reference; problem statements are not reproduced here.

---

<div align="center">

⭐ If this repo helps you, consider giving it a star!

*Consistency over shortcuts. Understanding over memorization.*

</div>
