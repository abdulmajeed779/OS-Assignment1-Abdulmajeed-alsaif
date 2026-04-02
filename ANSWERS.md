# Assignment Questions

## Instructions
Answer all 4 questions with detailed explanations. Each answer should be **3-5 sentences minimum** and demonstrate your understanding of the concepts.

---

## Question 1: Thread vs Process

**Question**: Explain the difference between a **thread** and a **process**. Why did we use threads in this assignment instead of creating separate processes?

**Your Answer:**
A thread is a small unit of execution that lives inside a process and shares the same memory and resources as a process, whereas a process is an independent program in operation with its own memory space, resources, and system state, Because they don't need separate memory allocation, threads can be created and switched between more quickly than processes,Because the scheduler simulation calls for frequent context switching and lightweight execution, we employed threads rather than processes in this assignment, Using procedures would result in significant overhead and decreased productivity, We can more effectively and realistically mimic CPU scheduling behavior (such as Round-Robin) by using threads.

---

## Question 2: Ready Queue Behavior

**Question**: In Round-Robin scheduling, what happens when a process doesn't finish within its time quantum? Explain using an example from your program output.

**Your Answer:**
A process in Round-Robin scheduling is preempted and placed at the end of the ready queue if it does not complete within the allotted time quantum, By letting other processes run before it gets its turn, this guarantees equity, The process will remain in line until it gets to the front once more and is given a new time quantum.


Example from my output:
```? P1 executing quantum [3000ms] ? P1 completed quantum 3000ms │ Overall progress: 66% Remaining time: 1496ms ? P1 yields CPU for context switch ? P1 (Priority: 1) added to ready queue
```

**Explanation of example:**
In this instance, process P1 had 1496 milliseconds left, hence it did not complete execution after its time quantum of 3000 milliseconds, Consequently, the scheduler put it at the end of the ready queue and halted its execution, This illustrates the Round-Robin behavior, in which each process cycles through the queue until it completes execution and receives an equal amount of CPU time.

---

## Question 3: Thread States

**Question**: A thread can be in different states: **New**, **Runnable**, **Running**, **Waiting**, **Terminated**. Walk through these states for one process (P1) from your simulation.

**Your Answer:**

[Write your answer here. For each state, explain when P1 enters that state during the simulation. Use your understanding of the code to trace through the lifecycle.]

1. **New**: P1 is in the New state when the thread is created using the constructor but before the start() method is called.

2. **Runnable**: After calling start(), P1 moves to the Runnable state, where it is ready to run and waiting for the CPU scheduler to assign it execution time.

3. **Running**: P1 enters the Running state when the CPU scheduler selects it and executes it for a time quantum, as shown in the output when it starts executing.

4. **Waiting**: P1 enters the Waiting state when the main thread calls join() and waits for the thread to finish its execution slice before continuing.

5. **Terminated**: P1 reaches the Terminated state after it completes all its remaining burst time, as shown in the output:

---

## Question 4: Real-World Applications

**Question**: Give **TWO** real-world examples where Round-Robin scheduling with threads would be useful. Explain why this scheduling algorithm works well for those scenarios.

**Your Answer:**

### Example 1: Operating System Task Scheduling

**Description**: 
Modern operating systems manage multiple processes such as applications, background services, and system tasks simultaneously.

**Why Round-Robin works well here**: 
Round-Robin ensures that all processes get a fair share of CPU time, preventing any single process from monopolizing the CPU. This improves system responsiveness and ensures that interactive applications do not freeze.

### Example 2: Web Server Request Handling

**Description**: 
A web server handles multiple client requests at the same time using threads.
**Why Round-Robin works well here**: 
Using Round-Robin scheduling ensures that each client request is processed fairly and efficiently. No single request can block others, which improves performance and user experience, especially under heavy load.

---

## Summary

**Key concepts I understood through these questions:**
1. The difference between threads and processes and why threads are more efficient for simulations.
2. How Round-Robin scheduling ensures fairness by re-queuing incomplete processes.
3. The lifecycle of a thread and its different states during execution.

**Concepts I need to study more:**
1.Advanced scheduling algorithms like Priority Scheduling and Multilevel Queue Scheduling. 
2. Optimization techniques for reducing context switching overhead.
