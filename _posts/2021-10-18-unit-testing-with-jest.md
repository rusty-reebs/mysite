---
title:  "Unit testing with Jest"
categories: 
---

I've been working on developing the classic game of Battleship in plain JavaScript. Part of the assignment (which you can read about [here](https://www.theodinproject.com/paths/full-stack-javascript/courses/javascript/lessons/battleship)) is using Test-Driven Development (TDD) as a tool to write the code.

> ☝️ Write a test, write the code to pass the test.

The tests are meant to check whether functions are working correctly. For example, if I have a test like this:

~~~javascript
test("attack is a miss", () => {
  playerOneGameboard.receiveAttack("A1");
  expect(playerOneGameboard.array[0].missedShot).toBe(true);
});
~~~

I can see if my code is working properly, without using `console.log`. 

The benefits of TDD are many, but the ones I've noticed the most in my own code are (1) *improving design* (tightly coupled vs loosely coupled!) and (2) *encouraging refactoring*. Plus, it's been (3) *fun* to write these simple tests and then make them pass.

And with a game like Battleship, there are many conditionals, and thus, many tests!