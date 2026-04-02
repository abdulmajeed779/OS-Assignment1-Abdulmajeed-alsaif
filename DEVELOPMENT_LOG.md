# Development Log

## Instructions
Document your development process as you work on the assignment. Add entries showing:
- What you worked on
- Problems you encountered
- How you solved them
- Time spent

**Requirements**: Minimum 5 entries showing progression over time.

---

## Example Entry Format:

### Entry 1 - [April 1, 2026, 2:30 PM]
**What I did**: Forked the repository and set up my student ID

**Details**: 
- Created GitHub account with university email
- Forked the starter repository
- Changed student ID on line 92 to my actual ID (441234567)
- Compiled and ran the program successfully

**Challenges**: Had to install JDK first because javac wasn't recognized

**Solution**: Downloaded JDK 17 from Oracle website and set PATH variable

**Time spent**: 30 minutes

---

## Your Development Log:

### Entry 1 - [MARCH 28, 2026, 11:08 PM]
**What I did**:Set up the project and ran the initial code 

**Details**: 
-Opened the project in Visual Studio
-Updated the student ID in the code
-Compiled and ran the program successfully
-Observed the Round-Robin scheduling output
**Challenges**: 
Understanding the structure of the code and how threads are used
**Solution**: 
Read through the code carefully and followed execution step by step
**Time spent**: 
45 minutes
---

### Entry 2 - [MARCH 30, 2026,  11:42 PM]
**What I did**: Implemented Feature 1 (Process Priority)

**Details**: 
-Added priority variable to Process class
-Generated random priority values (1–5)
-Modified output to display priority in ready queue
**Challenges**: 
Updating constructor and making sure priority prints correctly
**Solution**: 
Modified constructor and tested output multiple times
**Time spent**: 
1 hour
---

### Entry 3 - [MARCH 30, 2026, 9;47 PM]
**What I did**: Implemented Feature 2 (Context Switch Counter)

**Details**: 
-Added global counter variable
-Incremented it before each thread execution
-Printed total context switches at the end
**Challenges**: 
Finding the correct place to increment the counter
**Solution**: 
Placed the increment before start() based on scheduler logic
**Time spent**: 
45 minutes
---

### Entry 4 - [April 2, 2026, 3:41 PM]
**What I did**:Implemented Feature 3 (Waiting Time) 

**Details**: 
-Added arrivalTime and totalWaitingTime variables
-Implemented getter and setter methods
-Calculated waiting time inside scheduling loop
**Challenges**: 
Many errors due to private variables and incorrect placement
**Solution**: 
Used getters/setters and carefully adjusted code order
**Time spent**: 
2 hours
---

### Entry 5 - [April 2, 2026, 7:00 PM]
**What I did**: Debugging and fixing errors

**Details**: 
-Fixed syntax errors like incorrect print statements
-Corrected code order inside loop
-Verified waiting time calculations using output
**Challenges**: 
Multiple errors appearing from small mistakes
**Solution**: 
Debugged step by step and tested after each fix
**Time spent**: 
1.5 hours
---

### Entry 6 - [April 2, 2026, 9:00 PM]
**What I did**: Final testing and documentation

**Details**: 
-Ran full simulation and checked final output
-Verified Process Summary and context switches
-Completed ANSWERS.md and REFLECTION.md
**Challenges**: 
Ensuring output matches expected behavior
**Solution**: 
Compared results with logic and fixed minor issues
**Time spent**: 
1 hour
---

## Summary

**Total time spent on assignment**: 6.5 hours

**Most challenging part**: 
Implementing the waiting time feature and placing the logic correctly inside the scheduling loop
**Most interesting learning**: 
Knowing how Round-Robin scheduling operates for threads
**What I would do differently next time**: 
I would plan the features before coding and test each part earlier to reduce debugging time
