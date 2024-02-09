# Chapter 2: Adding & Group Work on git 
## Git Add
Sometimes for your project you want to add new files that didnt exist before.
Git by default will only look at the files it knows to look (tracked files) for when using `git commit -am"

This means that if we're adding a new file that doesnt exist in our repo already, it will be "untracked" and therefore we need to **add** it ourselves to our commit.

The way we do this is by using `git add path/to/file.txt` for a single file (path is from the root of the repo) or more commonly using `git add *` to add **all** untracked files.
After this we commit like normal.

So lets do this, in your terminal run:
`touch newfile.txt` This simple command just makes a new file called `newfile.txt`

Now we use what we just learnt.

Use add, commit, and push to get this new file onto your remote repo.
.
If you're successful your repo should look like this:

![image](https://github.com/StefVuck/gitgood-Git-Tutorial/assets/142335830/7c7f8e02-5ce9-4fae-a75b-c5062a638555)

As you can see, we successfully added a new file created locally to our remote repo.

## Group Work & git pull
Question: What happens to your repo if someone in your coding group pushes their code to the remote repo?
Answer: Nothing

Again, git is made to be efficient, and if it was constantly scanning your remote repository that would ruin it. 
But the question is valid, and you do need to keep your local repo up to date with the remote one to avoid code conflicts.

The way you solve this is with `git pull`

Just in the same way that you **PUSH** code from your machine to the remote repo, you **PULL** code from the remote repo to your machine. Makes sense right?

It's probably a hassle to get someone else to help you here so here's what you'll do:

On the github website:

Beside the big code button, theres a **Add File** button, feel free to add what you want here, or just make a new file with the github editor.

This acts as our update on the remote repo.

Now back in git bash/terminal, run:
`git pull`

You should notice some files being added here.
If the files been added correctly run `git checkout Chapter3` to start Chapter 3.
