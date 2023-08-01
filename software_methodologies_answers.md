# Software Design Methodologies

There are three principle design strategies used in software engineering:

- Structured design
- Function oriented design
- Object oriented design

Within each methodology there are various **design patterns** which provide further structure for us. In practice ***the language used for a project will likely be the last thing to be chosen***, determined by a combination of methodology and design pattern.

## Task

1. What do we mean by **coupling** and **cohesion** when discussing structured design?

Cohesion refers to what the class (or module) can do. There is two types of cohesion:

| Type | Description | Example
| ----------- | ----------- | -----------
Low cohesion | A class does a great variety of actions | STAFF 
checkEmail()
sendEmail()
emailValidate()
PrintLetter()

High cohesion | The class is focused on what it should be doing and have only methods relating to the intention of the class | ----------------------------
| Staff                   |
----------------------------
| -salary                 |
| -emailAddr              |
----------------------------
| setSalary(newSalary)    |
| getSalary()             |
| setEmailAddr(newEmail)  |
| getEmailAddr()          |
----------------------------







2. What is the difference between **top-down** and **bottom-up** design? Which best describes a function oriented design?
3. In which design methodology would a **class diagram** be most useful?
4. What are the **four pillars of object oriented programming**? Give a single-sentence description of each.
5. What is the **strategy pattern**? How would its implementation differ between a functional and object oriented system?
6. Imagine your is creating a new online payment system. In order to gain maximum market share it can't be tied to a particular sector - it needs to work just as well when ordering a takeaway as when buying a new coat. Which design methodology would you suggest following? Give some justification for your decision.