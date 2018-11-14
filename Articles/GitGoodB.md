* * *

# GIT Good: A Practical Introduction to GIT and GitHub (In GIT we trust!)

![](https://cdn-images-1.medium.com/max/2000/0*3iJLQaoQI66YJuQk.jpg)

**This is a two part series on GIT and GitHub,**
[GIT-Good Part-A: Hello GitHub](https://codeburst.io/git-good-part-a-e0d826286a2a) 
 → GIT-Good Part-B: In Git we trust! 
You are currently reading the **part B**.

> “Using Version Control is a basic necessity for the developers today and every developer is expected to have the knowledge(at least the basics) of any VCS. By far, the most widely used modern version control system in the world today is GIT. GIT and GitHub has made the life of developers so much easier that simply thanking them won’t be enough.”

### What did we study in the last article?

In the last article we had a look at basics of GIT and GitHub. We had an in depth look at GitHub and went through the basic terms and terminologies associated with version control systems. We made an account on GitHub, and created our first repository. Also, we learnt the importance of using VCS. We downloaded GIT on our desktop and and setup the SSH key for GitHub.
In case you missed out the [last article](https://codeburst.io/git-good-a-practical-introduction-to-git-and-github-hello-github-e0d826286a2a), do give it a read before proceeding further. This article will be covering the CLI commands required to work with GIT and GitHub.
Let’s get started…

### Configure Tooling

Before getting into the repositories and all, we first need to configure user information for all the local repositories. Follow along :)

![](https://cdn-images-1.medium.com/max/1600/1*_UBVwbIz-C0_x60O8WlWbg.gif)No, I’m gitticus!

<pre name="787a" id="787a" class="graf graf--pre graf-after--figure">$ git config --global user.name "[name]"
$ git config --global user.email "[email address]"
$ git config --global color.ui auto</pre>

> user.name — Sets the name you want attached to your commit transactions
> user.email — Sets the email you want attached to your commit transactions
> color.ui — Enables helpful colorization of command line output

![](https://cdn-images-1.medium.com/max/1600/1*a66RbZybvPoqq8Qh7frgig.png)Usage of git config command

You can also check your individual config variables by —

<pre name="32a4" id="32a4" class="graf graf--pre graf-after--p">$ git config --global user.name
$ git config --global user.email
...
...</pre>

### Setting up our first repository

We can create repositories, start a new repository, or obtain on from an existing URL.

**Go to the project directory on your local system**

<pre name="46a9" id="46a9" class="graf graf--pre graf-after--p">$ mkdir learn-git
$ cd learn-git</pre>

**Start a new repository — **Create a new local repository with the specified name.

<pre name="4669" id="4669" class="graf graf--pre graf-after--p">$ git init [project-name]
# Project name argument is not necessary </pre>

**We can also work on an existing repository — **`$ git clone [url]`

**Create a new repository on GitHub — **The repository which we made using CLI was our local repository, there has to be a global repository which contains all the code, for that, GitHub does our work

![](https://cdn-images-1.medium.com/max/2000/1*8MRf-lr-7b1WtUpEnkC9_g.gif)Thank you GitHub :)

### Our first commit — Let’s GIT started

In our project directory, open terminal (or, GIT) and type in

<pre name="96b1" id="96b1" class="graf graf--pre graf-after--p">$ git init
$ git remote add origin [url(https/ssh)]
$ touch README.md</pre>

By doing so, first we initialize a local repository in that directory (ignore if already done in previous step) then we add the default remote as origin in GitHub repository, or in simple words, we connect our repository with the GitHub remote (repository). After doing so, usually the first step is to add a README in which we generally describe the purpose of repository.

![](https://cdn-images-1.medium.com/max/1600/1*46fQ4HaY4yDuyLU4MA6kqw.png)May the — force be with you

### Make changes

Making changes involves reviewing edits and crafting a commit transaction.

`$ git status` — Lists all new or modified files to be committed

`$ git diff` — This command shows the file differences that are not yet staged

`$ git add [filename]` — This command snapshots the file in preparation for versioning. Instead of adding the files individually, we can add all of them by adding a `.` after add. `$ git add .`

`$ git diff --staged` — After adding the staged flag, now git diff hows the file differences between staging and the last file version.

`$ git reset [file]` — Unstages the file, but preserves it’s contents.

`$ git commit -m "[descriptive message about commit]"` — Records file snapshots permanently in the version history.

> -m is called the message flag, whenever we commit our changes, it is a good practice to add a message along with it. It helps a lot when you would be tracking your commit history in future.

`$ git push -u [remote] [branch]` — this command is used to push your staged changes to a branch (master by default) of remote (origin by default). In simple words, this command will push your code to GitHub :)

> -u is also a flag which stands for upstream. You can read more about these flags [here](https://git-scm.com/docs/git-push/1.6.4.1). 
> **Note:** `-f` flag is used for a force push. Never use that until there is no option left, force pushing will delete all commit history and previous works…

`$ git pull [remote] [branch]` — this command is used to take a pull of staged changes to a branch.

In ordinary language (**Please never use these terms**) pull is analogous to taking the code from a codebase and merging it to your local codebase (or, download xD), and push is simply the opposite of pull.

![](https://cdn-images-1.medium.com/max/1600/1*BcioK8CSIKuJ9Geg9YYj9g.gif)

### Summary

In short, we can do the above procedure by

<pre name="cef6" id="cef6" class="graf graf--pre graf-after--p">$ git status
$ git add .
$ git commit -m "[Some message]"
$ git push origin master</pre>

### Concept of branching

The concept of branching was very well discussed in the previous article, now we will have a look at the commands to implement the concept of branching.

`$ git branch` — lists all local branches in the current repository

`$ git branch [branch-name]` — Creates a new branch

`$ git checkout [branch-name]` — switches to the specified branch and updates the working directory. `$ git checkout -b [branch]` — makes a new branch and switches to it

`$ git merge [branch]` — Combines the specified branch into current branch

`$ git branch -d [branch-name]` — Deletes the specified branch

### Refactoring filenames

These commands are used for relocating and removing the versioned files. These are similar to terminal commands.

<pre name="fda6" id="fda6" class="graf graf--pre graf-after--p">$ git rm [file]    # Deletes the file from working directory 
# It also stages the deletion
$ git rm --cached [file] # Removes the file from version control 
# It preserves the file locally
$ git mv [file-original] [file-renamed]
# Changes the filename and prepares it for commit</pre>

### Redo commits

Erase mistakes and raft replacement history.

<pre name="3396" id="3396" class="graf graf--pre graf-after--p">$ git reset [commit]</pre>

> This command undoes all commits after [commit], preserving changes locally,
> after reset, you can add `--hard` flag to discard all history and change back to the specified commit

### Review history

It is used to track the commits, or in a more broader perspective, it is used to browse and inspect the evolution of project files.

`$ git log` — Lists version history for the current branch

`$ git log --follow [file]` — Lists version history for a file, including the renames

`$ git diff [first-branch]...[second-branch]` — shows the content differences between two branches.

`$ git show [commit]` — Outputs metadata and content changes of speified commit.

### Some info on open source…

GitHub provides an excellent environment for doing open source contribution. I suggest you should read more about [open-source](https://opensource.guide/) ecosystem and making [Pull requests (PR)](https://yangsu.github.io/pull-request-tutorial/).

### An open source contribution

Explaining open-source in depth would probably require another article, but in this one, we can surely talk about the basics…
There are some basic guidelines to be followed whenever you intend to do an open source contribution. first of all we need to find an open source project in which we want to collaborate.

![](https://cdn-images-1.medium.com/max/1600/1*9oSi9J-4nWo0qI8L-5Bp5Q.gif)May the forks be with you

1.  Fork the repository
2.  Pull your copy of repo and make the required changes
3.  push the changes to your forked copy of repository
4.  Open a pull request
5.  Wait for the changes to be approved

![](https://cdn-images-1.medium.com/max/2000/1*xLU5KyclNBat13s5H2Bhmg.gif)Open source contributions — follow the proceedure

After you make a pull request, the owners/members of the organisation will review the changes you made and if they think that the work you have done is legit, they will merge your code. When you make a pull PR, you will see terms like Reviewers, Assignees, Labels, Projects etc.
A reviewer is a person who is reviewing your code and the changes you have made. An assignee can be the PR opener, or someone responsible for changes (who is going to accept the PR after the review is done or just close it). Labels on GitHub help you organise and prioritise your work. You can apply labels to issues and pull requests to signify priority, category, or any other information you find useful.

### Concluding Words

That concludes the part 2 of this article. I hope you know what GIT and GitHub are and how they can be used. Keeping in mind that GIT and GitHub are vast topics and everything can not be put in an article, I personally suggest you should ask any sort of queries, and do send feedbacks and suggestions so that even I can improvise this article by adding more and more information.
Also, we can connect on [GitHub](https://github.com/MadhavBahlMD) or [LinkedIn](https://www.linkedin.com/in/madhavbahl/) and I would more than happy if you send your feedbacks, suggestions or ask queries, just drop me an email :)

* * *

Also, I am creating a community of developers to come, learn together, ask doubts, share resources and grow together. Here are the links to the Gitter chat room and slack workspace, do consider joining it.

1.  [https://gitter.im/Web-Weavers/Learning-Web](https://gitter.im/Web-Weavers/Learning-Web)
2.  [https://join.slack.com/t/web-weavers-group/shared_invite/enQtMzA1NjUwNTExMDEwLTcwMjU1MzNhZTZlNDQwNjYxNTdjYTk1NTg4YzJmNzdhYTZmNGE5NzViZWZkMjQwNmJjNmQzZDcyMzhmYzJiYzU](https://join.slack.com/t/web-weavers-group/shared_invite/enQtMzA1NjUwNTExMDEwLTcwMjU1MzNhZTZlNDQwNjYxNTdjYTk1NTg4YzJmNzdhYTZmNGE5NzViZWZkMjQwNmJjNmQzZDcyMzhmYzJiYzU)

Thanks and Happy coding