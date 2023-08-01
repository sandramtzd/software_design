# Software Design Methodologies

There are three principle design strategies used in software engineering:

- Structured design
- Function oriented design
- Object oriented design

Within each methodology there are various **design patterns** which provide further structure for us. In practice ***the language used for a project will likely be the last thing to be chosen***, determined by a combination of methodology and design pattern.

## Task

1. What do we mean by **coupling** and **cohesion** when discussing structured design?

**Cohesion** refers to what the class (or module) can do. There is two types of cohesion:

| Type | Description | Example
| ----------- | ----------- | -----------
Low cohesion | A class does a great variety of actions | STAFF checkEmail() sendEmail() emailValidate() PrintLetter()
High cohesion | The class is focused on what it should be doing and have only methods relating to the intention of the class | STAFF -salary -emailAddr   setSalary(newSalary) getSalary() setEmailAddr(newEmail) getEmailAddr()     

**Coupling** refers to how related or dependent two classes (or modules) are toward each other.
| Type | Description |
Low coupled classes | Changing something major in one class should not affect the other
High coupling | Making a change could require an entire system revamp

REMEMBER : *Good software design has **high cohesion** and **low coupling** .*

Reference : https://stackoverflow.com/questions/3085285/difference-between-cohesion-and-coupling

2. What is the difference between **top-down** and **bottom-up** design? Which best describes a function oriented design?

In the **top down** approach, a complex algorithm is broken into smaller fragments (modules). These modules are then further broken down into smaller fragments until they can no longer be fragmented.

On the other hand, **bottom-up** model, focuses on designing an algorithm by begining at the very basic level and building up as it goes. The modules here are designed individually and are integrated together to form a complete algorithmic design. 

The differences between *top-down* and *bottom-up* approach are as follows:

| Basis | Top-Down | Bottom-Up
| ----------- | ----------- | ------------
| Approach | Top-Down Approach is Theory-driven | Bottom-Up Approach is Data-Driven |
Significance | Emphasis is on doing things (algorithms) | Emphasis is on data rathar than procedure
| Focus | Large programs are divided into smaller programs which is known as decomposition | Programs are divided into what are known as objects is called Composition |
|Interaction | Communication is less among the modules | Communication is a key among the modules |
| Areas | Widely used in debugging, module documentation, etc | Widely used in testing |
| Language | The top-down approach is mainly used by Structured programming languages like C, Fortran, etc | The bottom-up approach is used by Object-Oriented programming languages like C++, C#, Java, etc |
| Redundancy | May contains redundancy as we break up the problem into smaller fragments, then build that section separately | This approach contains less redundancy if the data encapsulation and data hiding are being used |

Furthermore, ***the bottom-up model describes better a function oriented design***  since this approach divide programs into what are known as objects by composition. The bottom up approach finds its uses in testing and object-oriented programming languages like Java. 

Reference: https://www.codingninjas.com/studio/library/top-down-vs-bottom-up-programming-whats-the-difference


3. In which design methodology would a **class diagram** be most useful?

A class diagram would be most useful in ***object oriented design***. This design is the result of focusing attention not on the funcion performed by the program, but instead on the data that are to be manipulated by the program. In comparison with function oriented design where executes by using structured analysis and structured design like a data flow diagram, the object oriented design is carried out using UML. 

Is useful because an entire system can be modeled by a single class diagram using object oriented desing. Class diagrams are the blueprint of the system. Class diagrams can become in a snapshot that describes exactly how a system works, the relationships between system components at many levels, and how is planned to implement those components.

Reference:
-  https://www.geeksforgeeks.org/difference-between-function-oriented-design-and-object-oriented-design/
- https://www.ibm.com/docs/en/rsm/7.5.0?topic=structure-class-diagrams


4. What are the **four pillars of object oriented programming**? Give a single-sentence description of each.
- **Abstraction**. Means displaying only the necessary information about the data to the outside world and hiding the background info or implementation.
- **Encapsulation**. Wrapping up data and information under a single unit. In OOP, is definde as binging totheter the data and the functions to manipulate them.
- **Inheritance**. Is the process in which two classes have a relationship with each other, and objects of one class acquire properties and features of the other class (parent and child classes)
- **Polymorphism**. It is the ability to take more than one form. It is a feature that provides a function or an operator with more than one definition

Reference: https://www.codingninjas.com/studio/library/four-pillars-of-oops#:~:text=The%20four%20pillars%20of%20OOPS%20are%20Inheritance%2C%20Polymorphism%2C%20Encapsulation%20and,objects%20with%20attributes%20and%20functions.


5. What is the **strategy pattern**? How would its implementation differ between a functional and object oriented system?

**Strategy pattern** is a behavioral design pattern that allows the behavior of an object to be selected at runtime. It is one of the Gang of Four (GoF) design patterns, which are widely used in object-oriented programming.

The Strategy pattern is based on the idea of encapsulating a family of algorithms into separate classes that implement a common interface. The pattern consists of three main components: the Context, the Strategy, and the Concrete Strategy.



6. Imagine your is creating a new online payment system. In order to gain maximum market share it can't be tied to a particular sector - it needs to work just as well when ordering a takeaway as when buying a new coat. Which design methodology would you suggest following? Give some justification for your decision.