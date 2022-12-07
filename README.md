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
4. The 'return' statement

### 1. What is a function?
- Functions are one of the essential building blocks of a program 
- Think of them as the verbs, or the "action" pieces of the code
- Designed to perform a specific task each time we run them 
A common example of a function being run on a website is when we click a button. The action of that click will fire off a function that can potentially fire off other functions, and other functions, each with their own specific task that they are designed to perform.
Often times, a function's purpose is to take in information (input), perform its "task" with that info, and return an altered piece of information (output) to be used elsewhere.

(Algebra anyone?)

### 2. Why we use functions
Functions let us:
- Break our code down into smaller tasks
- Stay organized
- Run code without having to rewrite it. This allows us to be 'DRY' (Don't Repeat Yourself)
Let's say we needed to write a program where we price out several items with a tax rate of 7% included. Rather than separately multiply each item's price by 1.07, we could write a function that takes in the price of an item, performs this calculation on it, and sends it back to us. Each time we need the price plus tax of a new item, we just need to send it to the function.

Before we continue, let's head over to [replit.com](https://replit.com/) to follow along with the next part of the lesson...
- Create a Repl using Node.js as the language.
- Give it a title of "Intro to Functions"
We will follow along with the steps in the next section by writing a function that simply console logs "Hello World"

## 3. How to write a function
There are three ways to write a function in JavaScript, these being a Function Declaration, a Function Expression, and an Arrow Function. For now, we are going to focus on the Function Declaration. To write a Function Declaration, we need four things:
1. What it is 
  - We need to tell JavaScript that this is a function and we do that by declaring it with the word "function".
2. A name - This is the name of our choosing that we give to our function that describes what the function does. In our example above, our getTax function gets the tax of the priced item.
4. Parentheses - Depending on what our function does and information it needs, these can be either empty parentheses or have variables inside them called parameters. When we invoke/call a function (a.k.a. run the function), we can pass it information that it may need. This information is denoted inside the parentheses as a parameter that the function will use to perform it's specific task. Though the information being sent to the function may change each time it is invoked (think the different prices of items to get the tax of), the parameter name does not. With each price being sent to the function, the computer sets the price to that parameter name, like if it were called itemPrice, and multiplies it by 0.07. If the function does not need any information, no need for any parameters and they can be left empty.
5. Curly Brackets (or Curly Braces) - This is where all the function's... well... functionality goes. Everything that the function does, with any information it may given, is written inside of the brackets. This is where we'd write for instance, itemPrice * 0.07 and return it.

Now let's try to return "Hello World" rather than console logging it.

Now let's create a function called getSum that simply returns the sum of two numbers.

Now let's edit our getSum function to use parameters so we can dynamically change the numbers we want to add with each function call.

Now take 3 mins to write out a new function that executes our tax example from above. Be sure to use a descriptive function name and parameter. Remember to return and log your results.
