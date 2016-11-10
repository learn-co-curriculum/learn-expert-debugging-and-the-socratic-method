# Debugging and the Socratic Method

![Socrates](http://www.dailystormer.com/wp-content/uploads/2014/01/socrates-statue2.jpg)

> “I cannot teach anybody anything. I can only make them think”
> ― Socrates

When you're working with student questions related to test errors, it's important that you first are able to look at the problem, deconstruct, and debug it. Once you do that, then you can transfer the same process (**process and not answer**) to students.

## Error Messages and the Lab

* Always ask students to show you the error message first. Read through it and be able to identify where and when the code is not working.
  - If the student doesn’t already understand, be sure to mention that error messages are great because they identify for you the exact reasons and location of why your program isn't working the way that you want it to. Error messages get you one step closer to solving the problem in front of you and they're specific.
* Now ask students to show you the code block that is relevant to the error message. Use the following debugging strategies to see if you can figure out what's happening. If you can't from the given code block, then ask them to show you the whole code.
* From reading the error message, can you tell what the correct expected behavior is and what the error is? Great.
  - If you’re not clear on the error AND solution from the error from the limited snippet, ask the student to push their code with `learn save` and give you the link to their repo so you can pull down the whole thing.
* Make sure that you understand all the steps necessary to solve this. What are the inputs and the outputs that need to be defined. This might mean that in addition to the student's code, you will also need to read the Readme of the lab first and make sure that you know holistically what's expected.
* Now break the problem of the lab into the smaller components necessary to solve it.

## Breaking Down Student Code

* When looking at each method, you should know what the method does, what the inputs are, and what the expected outputs are, as well as any edge cases. By decoding a student's code this way, you'll realize what went amiss and what the bug is.
  - For example, a good place to start debugging is to track the value of your variables. You may find that variables in the student's code don't hold the values that they expect, or that they don't hold any value at all. There are several ways to examine the values your variables hold (IRB, pry, console, debugger...).
* And if you have time, always run the student's code to make sure that your assumptions are correct. And then test the solution too to make sure that it works. In some cases there may be a totally different bug that you weren't aware of.
* If you get stuck and you’re not sure _what_ the bug is, you can compare the student’s code to the solution branch. (An easy way to do this is with `git diff master solution`).

## Socratic Method

You've probably heard the phrase [Socratic Method](http://www.criticalthinking.org/pages/socratic-teaching/606) but why do we care so much about it? The focus of the Socratic Method is on asking questions and not on giving answers. By asking specific, guided questions we get students to think critically about their responses, connect pieces of information together, and, in the process, learn how to learn.

Now that you know what the student’s bug is, help them figure out what the problem is without giving them the answer right away. Use questions that will get them to explain their process and in this way, they may realize themselves what their mistake was.
  - As a rule of thumb, in the text chats that you have with a student, they should be “talking” at least 50% of the time.

### Know when to start asking questions
* Do they understand the error message? What is it saying? Make them explain the error message to you.
* The student got an error message, but what did they _expect_ to happen?
* If a student’s error message is tied specifically to a method then start your questions with that method.
* However, if the student’s error message is related to issues outside of the specific method and there might be larger conceptual issues, you should start your questioning with those concepts.


### How to ask questions
* Use the same approach you took yourself when you were debugging the student’s code.
* Ask them to walk you through their code by breaking it into structured steps where they go operation by operation. If you need input data to talk through the code, direct them to whatever the test feeds in for this particular failing test.
* Ask the student what the purpose of their method is, what the inputs of the method are, and what they expected to be the result.
* When you get to the point of the student’s mistake, here are the strategies you can use to get the student to realize their own mistake.
  - Ask additional questions about why they thought this was correct such as “What do you think this line returns?” **Always ask them to try out the code in IRB, pry, console, or debugger.** We want students to get into the habit of using debugging tools.
  - Point the student to resources or tell them the specific things in a lesson or lab that they need to re-read.
  - Restate the student’s incorrect process or assumptions. Seeing it written out by someone else can give the student enough distance to see what their mistake was. “What does your_variable equal here?” and “What kind of object does method `#some_method` return?”
  - Use questions instead of statements. Sometimes, especially if a student is frustrated, it’s best to tell them what their mistake is. But phrase it as a question.
    - For example, instead of saying “Your method requires two arguments,” say instead “Don’t you think the method should require two arguments?” This way, the student will have to think for, even just a few seconds about their problem.

Using the Socratic Method will better teach students how to debug because it shows them what questions we ask ourselves when we solve the lab. In turn, this teaches students better debugging techniques so that they’ll have a better shot debugging their code on their own in the future.

* However if the student’s error message is related to issues outside of the specific method and there might be larger conceptual issues, then you should start your questioning with those concepts.


### How to ask questions
* Use the same approach you took yourself when you were debugging the student’s code
* Ask them to walk you through their code by breaking it into structured steps where they go operation by operation. If you need input data to talk through the code, direct them to whatever the test feeds in for this particular failing test.
* Ask the student what the purpose of their method is, what the inputs of the method are, and what they expected to be the result
* When you get to the point of the student’s mistake, here are the strategies you can use to get the student to realize their own mistake.
  - Ask additional questions about why they thought this was correct such as “What do you think this line returns?” **Always ask them to try out the code in IRB, pry, console, or debugger.** We want students to get into the habit of using debugging tools.
  - Point the student to resources or tell them the specific things in a lesson or lab that they need to re-read.
  - Restate the student’s incorrect process or assumptions. Seeing it written out by someone else can give the student enough distance to see what their mistake was. “What does your_variable equal here?” and “What kind of object does method `#some_method` return?”
  - Use questions instead of statements. Sometimes, especially if a student is frustrated, it’s best to tell them what their mistake is. But phrase it as a question.
    - For example, instead of saying “Your method requires two arguments,” say instead “Don’t you think the method should require two arguments?” This way, the student will have to think for, even just a few seconds about their problem.

Using the Socratic Method will better teach students how to debug because it shows them what questions we ask ourselves when we solve the lab. In turn, this teaches students better debugging techniques so that they’ll have a better shot debugging their code on their own in the future.
