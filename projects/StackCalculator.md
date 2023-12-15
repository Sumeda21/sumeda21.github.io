---
layout: project
type: project
image: img/white-calc.png
title: "Stack Calculator"
date: 2022
published: true
labels:
  - Java
summary: "A project I wrote for an ICS 211 assignment using a stack to create a calculator"
---

  <img width="400px" src="../img/Screenshot 2023-08-31 153006.png" alt="Stack calculator code" >


For my 211 introductory class, I was tasked with creating a very simple terminal calculator. For this calculator, numbers are inputted one by one, and if an operand is input, it will push the top two elements of the stack and apply the operand to them. I was the sole author of the code, and received no help from my TA or teacher, which helped me confirm that I truly understood the concepts needed to create this stack calculator. Although the calculator isn't nearly as advanced as a calculator can be, I liked this project as my previous project were more algorithm based, whereas this was one of the first data structure based project I worked on. As this calculator was implemented using a stack instead of an array, you can see how this is a great learning experience.

Alongside my new understanding of stacks (and linked lists), I also learned an important type of code - Code which checks if there is something is wrong. This was my first introduction to Exception and error handling where I wrote code within a try catch statement. Its quite important for coding when there are lines of code that could potentially break/stop the program, and so understanding how we can prevent crashes and allow the program to keep running or output an easier to read error message is vital to a seamless program.

Below is a snippet of code which shows the use of Exception handling in my stack calculator:
```
public void applyOperation(char operation) {
...
 try {
   under = stack.peek();}
   catch (EmptyStackException e) {
     stack.push(top);
     throw new EmptyStackException();
   }
...
```

Again, while this project isn't the most complex code you can write, in fact its probably one of the easiest, what makes this project so meaningful to me is the new concepts I learned. It was not just about learning about stacks and exception handling, but two new facets of programming. Algortihms and Data structures are a large part of coding, and this was my first dive into data structures, and exception/error handling was one of the first interface related topics I learned about. This project goes to show my devlopment as a software engineer and my ability to see past the obvious and delve deeper.

Source code for my project : <a href="https://github.com/Sumeda21/Projects/tree/main">https://github.com/Sumeda21/Projects/tree/main</a>
