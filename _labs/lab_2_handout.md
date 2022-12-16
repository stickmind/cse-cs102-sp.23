---
type: lab
date: 2023-2-10T08:30:00+00:00
title: '实验 2. C Strings'
tldr: "Lab2 delves into those topics covered in recent string lectures."
pdf: https://h8pqt7tpdf.feishu.cn/file/boxcngByuwpodWGcIJRIDjiRclf
---

This lab delves into those topics covered in recent string lectures.

## Learning Goals

During this lab, you will:

1. read and analyze C code that operates on chars and C-strings
2. use gdb and Valgrind to detect and debug memory errors

## Get Started

To get started on the assignment, you must copy the starter code to your directory.

If you have created a cs102 folder in your home directory, you can type the following command:

```
cp -r /home/cs102-shared/labs/lab2 ~/cs102
```

### Task 1. Code Study: atoi (20 minutes)

### Task 2. Valgrind (30 minutes)

### Task 3. Code Study: strtok (40 minutes)

## Recap

It's okay if you don't completely finish all of the exercises during lab. However, we highly encourage you to finish on your own whatever is need to solidify your knowledge. Also take a chance to reflect on what you got what from this lab and whether you feel ready for what comes next!

The takeaways from lab2 should be further experience with gdb and Valgrind, learning your way around the `string.h` functions and manipulating C-strings as raw arrays/pointers. Here are some questions to verify your understanding and get you thinking further about these concepts:

- In which situations does a call to `strncpy` null-terminate the destination string and in which does it not? What are some of the consequences that result from using a string that is not properly null-terminated?
- A program appears to run just fine, but when run under Valgrind, it reports an error. Your friend dismisses the Valgrind report as off-base and paranoid. They argue that the program runs ok as proof, and what's the big deal? Explain to them why accessing any memory that doesn't belong to you is a problem and further describe how a memory bug can lurk asymptomatically, despite being in error.
- Give a C-expression that reports whether a given `char*` has a matching prefix/suffix N chars long. Be sure to take advantage of the `string.h` library functions. What would happen if your expression were evaluated with a value for N that was longer the string's length?
- The `atoi/strtol` functions convert a string of digits to a decimal, but no standard function that converts in reverse. Describe a technique you could use to convert a number to a string equivalent.
