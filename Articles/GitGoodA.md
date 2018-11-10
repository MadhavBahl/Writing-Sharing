* * *

# GIT Good: A Practical Introduction to GIT and GitHub (Hello GitHub)

![](https://cdn-images-1.medium.com/max/2000/1*FKJpjQO4ctBGmT1EM4d1mQ.jpeg)Lets GIT Going…

**This is a two part series on GIT and GitHub,**
 → GIT-Good Part-A: Hello GitHub 
[GIT-Good Part-B: In Git we trust!](https://medium.com/@madhavbahl10/git-good-a-practical-introduction-to-git-and-github-in-git-we-trust-f18fa263ec48)
You are currently reading the **Part A** in which we will talk about the basics of GIT and GitHub, if you are already familiar with the basics, you can directly jump to the [**Part B**](https://medium.com/@madhavbahl10/git-good-a-practical-introduction-to-git-and-github-in-git-we-trust-f18fa263ec48)in which we will discuss about the commands involved in GIT CLI.

> “Using Version Control is a basic necessity for the developers today and every developer is expected to have the knowledge(at least the basics) of any VCS. By far, the most widely used modern version control system in the world today is GIT. GIT and GitHub has made the life of developers so much easier that simply thanking them won’t be enough.”

### Let’s GIT Going — Why another article on GIT?

GIT is the most widely used VCS and is considered to be the best friend of any developer today. Whether it maybe **version control, project management, team collaboration or open source development/contribution**, GIT and GitHub has made our lives much more easier. Every good developer has an idea of how hard the life would have been without GIT and GitHub. But, the most common thing that is noticed in the novice developers is the fear of GIT CLI tool. This is a two part article which will comprehensively cover the GitHub version control service as a companion to the Git CLI tool.

### But, what do you mean by version control?

A version control can be seen as a system which keeps a track of your changes, allows an environment for collaborative development, allows you to know who made what changes and when, and most importantly, allows you to revert any changes and go back to a previously saved state.

### GitHub — Where software is built

![](https://cdn-images-1.medium.com/max/1600/0*6FETDgCn09uY2C4t.jpg)Be careful not to step in the git-gui! CLI is ❤

**GitHub** is a web-based hosting service for version control using git. It is mostly used for computer code. It offers all of the distributed version control and source code management (SCM) functionality of Git as well as adding its own features. It provides access control and several collaboration features such as bug tracking, feature requests, task management, and wikis for every project.

![](https://cdn-images-1.medium.com/max/1600/1*-p5kuyQdT5ici6NnBPT-Vw.png)

It’s Ok, I know if you are a beginner, you did not understand any of the thing’s which I talked about till now. Don’t worry, I will explain in detail.
GitHub is basically an online platform which provides many features. You can upload and manage your code here, if you have a team and you are working on a project, you can work together, you can make some open source contributions, or make your own open source projects/softwares, form your own tech community, or join an existing one, find other people’s projects, follow the people you feel are sound in their domain and much more.
To be honest, I am more active on **GitHub** than on Facebook.

> “Once you go git, you never go back.”

### Here, have a look at the features that GitHub provides:

*   **Collaboration** — Helps to work in team
*   **Version Maintenance** — Keep track of your code
*   **Transparency in work** — Detailed history of every commit
*   **Track issues **— Helps a lot in verification and validation
*   **Code reusability**
*   **Enterprise grade security**, and [much more](https://enterprise.github.com/features)..

**Are GIT and GitHub same thing?** It is my humble request, please never ask this stupid question ever again 😂 
**GIT** is a version control system, or basically a tool to manage your code history, while **GitHub** is a hosting service for GIT repositories. Clearly, they are not the same things. 
In short, **GIT** is a tool, and **GitHub** is a service for projects that use GIT.

> “At start using GitHub seems complicated, but rest assured, once you are used to it, you will come to know that there is no better thing than GitHub.
> GitHub has become an integral part of my daily routine, and my day seems incomplete without making a contribution”
>  — Many people who use GitHub

### Let’s make an account

First of all, we need to create an account on GitHub. Just as you create an account on any website just signup on GitHub.

**Note*** It’s not Github, it’s **G**it**H**ub :)

![](https://cdn-images-1.medium.com/max/1600/1*-J4m04VeX2IRWPczfn_VvA.gif)Getting Started Is A Piece Of Cake :)

### Let’s have a closer look at GitHub

![](https://cdn-images-1.medium.com/max/1600/1*a0ePVzfE1nlduReYvBadvw.png)Screenshot from my [GitHub profile](https://github.com/MadhavBahlMD)

This is how a GitHub profile looks like. Before starting with GIT CLI, we will have a look at GitHub, how a GitHub profile looks like and what all features do GitHub provides.

![](https://cdn-images-1.medium.com/max/1200/1*EsbPeyb2M7JQD3qaXHI6nQ.png)

### 1\. Your information

This is basically your dashboard in GitHub, where all your information is displayed. The amount of information to be displayed can be easily controlled by going into settings.

The displayed informaton includes name, username, your organizations, your caption(or, Bio), email, website and location.

I love to call this the _“About Me”_ section of GitHub account.

![](https://cdn-images-1.medium.com/max/1200/1*OQEcrvhIer_K7l4wLdMdWQ.png)

### 2\. Your Organizations

This area shows the logos of organisations that you are a part of. It will be visible to others only if the membership is public.

### 3\. Overview

![](https://cdn-images-1.medium.com/max/1600/1*PsTO_fAjIfaDq9l_zxQC4w.png)GIT: Committed for life ❤

This section of your GitHub profile shows your pinned repositories (the projects which you consider to show to the world) and your contributions. 
More dark green implies more contributions. Learn more about [how does GitHub counts contributions.](https://help.github.com/articles/why-are-my-contributions-not-showing-up-on-my-profile/)
Whenever anyone asks me, I want to be a developer or asks me any advise, joining GitHub and learning GIT is the first thing I say. The environment and community that GitHub provides is simply amazing.

### 4\. Stars, Repos, Followers and Following

![](https://cdn-images-1.medium.com/max/1600/1*flZnB3KwSNgsw98f2aS1qA.png)

The best thing about GitHub is that it provides an environment which is similar to social media, your can star the projects/repositories which you love, follow other developers and see their profiles.

![](https://cdn-images-1.medium.com/max/1600/0*aBMfrm3TuAwX0jyW.png)This feeling is lit 🔥

### 5\. More on GitHub

Apart from these, GitHub profile also has a notifications corner which (as the name suggests) shows the notifications about the repositories or teams you are a part of.

### Creating a repository

Now, that you have have an account on GitHub you might be wondering what a repository is?
In simple words, A repository is a digital directory or storage space where you can access your project, its files, and all the versions of its files that Git saves.

![](https://cdn-images-1.medium.com/max/2000/1*0_zja37vbfb5RNErugSYag.gif)Now we are getting to the point xD

Now that we have an account on GitHub, and we know basics like what is a repository and it’s the time to move forvard to GIT.

> Thank you for bearing with me till here, I know they were a bit boring, but those basics were necessary.
> I promise now we will get straight to the point.

### Let’s imagine a development without version control

![](https://cdn-images-1.medium.com/max/1600/1*wW5dcnXhZ72U-M3ChEDQbg.gif)[https://www.slideshare.net/jomikr/quick-introduction-to-git](https://www.slideshare.net/jomikr/quick-introduction-to-git)

Let’s imagine the case, there is a team of 4 people developing a software without using a version control.
Since they have tasks assigned, they will do some contributions, make some code and merge it. As in the image, lets say that Bob finishes a module, then Carol also finishes her module, when they combine let’s say some merge conflicts arise (for now, you can imagine merge conflicts as some problems in merging the code or integration of modules), then Alice also finishes the work allotted and tries to merge and then Ted also completes his portion of work and tries to integrate. 
You can easily imagine the mess that is created. To prevent situations like these, version controls are used.

### GIT is here!! Finally

After reading all of the above, you might have got a basic ideaof what GIT is. Just for revision I will tell again, Git is a type of **version control system** (VCS) that makes it easier to track changes to files. For example, when you edit a text file, git can help you determine exactly _what_ changed, _who_ changed it, and _why_. Git isn’t the only version control system out there, but it’s by far the most popular.

![](https://cdn-images-1.medium.com/max/1600/0*Xokg4oWGLB96vhyW.)I kissed a git, and I liked it. I hope my repo don’t mind it

The major difference between Git and any other VCS (Subversion and friends included) is the way Git thinks about its data. Conceptually, most other systems store information as a list of file-based changes. These other systems (CVS, Subversion, Perforce, Bazaar, and so on) think of the information they store as a set of files and the changes made to each file over time (this is commonly described as _delta-based_ version control).

![](https://cdn-images-1.medium.com/max/1600/1*6ywHRvYfgRVCSL_4xh1Mfw.png)Delta Based Version Control

Git doesn’t think of or store its data this way. Instead, Git thinks of its data more like a series of snapshots of a miniature filesystem. With Git, every time you commit, or save the state of your project, Git basically takes a picture of what all your files look like at that moment and stores a reference to that snapshot. To be efficient, if files have not changed, Git doesn’t store the file again, just a link to the previous identical file it has already stored. Git thinks about its data more like a **stream of snapshots**.

![](https://cdn-images-1.medium.com/max/1600/0*V1iIPrfbxJFLOQEU.png)*Images taken from [https://git-scm.com/book/en/v2/Getting-Started-Git-Basics](https://git-scm.com/book/en/v2/Getting-Started-Git-Basics)

### Before going any further, we need to know some basic terms…

1.  **Snapshot **— It records all your files at a given point of time so that you can look up at them anytime later. It is basically a way how GIT tracks your code history.
2.  **Commit** — The act of creating a snapshot is called a commit. One is advised to commit his code whenever there are significant changes made.
3.  **Repository** — The location or digital storage where all your files are stored.
4.  **Head **— The reference to the most recent commit is called Head.
5.  **Branches **— 
    GIT follows a sort of tree like analogy for keeping track of code, when several people are collaborating on a project, the general procedure is to make a branch from the master branch, do the changes there and make a request to the master branch to merge the code.
    Basically, All commits live on some branch and there can be many branches in a single project repository.

![](https://cdn-images-1.medium.com/max/1600/0*-8t0j0AN8GL2OP9y.png)

### Understanding the concept of branches…

This concept of branches is what every beginner fears of, even me (at my first day to GIT) feared this concept and tried to ignore it. But believe me, this is the most important and interesting thing about GIT. 
To express it simply, a branch can be called the current working environment of a developer. All the working and main code is stored in the master branch (as the name suggests). Whenever a developer wants to make some changes in the main code base or add a new project module, he is expected to make a new branch, make the changes/add new modules to that branch itself, test the code properly and then merge the branch with master branch. Doesn’t it seems very nice and clean process? That’s the beauty of using GIT.
So in short we can say, a bunch of commits makes up a branch and all the branch combined makes a repository.

![](https://cdn-images-1.medium.com/max/1600/0*o-6UAkbjP_LfmvJ6.)git: history is written only by those who are committed

This diagram beautifully represents the basic work flow. 
1\. Make a branch
2\. Do the work
3\. Make a **Pull Request**, and merge branches.
Here comes another new term, what is a pull request?

### Pull Request

As told earlier, Git uses a tree like structure for maintaining and tracking code. master branch is analogous to the main trunk of the tree, and contains the main codebase. Every time you add more changes (**commits**), your tree grows taller. Even if you delete code, that’s still considered a change and causes the master branch to grow. Every change is being recorded in form of snapshots which helps tracking of code as stated earlier.
Now, whenever you want to make a change, you make a new branch make changes and submit the code to be merged, **this submission can be done through a pull request(PR)** or a merge request (PULL? because you are requesting your changes to be pulled inside the master branch). Some people are afraid of making their first PR, but it’s really nothing to be afraid of. Most teams are happy to receive new PRs, even if the code needs a bit of work before being accepted. PRs are an important part for working in an open source environment (Google it!).

> Now that we know the theoretical concepts, lets start the real game :)

### Installing GIT

GIT is available for all three major platforms, Linux, Mac and Windows

**Installing GIT on Windows** Download _Git_ from [GIT for Windows](https://git-scm.com/download/win) and install it. It is a basic setup just like other softwares.

![](https://cdn-images-1.medium.com/max/1600/1*x2z-4tM-fMjaWyxdrMloPw.gif)As simple as that

**Installing GIT on MAC** You can download [GIT for MAC](https://git-scm.com/download/mac) and install it.
Or, you can install git using Homebrew, 
To install Homebrew, copy and paste the following into the terminal

<pre name="52ae" id="52ae" class="graf graf--pre graf-after--p">ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
brew doctor</pre>

Copy & paste the following into the terminal window and hit `Return`.
`brew install git`

**Installing GIT on Linux** Determine on which _Linux_ distribution your system is based on. Most _Linux_ systems (including _Ubuntu)_ are _Debian_-based.
1\. For **Debian-based** linux systems
Open a terminal window (ctrl+alt+t). Copy & paste the following into the terminal window and hit `Return`. You may be prompted to enter your password.

<pre name="0c02" id="0c02" class="graf graf--pre graf-after--p">sudo apt-get update
sudo apt-get upgrade
sudo apt-get install git</pre>

2\. For **Red Hat-Based** linux systems
Open a terminal. Copy & paste the following into the terminal window and hit `Return`. You may be prompted to enter your password.

<pre name="5b11" id="5b11" class="graf graf--pre graf-after--p">sudo yum upgrade
sudo yum install git</pre>

### Setting up SSH for GitHub is highly recommended.

Although, setting up an SSH key is not at all mandatory, but it is recommended that you do it. For the detailed procedure for the same, [refer here](https://help.github.com/articles/adding-a-new-ssh-key-to-your-github-account/). If you are not comfortable with the steps, you can watch this video.

<iframe data-width="854" data-height="480" width="700" height="393" src="/media/f8ee466030dee1700beb61b0a22a47c6?postId=e0d826286a2a" data-media-id="f8ee466030dee1700beb61b0a22a47c6" data-thumbnail="https://i.embed.ly/1/image?url=https%3A%2F%2Fi.ytimg.com%2Fvi%2FVi-WqFKYpnw%2Fhqdefault.jpg&amp;key=a19fcc184b9711e1b4764040d3dc5c07" allowfullscreen="" frameborder="0"></iframe>

### Concluding Words

That concludes the part 1 of this article. I hope you have gained some insight into what GIT and GitHub are and how they can be used. We can connect on [GitHub](https://github.com/MadhavBahlMD) or [LinkedIn](https://www.linkedin.com/in/madhavbahl/) and I would more than happy if you send your feedbacks, suggestions or ask queries, just drop me an email :)

* * *

#### If this post was helpful, please click the clap 👏 button a few times to show your support!

Also, I am creating a community of developers to come, learn together, ask doubts, share resources and grow together. Here are the links to the Gitter chat room and slack workspace, do consider joining it.

1.  [https://gitter.im/Web-Weavers/Learning-Web](https://gitter.im/Web-Weavers/Learning-Web)
2.  [https://join.slack.com/t/web-weavers-group/shared_invite/enQtMzA1NjUwNTExMDEwLTcwMjU1MzNhZTZlNDQwNjYxNTdjYTk1NTg4YzJmNzdhYTZmNGE5NzViZWZkMjQwNmJjNmQzZDcyMzhmYzJiYzU](https://join.slack.com/t/web-weavers-group/shared_invite/enQtMzA1NjUwNTExMDEwLTcwMjU1MzNhZTZlNDQwNjYxNTdjYTk1NTg4YzJmNzdhYTZmNGE5NzViZWZkMjQwNmJjNmQzZDcyMzhmYzJiYzU)

Thanks and Happy coding

### References

1.  [https://www.slideshare.net/jomikr/quick-introduction-to-git](https://www.slideshare.net/jomikr/quick-introduction-to-git)
2.  [https://git-scm.com/book/en/v2/Getting-Started-Git-Basics](https://git-scm.com/book/en/v2/Getting-Started-Git-Basics)