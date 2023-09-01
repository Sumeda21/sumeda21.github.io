---
layout: project
type: project
image: img/micromouse/micromouse-square.jpg
title: "Stack Calculator"
date: 2022
published: true
labels:
  - Java
summary: "A project I wrote for an ICS 211 assisngment using a stack to create a calculator"
---

<div class="text-center p-4">
  <img width="200px" src="../img/micromouse/micromouse-robot.png" class="img-thumbnail" >
  <img width="200px" src="../img/micromouse/micromouse-robot-2.jpg" class="img-thumbnail" >
  <img width="200px" src="../img/micromouse/micromouse-circuit.png" class="img-thumbnail" >
</div>

In this project I implemented is a stack which functioned as a calculator. Numbers are inputted one by one, and if an operand is input, it is operated on the top 2 numbers in the stack. I wrote and implemented all of the code for the Stack calculator. Although the calculator isn't as advanced as it can be, the use of stacks as well as the use of code which catches edge cases helps to show my development in coding.

Alongside this project, I coded a stack with both Linked Lists and Arrays, building on my knowledge and understanding of stacks. In addition, I learned how to catch, handle and throw exceptions, all which make the code alot more bug proof. It made me become more aware of all possibilities, making sure that there are no cracks in the code which could potentially cause the program to crash. 

An line of code which shows the use of Exception handling:
```
public void applyOperation(char operation) {
 Double top = stack.pop();
 Double under = 0.0;
 try {
   under = stack.peek();}
   catch (EmptyStackException e) {
     stack.push(top);
     throw new EmptyStackException();
   }
 under = stack.pop();
 Double result = 0.0; 
 switch (operation) {
   case '+' : result = under + top; break;
   case '-' : result = under - top; break;
   case '*' : result = under * top; break;
   case '/' : result = under / top; break;
   default : throw new IllegalArgumentException("");
 }```

Source code for my project : https://github.com/Sumeda21/Projects/tree/main
