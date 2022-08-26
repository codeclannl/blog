+++
title = "Why You Should Start Pair Programming Tomorrow"
description = "Why You Should Start Pair Programming Tomorrow"
date = "2022-08-26"
tags = ["pair-programming"]
author = "Ruben Scheedler"
+++
Software developers are expensive. Managers or product owners are always struggling to account for every hour that we as programmers work. Why then would they ever agree to let half of their developers simply watch others? Because in many cases **it saves more time than it costs.**

## What is Pair Programming
First of all, there is no one way of pair programming. [martinFowler.com](https://martinfowler.com/articles/on-pair-programming.html#HowToPair) gives a nice overview of some common styles. In this article, I will use the following definition for pair programming:

> Working on a single story with more than one developer

The key takeaway of this definition is that you don't have to work on a single machine all the time. Everything from occasional sparring to constantly sharing a keyboard is in some form of pair programming. 

In the sections below I will discuss some forms of pair programming and their added value.

## The Kickoff
By a **kickoff**, I mean a gettogether of two or more developers to discuss the technical solution to a story or task in advance. It is one of the simplest forms of pair programming, but it can nonetheless be of great value. 

The kickoff derives its value from avoiding technical implementations that later require refactoring. In other words: from limiting technical debt. Technical debt (TD), like regular debt, requires resolving (refactoring). Up till then, interest in some form is paid. Without going into much detail on TD know that avoiding it saves a lot of time in the future.

Avoiding TD in a story often means **forgetting as little as possible**. Although team members share a good portion of their knowledge, every member has unique insights. Person A might tend to forget scalability, but person B always considers this first. He however tends to have a blind spot for security. Person C might know an existing library, which would immensely reduce implementation time, etcetera. This gives rise to the diagram below:

![Kickoff and technical debt (1).png::img-medium](https://cdn.hashnode.com/res/hashnode/image/upload/v1650275562817/uZE6rehZt.png)

Instead of trying to come up with all the forces, problems, and potential solutions for a story yourself, join forces with a colleague. You can discuss things in advance so you don't have to rework things later. 

## Developing Together
Once the story's desired implementation is clear it is time to start coding. This is also the time you can choose to do traditional pair programming. One developer writes (the *writer*) and the other reads along (the *reader*). For this style to work it is very important that the reader *does not get distracted*. This is because the reader is in a special position. The writer has to focus on typing, syntax, and other low-level decision-making where the reader can zoom out. They can look back, look ahead and look around. For the reader it is easier to see possible refactorings, emerging patterns, emerging code duplication, etcetera. All these ideas that the reader might come up with can be implemented *during* the development instead of being suggested *after* the story at the code review. At that time, major refactoring might be required which makes it tempting to just "let things be" (enter more technical debt).

## Debugging Together

![rubber duck.jpg::img-medium](https://cdn.hashnode.com/res/hashnode/image/upload/v1650280129930/WC-zAfHs9.jpg)
Debugging can be a very time-consuming matter which can be limited by pair programming. Just the practice of **rubber duckying** can help solve problems. Walking through code with someone that has a fresh perspective often identifies problems much faster, because they have no bias toward your implementation. Finally debugging the same problem in parallel can be fruitful when you are dealing with complex bugs. 

Complex bugs are like escape rooms. To solve an escape room, a series of insights is required. Person A might find the first puzzle solution very quickly but blank on the second puzzle. This is where person B comes in with a different perspective, solving the second puzzle. Then person A immediately sees what needs to be done for puzzle three, etcetera. This shows that **working together can immensely speed up the process of solving complex problems**.

## Code Ownership and Mentoring
All forms of pair programming have the additional benefit of **distributing knowledge**. Pair programming distributes code ownership because more people are familiar with the code that was written. Moreover, team members automatically learn each other's development methods. Maybe you see your colleague use a shortcut or plugin you did not know existed, maybe they work test-first, or you get an insight into how other developers debug certain problems that are way less cumbersome than your own methods. All this increases the long-term productivity of the involved developers.

## When not to Pair Program
Pair programming is not a silver bullet. There are stories and tasks that are less suited for pair programming. These stories are simple stories that all team members know how to complete and would typically use the same solution to do so. Barely any knowledge transfer would occur during these stories and the reader of the pair would have little to no benefit from his perspective. Some examples of tasks where I would choose not to pair program would be

- Changing a well-known configuration property or text constants
- Writing unit tests for simple code (with little logic)
- Implementations that are repetitive from the team's perspective (everyone has done them many times)

## Conclusion
Pair programming is an undervalued practice that can have long-term and short-term benefits for developers and their companies. When next you want to convince your supervisor that pair programming is worth it, remember that pair programming:
 
1. Reduces technical debt accumulation, saving time in the future
2. Can drastically reduce debugging effort 
3. Lets developers learn from eachother
4. Spreads knowledge across team members
5. Does **not** mean permanently working on one machine

When applied at the right time, pair programming will bring your development team to the next level, so pair up!