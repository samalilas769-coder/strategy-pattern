
# Assignment 5 — Strategy Design Pattern

## Project Information
- Course: Software Design Patterns
- Student: Samal
- Project: Calculator Using Strategy Pattern
- Language: Java 17
- Build Tool: Maven
- Design Pattern: Strategy Pattern

## Introduction
This project demonstrates the implementation of the Strategy Design Pattern in Java.

The Strategy Pattern allows different algorithms to be selected and changed at runtime without modifying the main application logic.

## Project Description
The Calculator application supports three mathematical operations:

1. Addition
2. Subtraction
3. Multiplication

Each operation is implemented in a separate strategy class.

## Project Structure

### Strategy Interface
- OperationStrategy.java

### Concrete Strategies
- AddStrategy.java
- SubtractStrategy.java
- MultiplyStrategy.java

### Context
- Calculator.java

### Client
- Main.java

### Unit Tests
- CalculatorTest.java

## How It Works
The OperationStrategy interface defines the execute() method.

Each concrete strategy implements this method.

The Calculator class stores the selected strategy and delegates calculations to it.

The Main class creates strategies and switches between them at runtime using setStrategy().

## Expected Output

    Strategy Pattern Calculator
    Addition: 15.0
    Subtraction: 5.0
    Multiplication: 50.0

## Clean Code Principles
The project demonstrates five Clean Code principles:

1. Clean Unit Tests
2. Single Responsibility Principle
3. Small and Cohesive Classes
4. Separation of Construction and Use
5. Dependency Injection

These principles improve readability, flexibility, maintainability, and testability.

## How to Run
1. Open the project in IntelliJ IDEA.
2. Select JDK 17.
3. Load the Maven project.
4. Open Main.java.
5. Click Run.

## How to Test
Execute the following command in the terminal:

    mvn clean test

The tests verify:
- Addition
- Subtraction
- Multiplication
- Runtime strategy switching
- Null strategy validation

## Advantages
- Flexible strategy switching
- Easy maintenance
- Extensible design
- Reduced coupling
- Independent testing

## Disadvantages
- Requires additional classes
- Adds complexity to small applications
- Client must select the appropriate strategy

## Conclusion
The Strategy Design Pattern allows mathematical operations to be interchangeable at runtime.

The Calculator depends on the OperationStrategy interface instead of specific implementations.

This improves code flexibility, maintainability, and extensibility.

## GitHub Repository
https://github.com/samalilas769-coder/strategy-pattern
