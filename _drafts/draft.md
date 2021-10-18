---
layout: post
title:  "Title"
categories: 
---

Unit testing with Jest

I've been working on developing the classic game of Battleship in plain JavaScript. Part of the assignment (which you can read about here), is using Test-Driven Development (TDD) as a tool to write the code.

> ☝️ Write a test, write the code to pass the test.

The tests are meant to check whether functions are working correctly. For example, if I have a test like this:

`test("attack is a miss", () => {
  playerOneGameboard.receiveAttack("A1");
  expect(playerOneGameboard.array[0].missedShot).toBe(true);
});`

I can see if my code is working properly, without using `console.log`. 

The benefits of TDD are many, but the ones I've noticed the most in my own code are (1) improving design (tightly coupled vs loosely coupled!) and (2) encouraging refactoring. Plus, it's been (3) fun to write these simple tests and then make them pass.

And with a game like Battleship, there are many conditionals, and thus, many tests!



Array methods

findIndex and indexOf 



Having fun with APIs

I finished up a fun ☀️ [weather app](https://rusty-reebs.github.io/weather-app/) yesterday! I wrote asynchronous JavaScript functions as well as `fetch`, `await`, `try`, and `catch` to make it all work.

I decided to render the current date and time for the chosen location. This presented some challenges in plain JavaScript! 😅 I used the `Date` object and methods but it also required some additional math, processing, and manipulating! I'm really happy with how the whole app turned out, including the CSS styling. 🤩

Something that I'm finding more difficult as the projects get more complex is organizing my code. I'm currently reading *Clean Code* by Robert Martin for an online book club I'm in. I've already taken away lots of great tips that I'm incorporating into my code.

Tomorrow I'm diving into TDD -- Test Driven Development -- with Jest. ✌️


