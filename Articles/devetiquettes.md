* * *

# Dev **etiquettes** that you must not ignore

![](https://cdn-images-1.medium.com/max/2000/1*gg0YLENYcyQbrs6J3gokMw.jpeg)“Always code as if the guy who ends up maintaining your code will be a violent psychopath who knows where you live”

**Ever wondered what we really mean by etiquettes why were they made and why are they necessary in our daily lives?**

Okay, I’am about to give a small lecture, please bear with me for 30 seconds after that we will get straight to the point.

![](https://cdn-images-1.medium.com/max/1600/0*fhtVSE20t_rYnuSk.jpg)**“_First, solve the problem. Then, write the code._” **— John Johnson

### Etiquette

> “the customary code of polite behaviour in society or among members of a particular profession or group”

Human beings are social animals and it is our prime duty to be considerate towards other people and not annoy them with our illogical and ill-mannered behaviour, therefore even if no one forces you to maintain a code of conduct, it is your duty as a **good human being** to maintain your polite behaviour, that is, if you do want to live peacefully in this society……

![](https://cdn-images-1.medium.com/max/1600/1*bhOdNJ5tBSj_2y_W_HRIPQ.png)Let’s get to the point

### **OKAY, Why am I talking about etiquettes?**

Yes, it may sound weird to you (if you are a beginner), we coders, too maintain some manners while coding **#Coding_Etiquettes**. If you want to become a good coder/developer, you must never ignore these etiquettes.

![](https://cdn-images-1.medium.com/max/1600/1*dUQuNsBDaBT1SYgpXf6M6Q.png)“In Code We Trust”

Let’s have a look at some popular dev etiquettes that will help make your code much more readable, well structured, (obviously more good looking than before) and help you get some self-respect in developers’ community.

![](https://cdn-images-1.medium.com/max/1600/1*IkcQop8_z6QuZw_JUrw-jA.png)Write good quality code, stay happy :)

### Proper Indentation

I have seen tons of beginners, while writing their code they just start writing without keeping in mind proper spacing and indentations. Generally their code looks something like —

```cpp
#include< iostream.h >
using namespace std;
void main() 
{
int a,b;
cout<<"Please enter a: ";
cin>>a;
cout<<"Please enter b: ";
cin>>b;
.
.
.
if(a < b)  
cout<<"a+b = "<< a+b;
else   
cout<<"a-b = "<< a-b;
}
```

These are only 14 lines of code, so it doesn’t matter much. But now consider that some time has passed and they are given a project. That project may include 2000 lines of code. Just think about it, how messy the code would look like. I get scared even by the thought of it.
So, according to me, the first and foremost thing that teachers should teach after `Hello, World!` program is how to write a neat code. Have a look how beautiful a code with proper indentation looks like. It becomes like a nicely written poem, which the programmer can read and understand easily.

![](https://cdn-images-1.medium.com/max/1600/1*IwoBJ-tyo44n8Q88SsUAdw.png)“How beautiful a neatly written code looks like”

How beautiful this code looks like, isn’t it? 
Yes, so let’s take a decision, “We the coders, will always give proper indentation”. Giving 2 or 4 spaces in each structure is a general indentation practise nowadays. Furthermore, there are many other reasons why you should write properly indented code.
A proper indentation will make your code easier to read, understand, modify and maintain.

### Tree Like Directory Structures

Whenever you take up a project, keep one basic thing in mind that you are not going to write the whole code in a single file. You have to use different files for different purposes. It is a good practise to maintain proper tree like directory structure as shown in the diagram.

![](https://cdn-images-1.medium.com/max/1600/1*hK3HmceEAw4ZmDf7nLO8Tg.png)

Maintaining a good directory structure makes coding much more efficient. When you are doing a big project, maintaining such good structure will save you time in searching for the files you need.

### Comments PLEASE!

According to me, this is one of the most important coding etiquette. Many times it happens that people just go on writing the code finish it in a haste and when they come back after some time (say, 1 month) they have no idea what the code was all about.

![](https://cdn-images-1.medium.com/max/1600/1*Dv6_aCk8QTjUz94pS-KatQ.jpeg)“Dont understand your own code? GREAT!”

It is a very good practise to write comments for each and every function or module you write. Doing this helps a lot in debugging the code in case of errors. If you have comments for every particularity of code, it helps understand where the code went wrong, in case there are bugs.

![](https://cdn-images-1.medium.com/max/1600/1*otTaZoZHCErkJ-csCt4sdw.png)“Good code is self-documenting.”

Have a habit of writing comments because they help anyone (including your future self) to maintain, refactor, or extend your code.

### Document your code

When you are a developer, never ever forget to make a proper documentation for your code. Documentation comments are intended for anyone who is likely to consume your source code, but not likely to read through it.

![](https://cdn-images-1.medium.com/max/1600/0*Vbd68YNeq8-OHeOw.jpg)ALWAYS document your code.

Lets take an example, say you are a back-end developer, and you just made an API (Read more about APIs [here](https://en.wikipedia.org/wiki/Application_programming_interface)) and a front-end developer likes to use it for some specific purpose. Now he has to read and go through the whole code if you don’t write a proper documentation for your code, which becomes useless wastage of time. To prevent this, it is the moral duty of the developer of API to create and maintain proper documentation for the working of his code.
For example, see the following screenshot, it is taken from [mongoosejs](https://github.com/Automattic/mongoose) library, it has got amazing documentation

![](https://cdn-images-1.medium.com/max/1600/1*MGsdop2LyyhmBE-_sJc1Nw.png)See how the docs of mongooseJS [here](http://mongoosejs.com/docs/guide.html)

### Don’t just foobar everywhere

Well if you are a complete beginner, you might not be aware of what foobar is, the terms like foobar, foo, bar, and baz are common placeholders which are used when you cant think of a proper name for a variable or a file. These terms can be used to represent any part of a complicated system or idea, including the data, variables, functions, and commands.
Using such random names is a very bad practise, whenever you write a code always keep in mind that the name of your variables and functions must represent clearly their respective functions.

![](https://cdn-images-1.medium.com/max/1600/0*kAKIQ9-JpIyaUAn6.jpg)Your name represents your purpose.

Using such random names can create a huge problem while testing and debugging phase. No one would want to waste their time in finding what `foo` was used for and what `bar` was used for.

### Meaningful File Names

Never give random names to your files, just like variable names, your file names must also represent the purpose for which they were created.

![](https://cdn-images-1.medium.com/max/1600/1*7P3LwZid7bCsKYJe6CwQpw.png)Your file names should be understandable

Actually, there exist several file naming conventions, which are recommended and you should follow them. But even if you don’t follow them exactly, at least keep the file names in such a way that they are understandable to you. Never keep filenames such as: `xyz.md` or `abc.txt`

> A file naming convention (FNC) can help you stay organised by making it easy to identify the file(s) that contain the information that you are looking for just from its title and by grouping files that contain similar information close together. A good FNC can also help others better understand and navigate through your work. [**Read more here**](http://guides.lib.purdue.edu/c.php?g=353013&p=2378293)

### Select your case type

Following a typography for naming your variables is always a good practise. Select your case type and always write names in that case so that they become more clear and readable. For example, I always use camel case.

Have a look at some popular case types:

1.  **Capitalization** — Writing the first letter of a word in uppercase, and the rest of the letters in lowercase.
2.  **PascalCase —** Words are written without spaces, and the first letter of each word is capitalized. PascalCase is sometimes also called the UpperCamelCase.
3.  **camelCase** — A variation of Pascal Case in which the fist letter of the word is lowercase, e.g. iPhone.
4.  **snake_case** — Punctuation is removed and spaces are replaced by a single underscore. Can be done with either upper or lowercase, but whichever is used should continue to be used.

> “Just because you can write a program doesn’t make you a good programmer, writing a code which even a layman can understand is what makes you a good programmer”

### Keep your code DRY

What is DRY code? DRY is an abbreviation for don’t repeat yourself. If you have to copy and paste code several times while making a project or a software, you are not at all a good developer. Repeating same lines of code many times is considered a very bad practised in coding.

![](https://cdn-images-1.medium.com/max/1600/0*-v5er932CjzpQfp6.jpg)I will not repeat myself :)

Code can be kept DRY, with the extensive use of functions. whenever you see that you are repeating the same lines of code, make it a function. Keeping your code DRY has many advantages like it keeps your code clean and reduces the chances of bugs.
_“Bugs love a wet mess” — unknown_

**Dry code maintains modularity** You can even divide the main purpose of the program into several smaller functions and do them individually. It helps to manage big programs.

### How about choosing some common coding conventions?

**Coding conventions** are a set of guidelines for a specific programming language that recommends programming style, practices, and methods for each aspect of a program written in that language.
Choose a coding convention for your projects and stick to it… **ALWAYS** Find more about coding conventions [here](https://en.wikipedia.org/wiki/Coding_conventions).

### Have Fun!

Now this is the most important part of programming, whatever program you write, whatever software you develop, always have fun. Coding is amazing, make it your daily habit and you will find how amazing it is.
If you don’t have fun writing your code, it will clearly reflect in your code :)

* * *

### Concluding Words

I hope this article helped you, we can connect on [GitHub](https://github.com/MadhavBahlMD) or [LinkedIn](https://www.linkedin.com/in/madhavbahl/) and I would more than happy if you send your feedbacks, suggestions or ask queries. Moreover, I love to make new friends and we can be friends, just drop me a text :)
Just in case you wish to be a web developer, [have a look at this article](https://medium.com/@madhavbahl10/a-practical-approach-to-web-development-1ee37a4ad829), I wrote it to provide a clear road map of how to start and proceed with web development. We also have an open community to bring together developers so that we can learn and grow together, join the [Slack Workspace](https://codetoexpress.slack.com/join/shared_invite/enQtNDUwNzg0NDI1MzAwLWZiODY3OGZkZjdkZDA2MWNmMjFiNTY2MDlmMDg5ZGVjMzc5NDQ5OWU0NjEyNWZiM2Y4MmZmYmM0ZmQ3NjJmYWI) today.

Want to read this article on medium? [Click Here](https://medium.com/codeburst/dev-etiquettes-that-you-must-not-ignore-619e1bb490b8)

> Thanks a lot for keeping your calm and reading till end. 
> Now you know what all practises to adopt to have a write good code,
> All the best and Happy coding!
> You can contact me in case of any doubts or if you need any assistance:
> Email: madhavbahl10@gmail.com
> Web: [http://madhavbahl.ml/](http://madhavbahl.ml/)
> Github: [https://github.com/MadhavBahlMD](https://github.com/MadhavBahlMD)
> LinkedIn: [https://www.linkedin.com/in/madhavbahl/](https://www.linkedin.com/in/madhavbahl/)