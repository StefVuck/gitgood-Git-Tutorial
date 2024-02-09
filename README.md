# gitgood-Git-Tutorial
Beginners Tutorial for Git and Version Control

If you're convinced and you're just looking for the tutorial, skip to : [[#Tutorial Start: Chapter 0]]

## Why use Git?
Especially for smaller scale projects, its easy to scoff at the extra "complexity" of learning git, and using GitHub (or similar tools), however git is an essential tool to learn for any form of coding, heres why:

**Source Code Should Always Work**

I understand this may not seem obvious, but the source code (or what will typically be "main" or "master" for your git repos), are something you should always protect. If you're making code to be used somewhere, you **never** want to be in a position where someone has "broken" your code, and you're no longer able to use your functional code. So how does git tackle this?

Two Core Ideas:
- Version Control
- Branching

**Idea 1: Version Control**
Have you ever been editing a document and made a mistake and quickly rushed to press `Ctrl+Z` to undo your mistake?
What happens if you write code, save it, and close your editor? **No More Undo**
>"Well I wouldn't do that"

I too like to think I'm an amazing developer who is incapable of making mistakes, but somethings that compile, may break something else, and thats not exactly ideal.

**The Solution? Version Control**

Imagine being able to use your Ctrl+Z for every change you have **ever** made on a document, not just that, but **any** change, that **anyone** has made on any document in your project?
Not just that, you can see every change (difference) between each "save" that happens, allowing you to precisely pinpoint what code, developed by who has broken your working project.

No need to imagine, that's what Version Control provides.

**Idea 2: Branching**
Now given what I said about protecting our source code, you might ask:
> "If I'm meant to keep my git repo up to date with my changes, how do I make sure my source code always works? I can't make sure every save provides functional code"

This is a perfect point, and leads us to the beauty of branching:

If you want to develop something new, from already functional code, you create a branch, develop on that branch and then when what you've developed works as intended, you **merge** it back into main.

*What does this mean?* 

At any point if you need, you can take the code from main, being sure that it works correctly. You can also regularly "save" (commit) changes to your development branch, allowing you to save your progress before the new feature is done.

Think of it sort of like this:

![image](https://github.com/StefVuck/gitgood-Git-Tutorial/assets/142335830/d1ff4ec1-3fcd-4022-b337-18d0ca8f26a5)

`Source: https://www.abtasty.com/blog/git-branching-strategies/  under trunk-based.`


You can see, no matter what is happening on the two branches, we can always be sure that our source code (master) has functional codes, as we only merge the features in once they are done and working.


## Tutorial Start: Chapter 0
Typically, when working on a git repo, it will either be your own, or one that you already have permission for.

Unfortunately this is currently not the case, so you'll have to "fork" this repository, making a working copy under your name.

Provided you're on the main page for this repo: [Original Repo](github.com/StefVuck/gitgood-Git-Tutorial) , you should be able to see this bar at the top of the page:

![image](https://github.com/StefVuck/gitgood-Git-Tutorial/assets/142335830/d1e78623-821d-4ee9-b84f-c5fd93bd6cd3)

As you might guess by the massive red arrow, I want you to click that button to fork this repo  Optional: Star the repo too please :) 

GitHub will now take you to a screen like this:

![image](https://github.com/StefVuck/gitgood-Git-Tutorial/assets/142335830/e58650c8-7575-4b40-b985-46f51e082c98)

Before you proceed, it's essential that you **UNCHECK THE BOX THAT SAYS `Copy the main branch only`**, this tutorial simply won't work otherwise.
Once you've unchecked the box, go ahead and *Create Fork*

Now you should see a simliar looking repository, under your name!

Here's the *scary* part, windows users, I want you to download [Git Bash](https://gitforwindows.org/). Linux/Mac User? Okay: [Linux/Unix Install](https://git-scm.com/download/linux)
Now, I have a dual boot set up, but I'll be using Git Bash on windows, so Mac and Linux users, it may *look* different but it'll work the same.

> "I thought you said this was simple, I don't know how to use a Terminal/CLI !!"

Rest assured, I get terminals and such are potentially intimidating, but what we're doing is pretty simple.

Now first go back to your repository (the thing you just forked), and look for the **big green button** that says code. It should be close to where you forked.

When you press this button you should see something similar to this:

![image](https://github.com/StefVuck/gitgood-Git-Tutorial/assets/142335830/8207d3a5-5e5e-4d45-b4e0-22f7bf618363)

Provided it is on the https tab, you should copy this to your clipboard with the button beside the link.

Now open gitbash (or some other terminal):

You'll see something like this:

![image](https://github.com/StefVuck/gitgood-Git-Tutorial/assets/142335830/44ac13b1-5f46-4b0d-8065-78158e53a2ca)

This is pointing towards a folder currently, that you can see at the top of the tab.
Now you want to pick a place that you want to put this project.

> "How do I get there?"

This is the only terminal scripting beyond git you will do, but its important to know these basic commands in your shell:
- `cd` : This lets you "change directory" or folder, this is what you'll use most.
   -  You can either go from where you are: `cd University/gitTutorial/`
   -  You can also just copy the full file path from file explorer: `cd "C:\Users\stefv\University\gitTutorial"`
       -  Just be very careful, you can't directly `Ctrl+V` into here, you need to right click and paste (or use `Shift + Ins` if you're cool like that)
   - You can go to the folder above using `cd ..`
     
- `mkdir` : make directory (folder) does what it says on the tin, makes a folder with the name following the command in the current location
- `ls` : list, it lists all the folders and files in your current folder. Can be super useful
- `pwd` : print working directory (folder) : prints your current location

Now with this knowledge, I want you to navigate to the folder you want to put this project in (keeping in mind this makes an extra folder in here).

Do you still have the link copied from earlier? I hope so. You're going to write `git clone ` then right click to paste in the link. It should look like this:

![image](https://github.com/StefVuck/gitgood-Git-Tutorial/assets/142335830/457ec681-60a9-46bc-8346-9fcfd34bb0b0)

Obviously it will have your github username instead of StefVuck as well.

Now just press enter:

This should load and start "cloning" the remote (online) repo into your local files. 
One more command quickly:

`cd gitgood-Git-Tutorial` ps: you can press tab to autofill the directory name

You should now be in a working git repo, you can tell by seeing a little indicator of what branch you are on:

![image](https://github.com/StefVuck/gitgood-Git-Tutorial/assets/142335830/5eadfca5-ab8c-4f27-ac33-4cfc8cf443be)

So we've forked the repository and cloned it locally, we can start working!

**TO ACCESS CHAPTER 1:**

In your terminal write `git checkout Chapter1`, and read the readme on that new branch, you can also do this on the git website.

Hint:

![image](https://github.com/StefVuck/gitgood-Git-Tutorial/assets/142335830/606122d1-d4b3-46e1-9caa-5b1f7aec0c69)







