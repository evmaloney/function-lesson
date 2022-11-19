# Functions
## Lesson Objectives
In this lesson, we will learn:
1. What is a function?
2. Why we use functions
3. How to write a function
4. The difference between declaring a function and calling a function
5. How and why we use parameters and arguments

## What is a function?
Functions are one of the essential building blocks of a program. They can be thought of as the verbs, or the "action" pieces of the code. Functions are designed to perform a specific task, or set of tasks, each time we run them. It is not always as explicit as this, but generally speaking, each time you click on a button on the screen, assuming it is a working button that actually performs a duty, it fires of a function. This function can potentially fire off other functions, and other functions, each with their own specific task that they are designed to perform. Now you might see a little more clearly why functions are considered a building block of programming.
Often times, a function can take in information (input), do its "task" (or "tasks") with that info, and send out an altered or new piece of information (output) to be used elsewhere.

(Algebra anyone?)

## Why we use functions
Let's think about a relatively simple use case of a function - getting the sales tax of an item. Let's say we wanted to get the sales tax of an item that is $10.00 and our tax rate is 7%. We could write a program where we write out the number 10 and multiply is by 0.07 to get our answer. Now let's say we have 100 items, all priced differently. Writing our program in this manner, we'd have to write out our program to multiply each of the items by 0.07, but do that that 100 times. Alright, maybe that will take some time by using some good old fashioned copy and pasting this wouldn't take us more than 5 minutes. Now let's say we have 1,000,000 items... I think you get my point. Alternatively, we could write out a function called getTax (always camel-cased in JavaScript) that takes in the price of any given item (input), multiplies it by 0.07, and returns (outputs) the tax on that item. This saves us the hassle of writing * 0.07 after every item. We can just send it the price and it sends us back the tax. This is called being DRY (Don't Repeat Yourself). We generally want to write as few lines of code as possible and so by doing this, we only have to write * 0.07 once.

## How to write a function
There are three ways to write a function in JavaScript, these being a Function Declaration, a Function Expression, and an Arrow Function. There are slight differences and different use cases between the three but often times, any will get the job done and it can come down to a stylistic preference. For now, we are going to focus on the Function Declaration. To write a Function Declaration, we need four things:
1. What it is - We need to tell JavaScript that this is a function and we do that by declaring it with the word "function".
2. A name - This is written in Camel Case and can be anything you want, but we generally want a name that describes what the function does. In our example above, our getTax function gets the tax of the priced item. There is also something called an Anonymous Function that doesn't take a name but that is for special cases that will be covered in a future lesson.
3. Parentheses. Depending on what our function does and information it needs, these can be either empty parentheses or have variables inside them (these  called 
