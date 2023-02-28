# Sprint Challenge - JavaScript Fundamentals

**Read these instructions carefully. Understand exactly what is expected _before_ starting this Sprint Challenge.**

This challenge allows you to practice the concepts and techniques learned over the past week and apply them in project. This Sprint explored JavaScript Fundamentals. During this Sprint, you studied array methods, this keyword, prototypes, and class syntax. In your challenge this week, you will demonstrate proficiency by completing a range of JavaScript problems.

This is an individual assessment. All work must be your own. Your challenge score is a measure of your ability to work independently using the material covered through this sprint. You need to demonstrate proficiency in the concepts and objectives introduced and practiced in preceding days.

You are not allowed to collaborate during the sprint challenge. 

## Introduction

The index.js file contains all of your challenges. Please review it in full before answering the questions. If you complete the stretch goals please leave them in your file but commented out so that they do not affect the MVP tasks. 

In meeting the minimum viable product (MVP) specifications listed below, you should have all tests passing. You can console.log to check your work and ensure you are submitting the correct results. 

### Commits

Set up codegrade early and commit your code regularly and meaningfully. 

## Interview Questions
### (please edit this file and write your answer below each question.)
Demonstrate your understanding of this week's concepts by answering the following free-form questions.

Edit this document to include your answers after each question. Make sure to leave a blank line above and below your answer so it is clear and easy to read.

1. Explain the differences between `.map`, `.reduce` and `.filter` and describe a use case for each. 

`.map` iterates over an array and returns a new array. As it iterates, it can perform functionality on each item of the array. The items will then be returned in the new array. It is frequently used to "do something" to each item, like multiply each item by 2 and return the resulting items in the new array.

`.filter` iterates over an array, passes each item through a boolean test, and returns a new array with the items that passed the test. It is frequently used for filtering an array of elements by a specific conditions to remove extraneous data.

`.reduce` iterates over an array and returns a single value. The syntax for `.reduce` is different from `.filter` and .`map` because it takes a reducer function with two values: an accumulator and a current value. The accumulator is what gets updated and returned from the reducer function. It is most frequently used to reshape large sets of data into a single value (e.g., averages or sums).

2. Explain the difference between a callback and a higher order function.

A higher order function is a function that receives a callback function as an argument or returns a function. Whereas, a callback function gets passed into a higher order function. 

3. Explain what a closure is.

A closure happens when information must be accessed that is outside of the current block or function scope. Through closure, Javascript can find this information in the lexical scope, or the context around function or block that has memory from where the information originated. The information in the lexical scope could be the value of a variable that was declared within an external function. Closure and scope allow functional programs to have complexity. Without closure, Javascript would not have access to information bound within an exterior function's scope.

4. Describe the four principles of the 'this' keyword.

a. Window/Global Binding: 'this' has no particular context and is looking for meaning within the global context (with node) or the window (with the browser). 

b. Implicit Binding: 'this' within an object refers to the context that was set before the '.' (dot) when a method is called. For example, teacher.teach() will implicitly bind the object teacher to any '.this' keyword used in the method of teach().

c. Explicit Binding: A function is given explicit directions for where to look for the context for "this". Explicit Binding is accomplished through the ".call", ".apply" or ".bind" method. ".call" and ".apply" will immediately invoke the function and pass in arguments either one by one with ".call" or in an array with ".apply". The ".bind" method does not immediately invoke the function, but returns a new function with ".this" bound to the object that can be called later.  

d. New Binding: This approach creates a copy of a new object from a starting object. The starting object feeds values into the new object when the function is invoked with the "new" keyword. The "this" inside of the constructor function refers to the specific instance of the starting object that was returned and created through the use of the "new" keyword.

5. Why do we need super() in an extended class?

Super() replaces the use of the Object.create syntax and passes any attributes of the child back up to the parent object's constructor. It enables the parent object's constructor to access the properties and methods of the child.

You are expected to be able to answer questions in these areas. Your responses contribute to your Sprint Challenge grade. 

## Instructions

### Task 1: Set up Project

Using VSCode and Command Line:


1. Fork the repo
2. Go into canvas and connect your repo to codegrade
3. Clone your forked version of the repo
4. DO NOT CREATE A BRANCH. You will be pushing your changes to the main/master today
5. cd into your repo
6. open the terminal in your vs code and type `npm install`
7. next type `npm run test` in your terminal
8. Complete your work making regular commits to main/master; your codegrade score will update each time you make a push.


### Testing & Debugging

Open a second terminal inside of your project by clicking on the split terminal icon
![alt text](assets/split_terminal.png "Split Terminal")

Inside of your second terminal type `npm start` 
![alt text](assets/npm_start.png "type npm start")

You will be running your tests in one terminal and debugging in the other. As you work on your code you should make use of `console.log` to check your progress and debug.
![alt text](assets/tests_debug_terminal_final.png "your terminal should look like this")

### Task 2: Project Requirements (MVP)

You must complete all tasks inside of `index.js` and answer the questions above.

In your solutions, it is essential that you follow best practices and produce clean and professional results. Schedule time to review, refine, and assess your work and perform basic professional polishing including spell-checking and grammar-checking on your work. It is better to submit a challenge that meets MVP than one that attempts too much and does not.

## Resources
 
 [Sprint Challenge Study Guide](https://www.notion.so/bloomtech/Unit-1-Sprint-3-Study-Guide-033a9a00659a4ef98c12eb97e49a6110)

## Submission format

Please submit your project via codegrade by following [these instructions](https://bloomtech.notion.site/bloomtech/BloomTech-Git-Flow-Step-by-step-269f68ae3bf64eb689a8328715a179f9) (see part 2, submitting an assignment with codegrade).
