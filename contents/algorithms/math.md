---
id: math
title: Math
toc_max_heading_level: 2
---

## Introduction

Math is a foundational aspect of Computer Science and every programmer and computer scientist needs to have basic mathematical knowledge. Thankfully, for the purpose of coding interviews, there usually won't be that much math involved, but some basic math techniques is helpful to know as you may be asked to implement mathematical operations.

## Things to look out for during interviews

- If code involves division or modulo, remember to check for division or modulo by 0 case.
- Check for and handle overflow/underflow if you are using a typed language like Java and C++. At the very least, mention that overflow/underflow is possible and ask whether you need to handle it.
- Consider negative numbers and floating point numbers. This may sound obvious, but under interview pressure, many obvious cases go unnoticed.

## Common formulas

|  | Formula |
| --- | --- |
| Check if a number is even | `num % 2 == 0` |
| Sum of 1 to N | 1 + 2 + ... + (N - 1) + N = (N+1) \* N/2 |
| Sum of Geometric Progression | 2<sup>0</sup> + 2<sup>1</sup> + 2<sup>2</sup> + 2<sup>3</sup> + ... 2<sup>n</sup> = 2<sup>n+1</sup> - 1 |
| Permutations of N | N! / (N-K)! |
| Combinations of N | N! / (K! \* (N-K)!) |

## Techniques

### Multiples of a number

When a question involves "whether a number is a multiple of X", the modulo operator would be useful.

### Comparing floats

When dealing with floating point numbers, take note of rounding mistakes. Consider using epsilon comparisons instead of equality checks. E.g. `abs(x - y) <= 10e7` instead of `x == y`.

### Fast operators

If the question asks you to implement an operator such as power, square root or division and want it to be faster than O(n), some sort of doubling (fast exponentiation) or halving (binary search) is usually the approach to go. Examples: [Pow(x, n)](https://leetcode.com/problems/powx-n/), [Sqrt(x)](https://leetcode.com/problems/sqrtx/)

## Corner cases

- Division by 0
- Multiplication by 1
- Negative numbers
- Floats

## Recommended questions

- [Pow(x, n)](https://leetcode.com/problems/powx-n/)
- [Sqrt(x)](https://leetcode.com/problems/sqrtx/)
- [Integer to English Words](https://leetcode.com/problems/integer-to-english-words/)

## Recommended courses

import AlgorithmCourses from '../\_courses/AlgorithmCourses.md'

<AlgorithmCourses />
