---
type: lab
date: 2023-3-1T08:30:00+00:00
title: '实验 3. Pointers, Arrays and the Heap'
tldr: "Lab3 delves into topics covered in recent pointer, array and the heap lectures."
pdf: https://h8pqt7tpdf.feishu.cn/file/boxcn0nfaK08XAdGU8DOaedBIBe
---

This lab delves into topics covered in recent pointer, array and the heap lectures.

## Learning Goals

During this lab, you will:

1. investigate how arrays and pointers work in C
2. get further practice with gdb and valgrind
3. experiment with code that dynamically allocates memory on the heap

## Get Started

To get started on the assignment, you must copy the starter code to your directory.

If you have created a cs102 folder in your home directory, you can type the following command:

```
cp -r /home/cs102-shared/labs/lab3 ~/cs102
```

### Task 1. GDB: Pointers and Arrays (15 minutes)

### Task 2. Code Study: Heap Use (15 minutes)

### Task 3. Code study: calloc (15 minutes)

### Task 4. Valgrind: Heap Errors (15 minutes)

### Task 5. Valgrind: Memory Leaks (15 minutes)

### Task 6. Debugging (15 minutes)

## Recap

It's okay if you don't completely finish all of the exercises during lab; your sincere participation for the full lab period is sufficient for credit. However, we highly encourage you to finish on your own whatever is needed to solidify your knowledge. Also, take a chance to reflect on what you got what from this lab and whether you feel ready for what comes next!

The takeaways from lab3 should be continued development of your gdb and Valgrind skills, as well as your skills reading and writing code with heavy use of pointers. Arrays and pointers are ubiquitous in C and a good understanding of them is essential. Here are some questions to verify your understanding and get you thinking further about these concepts:

- If `ptr` is declared as an `char *`, what is the effect of `ptr++`? What if ptr is declared as a `int *`?
- Although `&` applied to the name of a stack-allocated array (e.g. `&buffer`) is a legal expression and has a defined meaning, it isn't really sensible. Explain why such use may indicate an error/misunderstanding on the part of the programmer.
- The argument to malloc is `size_t` (unsigned). Consider the erroneous call `malloc(-1)`, which seems to make no sense at all. The call compiles with nary a complaint -- why is it "ok"? What happens when it executes?
- What is the purpose of the `realloc` function? What happens if you attempt to realloc a non-malloc-ed pointer, such as a string constant?
- What is the difference between a memory error and a memory leak?
