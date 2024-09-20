# Lab: 8.0.20

**Objective:**

- Understand the concept and importance of the Singleton Design Pattern in Java development.
- Learn how to implement the Singleton pattern using Java. 
- Explore practical applications of the Singleton pattern in real-world Java projects. 
- Identify common pitfalls and best practices when working with Singletons. 
- Gain hands-on experience with a complete Java example that demonstrates the Singleton pattern.

**Prerequisites:**

- Basic understanding of Java programming.
- Familiarity with object-oriented programming concepts.
- Understanding of static methods and variables in Java.

**What You'll Achieve:**

- Develop a solid understanding of the Singleton Design Pattern.
- Implement a practical example that can be applied in real-world scenarios.
- Enhance your skills in design patterns and Java best practices.

**Assignment Details**

In this assignment, you will create a Singleton class representing a Ford Truck assembly line controller. Follow these steps:

1. Create a FordTruckController class:
   - Make the constructor private to prevent instantiation.
   - Create a private static instance of the class.
   - Implement a public static method `getInstance()` to return the single instance.
   - Add methods to control the assembly line (e.g., `startAssembly()`, `stopAssembly()`, `getStatus()`).
2. Create a `FordTruck` class:
   - Include fields like `model`, `color`, and `assemblyStatus`.
   - Implement a constructor and necessary getter/setter methods.
3. In the `FordTruckController` class:
   - Add a method `assembleTruck(String model, String color)` that creates and returns a new `FordTruck` object.
   - Keep track of the number of trucks assembled.
4. Create a `TruckAssemblySimulation` class with a `main` method:
   - Demonstrate that only one instance of `FordTruckController` can be created.
   - Use the controller to assemble multiple trucks.
   - Show that the same instance is used across different parts of the program.

**Example Output**

```
Ford Truck Assembly Line Simulation

Starting assembly line...
Assembly line started.

Assembling trucks:
Assembled Ford F-150 (Color: Red)
Assembled Ford Ranger (Color: Blue)
Assembled Ford F-250 (Color: Black)

Assembly line status: Running
Total trucks assembled: 3

Stopping assembly line...
Assembly line stopped.

Assembly line status: Stopped

Attempting to create a new controller instance...
Verified: Both controller references point to the same instance.
```

**Starter Code**

The `SmartHomeController.java` file contains the following starter code:

```java
package academy.javapro.lab;

class FordTruckController {
    // Implement Singleton pattern and assembly line control methods here
}

class FordTruck {
    // Implement FordTruck class here
}

public class TruckAssemblySimulation {
    public static void main(String[] args) {
        // Demonstrate Singleton usage and truck assembly here
    }
}

```

**Hints**

- Use a private static field to hold the single instance of `FordTruckController`.
- The `getInstance()` method should create the instance if it doesn't exist, or return the existing instance.
- Consider using lazy initialization for the Singleton instance.
- Remember to make the constructor private to prevent direct instantiation.
- Use the `==` operator to verify that two references to the Singleton point to the same instance.
- Think about how you would make this Singleton thread-safe if required.

**Submission Instructions**

1. Fork the repository
2. Clone your fork
3. Navigate into the repository
4. Implement the required classes and methods
5. Test your implementation with various inputs
6. Git add, commit, and push to your fork
7. Submit a pull request
    - Set the title of the pull request to your first name and last name
    - In the comment, briefly explain your implementation approach and any challenges you faced

Remember, the goal is to learn and have fun! Don't hesitate to ask for help if you get stuck.