---
type: lab
date: 2023-1-4T08:30:00+00:00
title: '实验 1. Bits Bytes and Integers'
tldr: "For lab1, the chosen code passages highlight interesting uses of the bitwise and integer operations."
pdf: https://h8pqt7tpdf.feishu.cn/file/boxcncfy3SbEyi7U0oSV7UYtMab
---

For lab1, the chosen code passages highlight interesting uses of the bitwise and integer operations.

## Learning Goals

During this lab you will:

- practice with bits, bitwise operators and bitmasks
- read and analyze C code that manipulates bits/ints
- further practice with the edit-compile-test-debug cycle in the Unix environment

Join in to your assigned breakout room and introduce yourselves. Together you will tackle the exercises below.

## Get Started

To get started in the lab, you must copy the starter code to your folder.
When you are at your home directory and have created a folder called cs102, you can type the following command.

```
cp -r ../cs102-shared/labs/lab1 cs102/
```

### Task 1. Bitwise Practice (25 min)

### Task 2. Round Up (20 min)

### Task 3. Midpoint (20 min)

### Task 4. Write, Test, Debug, Repeat (20 min)

### Task 5. Optional Challenge Problem

## Recap

It's okay if you don't completely finish all of the exercises during lab. However, we highly encourage you to finish on your own whatever is need to solidify your knowledge. Also take a chance to reflect on what you got what from this lab and whether you feel ready for what comes next!

The takeaways from lab1 should be proficiency with bitwise operations, constructing and using bitmasks, and a solid grasp on the representation of unsigned values as a binary polynomial and signed values in two's complement. Here are some questions to verify your understanding and get you thinking further about these concepts:

- Consider rounding the magnitude of an integer up to power of two (e.g. 3 rounds to 4, 4 to 4, 5 to 8, for negative: -3 rounds to -4, -4 to -4, and so on). How does the bit pattern of a positive int differ from the bit pattern of the value after rounding to power of two? What about for a negative int?
- Give a bitwise expression to zero the upper N bits of an unsigned int V. What does this expression compute numerically?
- When do you supply the command-line arguments to a program you wish to run under gdb: when starting gdb or from within gdb when running the program?
- Chapter 2 of B&O has many excellent practice problems presented with solutions - check them out!
