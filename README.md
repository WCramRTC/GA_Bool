
# Guided Assignment - Introduction to Boolean (Bool) in C#

## Introduction

A boolean, in programming, is a data type that represents a binary value, typically denoting one of two possible states: `true` or `false`. Booleans are fundamental in programming as they are used to control the flow of a program, make decisions, and store binary conditions or flags.

In C#, the `bool` data type is used to declare and work with boolean values. Here's a basic explanation of its usage in C#:

1. **Declaration and Initialization:**
   You can declare a boolean variable in C# like this:
   ```csharp
   bool isTrue; // Declaration without initialization
   ```
   You can also initialize a boolean variable at the time of declaration:
   ```csharp
   bool isEnabled = true; // Initialization with the value 'true'
   ```

2. **Comparison and Conditions:**
   Booleans are commonly used in conditional statements like `if`, `else`, `while`, `for`, and so on. They determine the flow of the program based on whether a condition is `true` or `false`. For example:
   ```csharp
   bool isUserLoggedIn = true;

   if (isUserLoggedIn)
   {
       // Code to execute when the user is logged in
   }
   else
   {
       // Code to execute when the user is not logged in
   }
   ```

3. **Logical Operations:**
   Booleans can be combined using logical operators like `&&` (AND), `||` (OR), and `!` (NOT). These operators allow you to create complex conditions by combining simple boolean expressions. For example:
   ```csharp
   bool isStudent = true;
   bool isTeenager = false;

   bool canVote = isStudent && !isTeenager; // AND and NOT operators
   ```

4. **Function Returns:**
   Functions and methods in C# often return boolean values to indicate success or failure. For instance, a function that checks if a file was successfully saved could return `true` for success and `false` for failure.

5. **Boolean Arrays and Collections:**
   Booleans can be used to create arrays or collections to represent multiple binary states. For example, you can use an array of booleans to represent the state of multiple checkboxes in a user interface.

6. **Boolean Expressions in Loops:**
   Booleans are used in loop control expressions. You can use them to determine whether a loop should continue running or terminate based on a certain condition.

---

### Project Requirements

1. **Project Naming:** The project should be named `GA_Bool_YourName`.
2. **Code Commenting:** Include a comment at the top of the code with your name.
3. **Code Compilation:** The submitted code should be free from compile errors.
4. **Implementation of Steps:** All the steps from the guided assignment should be correctly implemented.
    - Step 1: Display a Boolean Value
    - Step 2: Declaring a Boolean Variable
    - Step 3: Using Booleans in Conditional Statements
    - Step 4: Toggling a Boolean Value
    - Step 5: Boolean Logic

---

## Step By Step

## Watch the Boolean Segment of the Lecture 4 ( Starts at 32:30 - 2 Minutes)
## https://www.youtube.com/watch?v=QwpnaIsL1MQ&t=1950s

Then following instructions in the Step By Step portion of the assignment on GitHub

### Starting Code
```csharp
using System;

class Program
{
    static void Main(string[] args)
    {
        Console.WriteLine("Boolean Value: False");
    }
}
```

**Understanding the Code:** This initial code prints a boolean value to the console. We will modify this to understand booleans better.

**Write this code**  
- Add a comment above the `Main` method for context.

```csharp
    // Entry point of our C# program
    static void Main(string[] args)
    {
        Console.WriteLine("Boolean Value: False");
    }
```

---

### **Step 1: Display a Boolean Value**

**Objective:** Learn to print a boolean value.

Replace `"Boolean Value: False"` with the boolean value `true`. Booleans in C# represent true or false values and do not need quotes.

```csharp
static void Main(string[] args)
{
    Console.WriteLine(true);
}
```

**Run your code**  
You should see `True` printed.

**Understanding Booleans:** In C#, a boolean (`bool`) represents a true or false value.

---

### **Step 2: Declaring a Boolean Variable**

**Objective:** Learn to store true or false values in variables.

1. Declare a `bool` variable named `isAdult` and assign a value to it.

```csharp
    bool isAdult = true; // Replace true with true or false
```

2. Update `Console.WriteLine` to use `isAdult`.

```csharp
    Console.WriteLine(isAdult); 
```

**Run your code**

The value assigned to `isAdult` will be displayed.

**Understanding Variables:** A `bool` variable in C# can hold either `true` or `false`.

---

### **Step 3: Using Booleans in Conditional Statements**

**Objective:** Learn to use `bool` in conditional statements.

1. Write an `if` statement to check if `isAdult` is true and print a message.

```csharp
    if (isAdult)
    {
        Console.WriteLine("You are an adult.");
    }
    else
    {
        Console.WriteLine("You are not an adult.");
    }
```

**Run your code**  

Based on the value of `isAdult`, the appropriate message will be displayed.

**Understanding Conditionals:** Booleans are often used in conditional statements to control the flow of programs.

---

### **Step 4: Toggling a Boolean Value**

**Objective:** Understand how to change the value of a boolean.

Toggle the value of `isAdult`.

1. Change the value of `isAdult` to `false` and observe the output.

```csharp
    isAdult = false;
    Console.WriteLine(isAdult);
```

**Run The Code**

The new boolean value will be displayed.

---

### **Step 5: Boolean Logic**

**Objective:** Explore basic boolean logic.

Experiment with boolean logic using the `&&` (AND) and `||` (OR) operators.

1. Declare another boolean `hasLicense` and set it to `true`.
2. Use boolean logic to check multiple conditions.

```csharp
    bool hasLicense = true;
    if (isAdult && hasLicense)
    {
        Console.WriteLine("You are an adult and have a license.");
    }
    else
    {
        Console.WriteLine("Condition not met.");
    }
```

**Run your code**

The result will depend on the combination of `isAdult` and `hasLicense`.

**Understanding Boolean Logic:** Boolean logic is fundamental in programming, allowing complex conditions to be evaluated.

---

### Additional Tips and Resources

- **Debugging:** Ensure that you use the correct boolean operators for your logic.
- **Challenge:** Try creating more complex conditions using boolean logic.
- **Further Learning:** Explore [Microsoft's C# documentation](https://docs.microsoft.com/en-us/dotnet/csharp/) for advanced boolean operations.
- **Syntax Highlighting:** Notice how different elements like variables, booleans, and conditional statements are highlighted.

---


Based on the provided guided assignment, here are the requirements and rubric for the project:



### Rubric

| **Name** | **Description** | **Points** |
|----------|-----------------|------------|
| Project Naming | The project is named `GA_Bool_YourName`. | 10 |
| Code Commenting | A comment with the student's name is included at the top of the code. | 10 |
| Error-Free Code | The submitted code compiles without any errors. | 20 |
| Step 1 Completion | Correctly displaying a boolean value (`true`) in the console. | 10 |
| Step 2 Completion | Successfully declaring a `bool` variable and using it in `Console.WriteLine`. | 10 |
| Step 3 Completion | Implementing an `if` statement using the `bool` variable and displaying appropriate messages. | 10 |
| Step 4 Completion | Toggling the `bool` value and observing the output change. | 10 |
| Step 5 Completion | Using `&&` (AND) and `||` (OR) operators correctly in a conditional statement with two `bool` variables. | 10 |
| Additional Challenge | Completing an additional challenge like creating more complex conditions using boolean logic. | 10 |

**Total Points:** 100

### Additional Notes

- Students should follow the guided assignment closely and ensure they understand each step before proceeding.
- Creativity in the additional challenge will be appreciated but should adhere to the use of boolean logic.
- Proper coding practices, such as meaningful variable names and readability, are encouraged.
- The rubric points for each step are based on both implementation and understanding, as evidenced by the code written.