# Assignment Questions

## Instructions
Answer all 4 questions with detailed explanations. Each answer should be **3-5 sentences minimum** and demonstrate your understanding of the concepts.

---

## Question 1: Thread vs Process

**Question**: Explain the difference between a **thread** and a **process**. Why did we use threads in this assignment instead of creating separate processes?

A process is a program that is currently running and has its own memory and system resources. A thread is a smaller unit of execution inside a process, and multiple threads can exist within the same process while sharing memory.

The main difference is that processes are heavier and take more time and resources to create, while threads are lightweight and faster to manage. Threads also communicate more easily because they share the same memory space.

In this assignment, we used threads instead of processes because we are simulating CPU scheduling inside one program. Using processes would be slower and unnecessary, while threads allow us to simulate multiple running tasks efficiently.

[Write your answer here. Consider: What is a process? What is a thread? How do they differ in terms of memory, resources, creation overhead? Why are threads more suitable for this simulation?]

---

## Question 2: Ready Queue Behavior

**Question**: In Round-Robin scheduling, what happens when a process doesn't finish within its time quantum? Explain using an example from your program output.

In Round-Robin scheduling, if a process does not finish within its time quantum, it is placed back at the end of the ready queue. This allows other processes to get CPU time before it runs again.

[Write your answer here. Describe the specific behavior - where does the process go? When does it run again? Give an example from your actual program output showing a process that was re-queued.]

Example from my output:
```
P3 executing quantum [3000ms]
Remaining time: 6453ms
P3 yields CPU for context switch
➕ P3 added to ready queue
```

In this example, process P3 did not finish during its time quantum, so it stopped execution and was added back to the queue. It then waits for its next turn while other processes execute. This ensures fairness, since every process gets a chance to run.
[Explain what's happening in the output snippet you pasted]

---

## Question 3: Thread States

**Question**: A thread can be in different states: **New**, **Runnable**, **Running**, **Waiting**, **Terminated**. Walk through these states for one process (P1) from your simulation.

**Your Answer:**

[Write your answer here. For each state, explain when P1 enters that state during the simulation. Use your understanding of the code to trace through the lifecycle.]

1. **New**: [When is P1 in New state?]
P1 is in the New state when the thread is created using new Thread(process) but has not started yet.

2. **Runnable**: [When does P1 become Runnable?]
 P1 becomes Runnable after it is added to the ready queue and is waiting for the CPU to execute it.

3. **Running**: [When is P1 Running?]
P1 is in the Running state when Thread.start() is called and the process begins executing its time quantum.

4. **Waiting**: [When/why would P1 be Waiting?]
   P1 goes into a waiting state when it finishes its time quantum and is placed back into the queue, waiting for its next turn.

5. **Terminated**: [When is P1 Terminated?]
   P1 becomes Terminated when its remaining time reaches zero and it finishes execution completely.

---

## Question 4: Real-World Applications

**Question**: Give **TWO** real-world examples where Round-Robin scheduling with threads would be useful. Explain why this scheduling algorithm works well for those scenarios.

**Your Answer:**

### Example 1:Operating Systems (CPU Scheduling)

**Description**: 
Operating systems like Windows or Linux manage multiple programs running at the same time, such as browsers, games, and background services.

**Why Round-Robin works well here**: 
Round-Robin ensures that each program gets a fair share of CPU time, preventing any program from taking over the system. It also improves responsiveness, so users can switch between applications smoothly.

### Example 2: Web Servers Handling Multiple Requests

**Description**: 
Web servers handle many user requests at the same time, such as loading web pages or processing data.

**Why Round-Robin works well here**: 
It ensures each request gets processed fairly without one request blocking others. This improves performance and keeps the server responsive even under heavy load.
---

## Summary

**Key concepts I understood through these questions:**
1. Difference between threads and processes
2. How Round-Robin scheduling ensures fairness
3. How thread states change during execution

**Concepts I need to study more:**
1. Advanced scheduling algorithms
2. Thread synchronization and race conditions
