# Chapter 1: Commits and Pushes

So in Chapter 0 we read something about "Local" and "Remote" repositories. 

A **local** repository is the one on your machine, ideally it represents a mirror of the **remote** repository, which is the one everyone can access online.

So how do we do this?

To save our current changes we **commit** our files, and then we **push** them to a remote repository.

Let's try this out then.

In this chapter there is a python file, that contains an error, that I've tried to make obvious to you.

Using your text editor of choice open this file and fix it. If you're using vscode you should write `code .` in your terminal to open the folder to start editing

(If you're using a different text editor I'm assuming you know how to open it :P)

> "I've fixed the bug and saved my file. What now?"

Great! Now we are going to make a commit, and use the message to convey what we changed

In your terminal, write: `git commit -am "Fixed myfile.py"` 
(I'm aware that you can commit straight from some of these editors, but keeping to the tutorial will help you be able to do this from anywhere)

Now you might be wondering, why are we writing `-am` between the *commit* command and our message?

These are called flags, and in essence they add functionality to the command after them. In this case we are adding the flags `a` and `m`. These two flags signify that we want to add the changes to all tracked files (more on this in chapter 2), and that we want to add a message to our commit.

Unless you add these files manually, git will even remind you that you need to add these tracked files to the commit. Also making a commit with no message is pretty frowned upon, cause how are you going to be able to tell what you added with that commit otherwise?

You might also wonder: "Why do I need to say I want to add all my tracked files?". You'll come to see that being able to **selectively add files to your commit** is a superpower of its own for bigger projects.

Okay, enough waffling, its time for us to see our progress on our remote repo (github.com/...).

Provided your commit was successful, all you need to do now is:

`git push`

Now if you refresh the github repo, you'll see your changes, and anyone will be able to access them.

Now to go to Chapter 2 run the following command:
`git checkout Chapter2`


.


