# Reflection Questions

## Instructions
Answer the following questions about your learning experience. Each answer should be **at least 5-7 sentences** and show your understanding.

---

## Question 1: What did you learn about multithreading?

**Your Answer:**

I gained practical knowledge about Java multithreading through this assignment. A thread is faster than a process because it shares memory and is a lightweight unit of execution. I was able to comprehend how start() is used to generate threads and how they go through several phases, including New, Runnable, Running, Waiting, and Terminated. Additionally, I discovered how join() synchronizes thread execution. The idea that threads operate concurrently to mimic CPU scheduling was crucial. I was able to comprehend how each process receives an equal amount of CPU time by putting Round-Robin into practice. I was able to make the connection between theoretical ideas from the textbook and practical application thanks to this project.

---

## Question 2: What was the most challenging part of this assignment?

**Your Answer:**
Implementing the waiting time feature (Feature 3) was the most difficult aspect of this task. Finding the right location within the scheduling loop to compute waiting time without altering the logic was challenging. Additionally, I had trouble accessing private variables like arrivalTime and totalWaitingTime, which led to a number of errors. It was also difficult to determine when a process began waiting and ended, particularly when Round-Robin re-queuing was involved. Furthermore, the sequence in which start(), join(), and fetching the process from the map were performed was quite delicate. Inaccurate results were caused by a little error. A deeper comprehension of thread behavior and scheduling was necessary for this section.

---

## Question 3: How did you overcome the challenges you faced?

**Your Answer:**
By focusing on one issue at a time and breaking the difficulty down into smaller steps, I was able to overcome the obstacles. I started by going over the scheduler loop's structure to determine the proper locations for each operation. To confirm computations, I employed debugging strategies such outputting intermediate values. In order to properly access private variables, I also implemented object-oriented principles by providing getter and setter methods. I was able to comprehend ideas like context switching and waiting time by consulting the textbook and lecture notes. After each modification, I evaluated the program to make sure it was accurate. I was able to find mistakes fast and correct them effectively because to this methodical approach.

---

## Question 4: How can you apply multithreading concepts in real-world applications?

**Your Answer:**
Numerous real-world applications make extensive use of multithreading. For instance, web browsers increase responsiveness by using many threads to load sites, execute scripts, and process user input at the same time. Additionally, operating systems employ scheduling algorithms like Round-Robin to effectively manage several processes through the usage of threads. Threads are used in mobile applications to do background operations, including loading data, without causing the user interface to freeze. Additionally, servers use multithreading to manage several client requests concurrently. Performance and scalability are enhanced as a result. I can use the ideas I gained from this assignment to develop effective systems that need responsiveness and concurrency.

---

## Additional Reflections (Optional)

### What would you like to learn more about?
Advanced scheduling algorithms like Priority Scheduling, Multilevel Queue Scheduling, and Multilevel Feedback Queue are topics I'd like to learn more about. Additionally, I'd like to understand more about thread synchronization methods like monitors, locks, and semaphores. How to avoid common multithreading problems like race situations and deadlocks is another area I would want to investigate. It would also be helpful to comprehend how actual operating systems optimize scheduling choices. I would learn more about concurrency and system performance from these subjects.

---

### How confident do you feel about multithreading concepts now?
Intermediate

I believe my comprehension of multithreading principles has reached an intermediate level. I am at ease with fundamental concepts like Round-Robin scheduling, lifetime, and thread generation. Additionally, I am able to incorporate aspects like context switching and waiting time into a simulation. I still need to practice advanced concepts like synchronization and managing challenging concurrency issues, though. I think I can further develop my abilities with additional practice and exposure to real-world situations.

---

### Feedback on the assignment
I learned a lot about how operating system theory is implemented in actual code thanks to this assignment. It offered an excellent balance between comprehending ideas and putting them into practice. Although some aspects, such as feature implementation, required careful consideration and debugging, the level of difficulty was appropriate. Giving a little more direction on where to add new features to the code is one way to make it better. All things considered, the task was interesting and improved my comprehension of CPU scheduling and multithreading.
