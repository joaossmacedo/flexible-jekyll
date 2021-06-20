---
layout: post
title: Input Componentization
date: 2020-05-27 00:00:00 +0300
description: You’ll find this post in your `_posts` directory. Go ahead and edit it and re-build the site to see your changes. # Add post description (optional)
img: # workflow.jpg # Add image post (optional)
fig-caption: # Add figcaption (optional)
tags: [Software Devlopment, Web Development, Angular, Ionic] # add tag
---
During my time as a software developer I've faced several issues that I found annoying, the most annoying being the need to replicate both behaviour and design changes in projects with lots of inputs. That can be partially solved with good pratices, however this repository makes it even easier as you can create inputs with predefined behaviours with a simple line.

## What is the objective of the project?
Create an input component that receive values such as type, placeholder and initialValue, creates an input field based on those parameters and then return the value and errors whenever there is a change on the field.

![Input Component Logic](../assets/img/input/InputComponent.png)

## Why should I use this concept?
1. Maintainability and reuse  
Since all the code regarding inputs is in the same place it's much easier to maintain and edit your code. One change affects the whole code. This way it is much easier to fix bugs and you ensure that once a bug is fixed the same bug won't pop out elsewhere(if you repeat the type of an input a lot it's pretty common to forget to fix the bug somewhere).

2. Low coupling  
As long as you always return the value of the input and which errors it contain, doesn't matter how you implement it. Suppose you are using Ionic w/ Angular and you want to change from ion-input to mat-input, if you are using this concept you only need to make a single change.

## When should I use this concept?
1. Big projects;
2. Medium/small project with a high number of inputs.

## When should I not use this concept?
1. Medium/small project with a low number of inputs.

## How to see a demo of this project?
1. Clone the repository;
2. Go to the folder cloned;
3. Open either the 'angular' or the 'ionic' folder;
4. Run 'npm install'.

#### If you selected 'angular'
3. Run 'ng serve';
4. Open 'localhost:4200' at your browser.

#### If you selected 'ionic'
3. Run 'ionic serve';
4. Open 'localhost:8100' at your browser.
