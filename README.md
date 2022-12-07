# JavaScript Functions
![](https://i0.wp.com/i.pinimg.com/originals/c6/4e/fc/c64efc9adaedbf446f328698e8b67388.jpg?resize=650,400)
![](https://www.meme-arsenal.com/memes/5c0b28a7cc04db2c07327b7f3fe81c1f.jpg)

## Learning Objectives
By the end of this lesson, we will be able to:
- Write a function
- Call a function
### Previous JavaScript knowledge that would be helpful:
- How to declare and initialize a variable
- How to console log

## Learning Objectives
In this lesson, we will learn:
1. What is a function?
2. Why we use functions
3. How to write and call a function

## What is a function?
Functions are one of the essential building blocks of a program. They can be thought of as the verbs, or the "action" pieces of the code. Functions are designed to perform a specific task, or set of tasks, each time we run them. A common example of a function being run on a website is when we click a button. Assuming this is a working button that actually performs a duty, this action will fire off a function that can potentially fire off other functions, and other functions, each with their own specific task that they are designed to perform.
Often times, a function can take in information (input), do its "task" (or "tasks") with that info, and send out an altered or new piece of information (output) to be used elsewhere.

(Algebra anyone?)

## Why we use functions
Let's think about a relatively simple use case of a function - pricing an item with sales tax included. Let's say we wanted to price an item that is $10.00 and our tax rate is 7%. We could simply type out the number 10 and multiply it by 1.07 and run our program to get our answer. But now, let's say we have hundreds of items, all priced differently. Writing our program in the same manner, we'd have to write out our program to multiply each of the items by 0.07, but do that that 100 times. Alternatively, we could create a function called getTax (always camel-cased in JavaScript) that takes in the price of any given item (input), multiplies it by 1.07, and returns (outputs) the tax on that item. This saves us the hassle of writing "* 0.07" after every item. We can just send it the price and it sends us back the price with tax included. This is called being DRY (Don't Repeat Yourself). We generally want to write as few lines of code as possible and so by doing this, we only have to write "* 0.07" once.

Before we continue, let's head over to https://replit.com/ to follow along with the next part of the lesson...
Create a Repl using Node.js as the language. Node.js is essentially JavaScript.
Give it a title of "Intro to Functions"
We will follow along with the steps in the next section by writing a function that simply console logs "Hello World"

## How to write a function
There are three ways to write a function in JavaScript, these being a Function Declaration, a Function Expression, and an Arrow Function. For now, we are going to focus on the Function Declaration. To write a Function Declaration, we need four things:
1. What it is - We need to tell JavaScript that this is a function and we do that by declaring it with the word "function".
2. A name - This is written in Camel Case and can be anything you want, but we generally want a name that describes what the function does. In our example above, our getTax function gets the tax of the priced item. There is also something called an Anonymous Function that doesn't take a name but that is for special cases that will be covered in a future lesson.
3. Parentheses - Depending on what our function does and information it needs, these can be either empty parentheses or have variables inside them called parameters. When we invoke/call a function (a.k.a. run the function), we can pass it information that it may need. This information is denoted inside the parentheses as a parameter that the function will use to perform it's specific task. Though the information being sent to the function may change each time it is invoked (think the different prices of items to get the tax of), the parameter name does not. With each price being sent to the function, the computer sets the price to that parameter name, like if it were called itemPrice, and multiplies it by 0.07. If the function does not need any information, no need for any parameters and they can be left empty.
4. Curly Brackets (or Curly Braces) - This is where all the function's... well... functionality goes. Everything that the function does, with any information it may given, is written inside of the brackets. This is where we'd write for instance, itemPrice * 0.07 and return it.

Before we continue, let's head over to https://replit.com/ to follow along with the next part of the lesson...
Create a Repl using Node.js as the language. Node.js is essentially JavaScript.
Give it a title of "Intro to Functions"

Let's start off with a classic Hello World example. Here are the steps we are going to take.
1. Declare the next block of code we are going to write as a function.
2. Give our function a name of sayHelloWorld.
3. Our function will not be taking any information in, so we will use empty parentheses.
4. Type out opening and closing curly brackets with a bit of code inside that just console logs "Hello World".

Now let's try to return "Hello World" rather than console logging it.

Now let's create a function called getSum that simply returns the sum of two numbers.

Now let's edit our getSum function to use parameters so we can dynamically change the numbers we want to add with each function call.

Now take 3 mins to write out a new function that executes our tax example from above. Be sure to use a descriptive function name and parameter. Remember to return and log your results.
