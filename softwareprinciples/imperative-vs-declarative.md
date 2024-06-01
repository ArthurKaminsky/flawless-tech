# Imperative vs Declarative Programming

Imperative programming is a programming paradigm that focuses on explicitly specifying the sequence of operations or steps that the computer 
must take to achieve a desired outcome. In imperative programming, you describe how to accomplish a task through detailed instructions, 
which the computer follows step-by-step.

For example, let's make a sandwitch. We need to have the ingredients and the instructions in order to make our sandwitch.
You get the ingredients and then follow step by step in making the sandwitch based on the instructions.

Declarative programming is a programming paradigm where you describe the desired outcome or end result, 
rather than explicitly writing the step-by-step instructions for achieving that outcome. 
In declarative programming, you focus on what you want to accomplish rather than how to accomplish it.

For example, instead of making the sandwitch yourself, you go to a restaurant or a coffee shop and buy a sandwitch.
You can buy an already made sandwitch or have the chef make one for you.
You don't focus on the how, but on the what of the end result.

## Further Explanation of Declarative Programming

Here are some key characteristics of declarative programming:

> * Focus on What, Not How: Instead of specifying the exact sequence of steps to perform a task,
you declare what you want to achieve, and the underlying system or framework figures out how to accomplish it.

> * Higher Level of Abstraction: Declarative programming operates at a higher level of abstraction compared to imperative programming.
It allows you to express complex logic in a concise and readable manner.

> * Decoupling of Concerns: Declarative code often leads to better separation of concerns,
as it emphasizes the intent or purpose of the code rather than its implementation details.
This can improve code maintainability and readability.

> * Emphasis on Expressiveness: Declarative programming languages and frameworks often prioritize expressiveness,
allowing developers to write code that closely resembles natural language or mathematical expressions.

> * Declarative Constructs: Declarative programming often involves the use of specific language constructs or frameworks
designed to facilitate declarative-style code, such as declarative SQL queries, HTML templates in web development, or configuration files in software deployment.

> * Immutable Data: Declarative programming often promotes the use of immutable data structures,
where data is not modified in place but instead transformed through pure functions or transformations.

Declarative programming contrasts with imperative programming, where the focus is on explicitly 
specifying the sequence of steps needed to achieve a desired outcome. 
Examples of declarative programming paradigms and languages include SQL for database queries, 
HTML/CSS for web development, and declarative configuration languages like YAML or JSON for system configurations.

--------------------------------------------

Generated answers from ChatGPT

## Further Explanation of Imperative Programming

Here are some key characteristics of imperative programming:

> * Focus on How, Not What: Imperative programming involves writing code that specifies exactly how to perform tasks.
You give explicit commands that detail the control flow and operations needed to achieve the result.

> * Sequential Execution: Imperative programs are generally written as a sequence of statements or instructions that are executed in order.
Control flow constructs like loops, conditionals, and function calls are used to manage the execution sequence.

> * State and Mutability: Imperative programming often involves managing state through variables and mutable data structures. 
Variables can be updated and changed throughout the program's execution.

> * Detailed Instructions: In imperative programming, you provide detailed instructions to the computer, 
breaking down tasks into smaller, precise steps. This often includes low-level operations like memory 
management and manipulation of data structures.

> * Procedural Code: Imperative programming is closely related to procedural programming, 
where code is organized into procedures or functions that encapsulate sequences of operations. 
These procedures can be called and executed as needed.

> * Examples: Common imperative programming languages include C, C++, Java, Python, and JavaScript. 
These languages allow you to write detailed instructions and manage the flow of execution explicitly.

## Comparison Between the Both

Imperative Programming:

* You describe how to do something.
* Focus on control flow and state changes.

Examples: Writing a for-loop to iterate over a collection, manually updating the state of variables.

Declarative Programming:

* You describe what you want to achieve.
* Focus on describing the desired result, abstracting away the control flow.

Examples: Writing an SQL query to fetch data, using HTML to describe the structure of a web page.

**Example**
Imperative Code (Python):
```Python
# Imperative approach to find the sum of squares of a list of numbers
numbers = [1, 2, 3, 4, 5]
sum_of_squares = 0
for number in numbers:
    square = number * number
    sum_of_squares += square
print(sum_of_squares)
```
Declarative Code (Python):
```Python
# Declarative approach to find the sum of squares of a list of numbers using map and sum functions
numbers = [1, 2, 3, 4, 5]
sum_of_squares = sum(map(lambda x: x * x, numbers))
print(sum_of_squares)
```
In the imperative example, you explicitly detail the steps of looping through the list, 
calculating the square of each number, and summing them up. In the declarative example, 
you express the intent to calculate the sum of squares using higher-level functions without detailing the control flow.
