# OOP Laboratory Work

## Laboratory #1: Building OOP Solutions

### October Edition

### Task: Student Management System for Technical University of Moldova

You are tasked with designing an Object-Oriented solution to model a **Student Management System** for the Technical University of Moldova (TUM). Your design should allow managing faculties and students, with additional operations.

---

### General Restrictions

- No third-party libraries are allowed, only those available by default.
- You can create as many classes as necessary for a well-structured system.
- You may use advanced concepts such as **Polymorphism**, **Inheritance**, and **Abstraction** where relevant, but they are not mandatory.

---

## Base Laboratory (8th Grade Level)

### Required Operations

- **Faculty Operations:**
  - Create and assign a student to a faculty.
  - Graduate a student from a faculty.
  - Display currently enrolled students (excluding graduates).
  - Display graduates (excluding current students).
  - Check if a student belongs to a specific faculty.

- **General Operations:**
  - Create a new faculty.
  - Search for the faculty of a student by a unique identifier (e.g., email or student ID).
  - Display all university faculties.
  - Display all faculties within a specific field (e.g., *Food Technology*).

---

## Improved Laboratory (9th Grade Level)

- **Persistence:**
  The program should save its state between sessions. Students and faculties created in the previous session must be preserved. Design a `SaveManager` (or `FileManager`) class to handle saving and loading data.

---

## Working System (10th Grade Level)

- **Logging System:**
  Design an operation logging system to track all operations performed in the system, such as student creation, graduation, and faculty creation.

- **Additional Operations:**
  - Batch enrollment of students from a text file.
  - Batch graduation of students from a text file.
  - Input validation with meaningful error messages (e.g., “Cannot graduate student: <email> (student not found)”).

---

### Earning Extra Points or Penalties:

- Maintain a clean project structure.
- Follow the coding conventions of the chosen programming language.
- Demonstrate the use of **SOLID**, **DRY**, and **KISS** principles.

---

## Additional Exercises

### 1. Operator Overloading

**Unary Operator Overloading:** Implement the increment (`++`) and decrement (`--`) operators for the `Student` class to handle operations such as increasing or decreasing the number of credits a student has.

**Binary Operator Overloading:** Implement the `+` operator to allow adding credits between two students, or between a student and a faculty to reflect additional course credit assignment.

Example:
```cpp
Student s1, s2;
s1 += s2;  // Adds s2's credits to s1
```

### 2. Single and Multiple Inheritance
**Single Inheritance**: Create a Person class with basic information like name and age, and derive a Student class that adds specific properties like studentID and faculty.

**Multiple Inheritance**: Design an Employee class, and create a StudentEmployee class by inheriting from both Student and Employee, combining attributes from both classes.

### 3. Pure Virtual Functions and Abstract Classes
Create an abstract base class Person with a pure virtual function getRole().
Derive Student, Teacher, and Administrator classes from Person, each implementing the getRole() function.

Example:

```cpp
class Person {
    virtual string getRole() = 0; // Pure virtual function
};

class Student : public Person {
    string getRole() override {
        return "Student";
    }
};
```

### 4. Polymorphism
Create a function that accepts a pointer to a Person object and prints the role of the person. Using polymorphism, ensure that calling this function with either a Student or Teacher object prints their respective roles.

Example:

```cpp
Person *p = new Student();
printRole(p);  // Output: "Student"
```

### 5. Relationships between Classes: Aggregation and Composition
**Aggregation**: Implement a Faculty class that contains a list of Students. Faculties are aware of their students, but students can exist independently of faculties.

**Composition**: Implement a Library class where a Book is an essential part of the library. The destruction of the library also destroys all the books.

### 6. Polymorphic Logging System
Extend the Logging System from the 10th grade lab by using Polymorphism. Create a base class OperationLogger, and then derive specialized loggers like FileLogger and ConsoleLogger. Each logger should implement the log() function differently.

Example:

```cpp
class OperationLogger {
    virtual void log(const string& message) = 0;
};

class FileLogger : public OperationLogger {
    void log(const string& message) override {
        // Write message to a file
    }
};

class ConsoleLogger : public OperationLogger {
    void log(const string& message) override {
        // Print message to the console
    }
};
```

### 7. Advanced Error Handling with Custom Exceptions
Create custom exception classes for handling specific errors, such as StudentNotFoundException or InvalidFacultyOperation. Ensure your system throws and catches these exceptions where appropriate.
