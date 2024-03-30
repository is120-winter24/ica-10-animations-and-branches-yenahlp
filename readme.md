[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-24ddc0f5d75046c5622901739e7c5dd533143b0c8e959d652212380cedb1ea36.svg)](https://classroom.github.com/a/QIwIzeNT)
# Introduction
Welcome to In-Class Activity number 10! In this activity we are going to learn about CSS Animations and Git Branching, Merging, and Pull Requests!

This activity is designed to be completed with a partner. You will be working together to complete a set of tasks that will require you to use CSS animations and transitions to create a dynamic webpage. You will also need to use Git to create branches, make changes, and merge those changes back into the master branch.

## Set Up Instructions
Before you add any code, you will need to do the following tasks with your partner:
1. Designate one person to be the repository owner and the other to be the collaborator. Whoever is the repository owner will accept the GitHub Classroom assignment, and add the collaborator to the repository in the repository settings on GitHub.
2. Both the repository owner and the collaborator will need to clone the repository to their local machine.
3. Read through the task list and split up the six required tasks between the two of you, so that each person should complete three tasks. The tasks are listed in the task list below. One person should complete their tasks in the `ica10-branch1.html` and `ica10-branch1.css` files, while the other person should complete their tasks in the `ica10-branch2.html` and `ica10-branch2.css` files. These files are already created in the repository and are stored in folders named similarly to the files.
4. Both the repository owner and the collaborator should create a new branch for their set of tasks that they are responsible for. Name your branches by your names, so that it is clear who is responsible for which tasks.
5. Add your names and the tasks complete somewhere on your respective pages so that it is clear who completed which tasks. This name can be in the provided HTML comments at the top of each `ica10-branch#.html` file.

> [!TIP] 
> It would be wise to brainstorm with your partner how to accomplish all of the tasks before you start coding. This will help you to be more efficient and to avoid any potential conflicts when merging your changes back into the master branch.

## Task List
### 1. Animate a logo in the header of the page.
Add a logo to the header of either page. Have the logo get bigger and slighty rotate when hovered over.
> [!TIP]
> Remember that the `transition` property can be given multiple values to transition multiple properties at once: like `transition: width 2s, height 2s, translate(3px, 5px) 2s;`

### 2. Highlight a dynamic quote in a box in the grid.
Insert a quote in any of the boxes, and create a `background-image` of a gradient that only has a `background-size` representative of an underline. The underline should grow along the bottom of the text on hover.
> [!TIP]
> I *highly* recommend watching this short tutorial on this, as it'll take you through the steps. [Watch Here](https://youtu.be/_1vEGYWaaQY?si=BkrLWJVMbVt1qlbD)

### 3. Change the position of any square in the grid continually.
Have the position of any square in the CSS grid change continuously by set parameters. There are many ways to go about this (think of order, align-self, or others), but I would definitely recommend changing the `grid-column` or `grid-row` properties through `@keyframes`.

### 4. Highlight a notification on the page.
Have a notification scroll in from anywhere offscreen on a set interval. In my example, I have a notification that scrolls in from the bottom right corner of the page every 10 seconds.
> [!TIP]
> It would be extrememly beneficial to think through this task before you start coding. Start by asking yourself, "how can I make an element be positioned offscreen?" and "how can I make an element move from offscreen to onscreen?"

### 5. Have a square with a linear gradient background-image change on hover.
Now this is a fun one. Have a square in the grid with a `background-image` of a linear gradient. When hovered over, the gradient should change to a different gradient.
> [!TIP]
> The easiest way to do this is to have only one gradient set in the selector before the hover event. Then, during the hover, trigger an infinite, linear animation. Your `@keyframes` should have two states, where the property value pair of `filter: hue-rotate();` is set. Think of this like a color wheel, where your start will be `0deg` and the end will be `360deg`!

### 6. Make the circular text in one of the squares in the grid rotate continuously.
I provided an svg with a specific `textPath` that's been hard coded into the HTML. First, fill in whatever text content you would like in the `textPath`. You'll need to make the text rotate continuously around the circle, which you can do by just rotating the entire `svg`.

## Submission
When you have completed your tasks, you will need to create a pull request to merge your changes back into the master branch. Each partner should create a pull request for their set of tasks, and the other partner should review the pull request and approve the changes or request more changes if needed. Once all changes are merged, you will be done with the activity! Ensure that everything has pushed to GitHub correctly and that the changes are visible on the GitHub repository.

## Example Code
I will provide an example website showcasing some of the tasks that you will be completing so you can get an idea of what the final product should look like. You can find the example code [at this website](https://ckearl.github.io/ica10-example/).

## Lecture Resources
If you need resources to help you complete the tasks, the content for the lecture slides from this week can be found in the `lecture-resources` folder in the repository. You can find information on CSS animations and transitions in the `animation-slides.md` file and information on Git branching, merging, and pull requests in the `github-slides.md` file.

## A note on editing and your styling decisions
You may edit the CSS of the `template.css` file, but just know that it will effect both the `ica10-branch1.html` and `ica10-branch2.html` files. I would take a moment to study the structure of the code that's going on. You'll notice that I've set up a CSS grid with a few different classes. You can use these classes to style the elements in the grid. You can also add new classes if you need to.

If you feel inclined, you and your teammate can accomplish the six tasks in any way you'd like, I just provided a template that made an approachable canvas for us to learn about more GitHub functions and CSS Animations. You can add new elements, change the structure of the grid, or anything else you'd like to do.