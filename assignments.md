---
layout: assignments
title: 作业发布
permalink: /assignments/
---

### Assignment Tips

- **Be cautious with C**: C is designed for high efficiency and unrestricted programmer control, with no emphasis on safety and little support for high-level abstractions. A C compiler won't complain about such things as uninitialized variables, narrowing conversions, or functions that fail to return a needed value. C has no runtime error support, which means no helpful messages when your code accesses an array out of bounds or dereferences an invalid pointer; such errors compile and execute with surprising results. Keep an eye out for problems that you may have previously depended on the language to detect for you.
- **Memory and pointers**: Bugs related to memory and/or pointers can be tricky to resolve. Make sure you understand every part of your code that you write or change. Also keep in mind that the observable effects of a memory error can come at a place and time far removed from the root cause (i.e. running off the end of a array may "work fine" until you later read the contents of a supposedly unrelated variable). gdb and Valgrind can be extremely helpful in resolving these kinds of bugs. In particular, Valgrind is useful throughout the programming process, not just at the end. Valgrind reports on two types of memory issues: *errors* and *leaks*. Memory errors are toxic and should be found and fixed without delay. Memory leaks are of less concern and can be ignored early in development. Given that the wrong deallocation can wreak havoc, we recommend you write the initial code with all `free()` calls commented out. Much later, after having finished with the correct functionality and turning your attention to polishing, add in the `free` calls one at a time, run under Valgrind, and iterate until you verify complete and proper deallocation.
- **Use good style from the start**: Always start with good decomposition, rather than adding it later. Sketch each function's role and have a rough idea of its inputs and outputs. A function should be designed to complete one well-defined task. If you can't describe the function's role in a sentence or two then maybe your function is doing too much and should be decomposed further. Commenting the function before you write the code may help you clarify your design (what the function does, what inputs it takes, and what outputs it produces, how it will be used). Start by using good variable names, rather than going through and changing them later. Using good style the first time makes your code better designed, easier to understand, and easier to debug.
- **Understand your code**: At every step, you want to ensure that you understand the code you are writing, what it does, and how it works. Don't make changes without understanding why you are making them, and what the result will be.
- **Testing**: use our recommended testing techniques to incrementally develop your program, test at each step, and always have a working program.

### Frequently Asked Questions

- **What is the expected assignment workload?**

  There are roughly 6 assignments and a final project, spaced about *a two-week apart*. These are largely programming projects with occasional problem-set-like activities mixed in. Each assignment will take between 10 and 20 hours.

- **What programming environment and tools are used?**

  You can use your own account on Linux machines and login remotely. You can edit, compile, and debug on the systems using a suite of open source development tools including `gcc`, `make`, `gdb` and `valgrind`, with cs102-specific tools `codecheck` and `sanitycheck`.

- **How are assignments weighted?**

  The total number of points for an assignment is noted in its writeup. The points indicate the weight of that assignment relative to the others; i.e. an assignment graded out of 100 points has twice the weight of one graded out of 50.

- **How can I reproduce/debug a problem that appears during sanity check?**

  Look through the sanity check output to find the command being executed:

  ```
  Command: ./triangle -1
  ```

  Run that same command (in shell, gdb, or Valgrind) to replicate the situation being tested.

- **Is it possible to write a custom test to verify Valgrind correctness or memory/time efficiency?**

  Unfortunately not; custom sanity check tests compare on output only. You will need to supplement with other forms of testing to verify those additional requirements.
