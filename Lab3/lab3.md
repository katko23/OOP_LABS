# OOP Laboratory Work

## Laboratory #3: Inheritance & Polymorphism

### October Edition

### Task: Document Change Detection System

In this laboratory, your task is to create an Object-Oriented program that monitors and detects changes in documents within a designated folder. This simplified version of git functionality should detect changes in files and provide output about their status since the last snapshot.

---

### General Restrictions

- No third-party libraries are allowed; only those available by default.
- You can create as many classes as needed to ensure a well-structured system.
- **Required Concepts:** Use **Inheritance** and **Polymorphism** (both compile-time and runtime).
- **Using Git:** Commit each significant change. Failure to do so will result in a 2-point deduction and a 2-page report on the usefulness of Git. Submitting without the report will result in the laboratory not being accepted.

---

## Base Laboratory (8th Grade Level)

### Required Actions

Create a program loop with an interactive command line for users to monitor changes in a hardcoded folder location. The three mandatory actions are:

1. **commit** - Updates the snapshot time (a variable) to the current time to emulate change detection from the previous snapshot. The snapshot is updated and resets the state to "clean" (no changes).

2. **info <filename>** - Prints general information about a file. `filename` is unique within the folder.
   - **General File Info:** Display filename, extension, creation date, and last updated date.
   - **Image Files** (`.png`, `.jpg`): Display image dimensions.
   - **Text Files** (`.txt`): Display line count, word count, and character count.
   - **Program Files** (`.py`, `.java`): Display line count, class count, and method count.

3. **status** - Shows the change status of each file since the last snapshot. Each file’s state (changed or unchanged) is displayed.

*Action names are flexible and can be customized.*

---

## Improved Laboratory (9th Grade Level)

- Extend the detection to also identify when files are added or deleted in the specified folder. Display the changes according to the example provided:
  - **Example Output:** `image.png` is a new file, while `python_script.py` was deleted since the last snapshot.

---

## Working System (10th Grade Level)

- **Real-Time Change Detection:** 
  Implement a real-time monitoring system that automatically detects and reports changes in files without needing user actions.
  - **Scheduling:** The system should run a detection flow every 5 seconds, displaying changes as they happen.
  - **Console Availability:** The user should still be able to interact with the program via the console while the monitoring system is running. Minor artifacts (such as overlapping console messages) are acceptable.

---

### Earning Extra Points or Penalties

You may earn or lose points based on the following:
- **Project Structure:** +1 or -1 point for maintaining a clean structure.
- **Coding Conventions:** -1 point for not following language conventions.

---

### Resources

To support your understanding and implementation, consider reviewing the following resources:

- **Inheritance and Polymorphism:**
  - [Java Inheritance (W3Schools)](https://www.w3schools.com/java/java_inheritance.asp)
  - [Java Inheritance (GeeksforGeeks)](https://www.geeksforgeeks.org/inheritance-in-java/)
  - [Java Polymorphism (W3Schools)](https://www.w3schools.com/java/java_polymorphism.asp)
  - [Java Polymorphism (GeeksforGeeks)](https://www.geeksforgeeks.org/polymorphism-in-java/)
  - [Runtime and Compile-Time Polymorphism in Java](https://www.geeksforgeeks.org/difference-between-compile-time-and-run-time-polymorphism-in-java/)

- **Concurrency and File Management:**
  - [Understanding Programs, Processes, and Threads](https://medium.com/@rodbauer/understanding-programs-processes-and-threads-fd9fdede4d88)
  - [Java Threads (Baeldung)](https://www.baeldung.com/java-start-thread)
  - [Java Directories Library](https://docs.oracle.com/javase/tutorial/essential/io/dirs.html)

- **Git:**
  - [Git Flow Introduction](https://nvie.com/posts/a-successful-git-branching-model/)
  - [Git Exercises (W3Schools)](https://www.w3schools.com/git/exercise.asp)
  - Additional Git resources and tutorials can be found by searching online to improve Git fluency and proficiency.
