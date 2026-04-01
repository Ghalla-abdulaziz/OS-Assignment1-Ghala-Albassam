# Reflection Questions

## Instructions
Answer the following questions about your learning experience. Each answer should be **at least 5-7 sentences** and show your understanding.

---

## Question 1: What did you learn about multithreading?

In this assignment, I learned how multithreading works in Java and how multiple threads can simulate concurrent execution. I understood how to create threads using the Runnable interface and how they are started using Thread.start(). I also learned about different thread states such as new, runnable, running, and terminated, and how a thread moves between these states during execution. One important concept I learned is how threads share resources within the same process, which makes them more efficient than using multiple processes. I also understood how the scheduler controls which thread runs at a given time. What surprised me is how the program appears to run multiple tasks at once, even though the CPU is switching between them quickly. Overall, this helped me understand how operating systems manage multiple tasks efficiently.

[Write your answer here. Discuss specific concepts like thread creation, thread states, how threads execute concurrently, what surprised you, etc.]

---

## Question 2: What was the most challenging part of this assignment?

The most challenging part of this assignment was implementing the waiting time calculation correctly. It was difficult to track how long each process stayed in the queue across multiple cycles. Another challenge was dealing with duplicate processes appearing in the final output table, which made the results confusing. I also found it tricky to understand where exactly to place certain lines of code, especially inside the scheduling loop. Additionally, working with Git and commits was initially confusing, especially understanding staging and committing changes properly. These challenges required careful attention to both logic and structure in the program. Overall, the combination of coding and version control made this part more complex.

[Describe the specific challenge. Was it understanding the code? Implementing a feature? Using Git? Explain what made it difficult and how it relates to the course concepts.]

---

## Question 3: How did you overcome the challenges you faced?

I overcame these challenges by breaking the problem into smaller steps and testing each feature separately. For example, I first implemented waiting time tracking, then tested it before adding the summary table. To fix duplicate processes, I analyzed the output and realized that processes were being stored multiple times, so I used a HashMap to keep only unique processes. For the Git issues, I followed step-by-step commands and learned how staging and committing works through practice. I also used debugging by printing outputs and checking values during execution. Asking questions and verifying each step helped me understand the logic better. This approach made it easier to solve problems one by one.

[Describe your problem-solving approach. Did you read documentation? Ask for help? Debug systematically? What resources did you use? What strategies worked?]

---

## Question 4: How can you apply multithreading concepts in real-world applications?

Multithreading is used in many real-world applications such as web browsers, games, and operating systems. For example, a web browser uses multiple threads to load web pages, play videos, and respond to user input at the same time. In games, threads are used to handle graphics rendering, user input, and background processes simultaneously. This improves performance and provides a smooth user experience. Operating systems also use multithreading to run multiple programs efficiently without freezing. The concepts from this assignment, like scheduling and context switching, are directly applied in these systems. Understanding multithreading helps in building responsive and efficient applications.

[Give specific examples from real applications you use (web browsers, games, mobile apps, etc.). Explain why threads are useful in those scenarios. Connect to what you learned in this assignment.]

---

## Additional Reflections (Optional)

### What would you like to learn more about?

[Any topics related to threading, concurrency, or operating systems that you're curious about?]

---

### How confident do you feel about multithreading concepts now?

[Rate yourself and explain: Beginner / Intermediate / Confident]

[Explain your rating - what do you understand well? What needs more practice?]

---

### Feedback on the assignment

[Any comments about the assignment? Was it helpful? Too easy/hard? Suggestions for improvement?]
