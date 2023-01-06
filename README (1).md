---
description: Get familiar with the C programming language with the queue data structure
---

# P0: Queue

The intention of this project is to teach you some basic C that you will need to complete the following projects. You will implement a queue as a simple, _singly linked list_, as well as a test program.

The API is specified in queue.h and hopefully self-explanatory. Do not modify queue.h: you are only supposed to turn in queue.c and test\_queue.c. This project will be auto-graded.

To compile, run (from the shell):

```
make
# or 'make test_queue'
```

When 'make' completes, there will be a program called 'test\_queue'. There are some comments in Makefile for you to understand what happened. You can run this program from the shell as follows:

```
./test_queue
```

To clean up, run

```
make clean
```

Try to do this last thing if you have any 'strange' issues with building. Sometimes it helps to build things from scratch.

If you have build/compiling issues, please investigate them yourself before asking on Ed Discussion or coming to office hours. Google and Stack Overflow are your friends!

Put your tests in the test\_queue.c file. It is compiled automatically when you run make and includes a single basic test and framework. Testing is important. Your tests should be thorough and organized so that someone who hasn't seen your interface can figure out what's going on.

test\_queue should not output anything (!) and exit with status 0 if no bugs are found. test\_queue should output a brief, self-explanatory error report and exit with a non-zero status if a bug was found. At most one bug should be reported.

Make sure all your code is well-commented. Anybody should be able to look at your code and quickly understand what's going on even without looking at the C code.

Common misunderstandings:

* Feel free to add data structures in queue.c.
* The user is allowed to enqueue and dequeue NULL items.
* All operations should be O(1), except iterate() and delete() i.e., execution time should not grow with the length of the queue.
* assert() is to check invariant and can be used within queue.c to check the integrity of the queue. Do not use it as a shortcut to report failures in test\_queue.c.
* In this project, your code does not have to check for invalid arguments. If somebody calls dequeue on a NULL pointer, that is allowed to crash. If your code is called with bad arguments, then its behavior will be undefined.

Submission and grading:

* Submit all files in the directory in an archive, after `make clean`.
* We will test whether your queue is correct by testing the various functions (enqueue, dequeue, etc.).
* We will test whether your test\_queue is correct by compiling it with various _wrong_ queue implementations and see whether your test\_queue complains that the queue is wrong. And vise versa for correct queue implementations.

Resources:

C programming tutorial: http://www.lysator.liu.se/c/bwk-tutor.html&#x20;

Basic C Reference: https://www.geeksforgeeks.org/c-language-set-1-introduction/&#x20;

C debugger, GDB: https://www.gnu.org/software/gdb/

Have fun!

