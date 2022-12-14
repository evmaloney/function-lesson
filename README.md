# JavaScript Functions

## Learning Objectives
By the end of this lesson, we will be able to:
- Write a function
- Call a function
### Previous JavaScript knowledge that would be helpful:
- How to declare and initialize a variable
- How to log something to the console 
- Mathematical operations

![](https://pbs.twimg.com/media/FAULatTXsAINYzo.jpg)

## Road Map
In this lesson, we will learn:
1. What is a function?
2. Why we use functions
3. How to write a function
4. How to call a function
5. The return statement
6. Parameters and arguments

### 1. What is a function?
- Functions are one of the essential building blocks of a program
- Think of them as the verbs, or the *"action"* pieces of the code
- Designed to perform a specific task each time we run them 

A common example of a function being run on a website is when we click a button. The action of that click will fire off a function that can potentially fire off other functions, and other functions, each with their own specific task that they are designed to perform.

Often times, a function's purpose is to take in information *(input)*, perform its "task" with that info, and return an altered piece of information *(output)* to be used elsewhere.

***Algebra anyone?***

### 2. Why we use functions
Functions let us:
- Break our code down into smaller tasks
- Stay organized
- Run code without having to rewrite it. This allows us to be ***'DRY' (Don't Repeat Yourself)*** and write less code.
- Build dynamic programs by allowing us to change inputs

Let's say we were writing a program where we needed to get the tax on several separate items at a rate of 7%. Rather than separately multiply each item's price by 0.07, we could write a function that takes in the price of an item, performs this calculation on it, and sends it back to us. Each time we need the tax amount of an item, we just need to send its price to the function.

#### 🛑 Questions so far???

---
Before we continue, let's head over to [replit.com](https://replit.com/) to follow along with the next part of the lesson...
- Create a Repl using Node.js as the language.
- Give it a title of "Intro to Functions"

We will follow along with the steps in the next section by writing a function that simply console logs *"Hello World"*

---

### 3. How to write a function
There are three ways to write a function in JavaScript, these being a ***Function Declaration***, a ***Function Expression***, and an ***Arrow Function***. For now, we are going to focus on the Function Declaration. To write a Function Declaration, we need four things:
#### 1. What it is 
  - We need to tell JavaScript that this is a function and we do that by declaring it with the word ```function```.
#### 2. A name
  - This is a descriptive name of our choosing that we give to our function. A good name for our function in our example above that calculates tax could be ```getTax```
#### 3. Parentheses
  - If our function does not need any input, the parentheses are empty
  - If our function does take one or more inputs, there will be variables inside the parentheses that our function will use. We call these variables ***parameters***
#### 4. Curly Brackets (or Curly Braces)
  - This is where all the function's... well... functionality goes. Everything that the function *does*, with any information it may be given, is written inside of the brackets. In our tax example above, this would be where we multiply our ```itemPrice``` by ```0.07``` and return it.

### 4. How to call a function
Luckily, calling a function is the easiest part of a function. Unfortunately, forgetting to call a function is going to be a source of major headaches of your careers. Normally, and in other languages this is a must, a function is called **below** its declaration. In JavaScript and with *function declarations* in particular, we may call them anywhere.

To call a function, all we need is simply the name of the function and a pair of parentheses.
- If you don't need to send an input to the function, these parentheses are empty
- If you do need to send one or more inputs, we just fill the parentheses with the input(s), separated by commas if there are more then one. We call these ***arguments***.

### 5. The return statement
Though most people wait until after the holidays to return their gifts, we programmers enjoy returning things year round 🤓

**laughter, applause, standing ovation,** ***"thank you, you may be seated!"***

The ```return``` statement allows us to *output* a single piece of information. In our tax example, we'd be returning the tax on that particular item.

To return something, all we'd do is put ```return``` in front of whatever we want to output from the function.

- **Let's edit our function to return "Hello World" rather than console logging it.**

#### 🛑 Questions so far???

---
### 6. Parameters and arguments
We spoke briefly about paramters and arguments - here's a quick recap:
- When we call our function and want to send it information, we put our ***arguments*** inside of the parentheses. These are often strings or integers.
- When we want to input those arguments into our function, we give them ***parameters*** in our function's parentheses that will represent the values of the arguments that were sent in. Much like our function name, the name of each parameter should be descriptive and camel-cased.

***!!!Please not that the order or these matter - the first parameter will represent the value of the first argument!!!***

Sample:
```js
function getSum(num1, num2) {
  const sum = num1 + num2;
  return sum;
}

getSum(8, 6)
// => returns 14
```

- **Now's your turn! Take ⏱ 2 mins to write out a new function that executes our tax example from above. Be sure to use a descriptive function name and parameter. Remember to return and log your results.

---
---

## More info ##
#### Function Expression
```js
const getArea = function(num1, num2) {
  const area = num1 * num2;
  return area;
}

getArea(8, 6)
```
#### Arrow function
```js
const getSquare = (num) => {
  const square = num * num;
  return square;
}

getSquare(5)
```
Alternative one liner of arrow function. This automatically return what comes after the arrow.
```js
const getSquare = (num) => num * num;

getSquare(5)
```
