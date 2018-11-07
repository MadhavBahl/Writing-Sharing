* * *

# Let’s Code Our Portfolio — A Practical Approach To MaterializeCSS

![](https://cdn-images-1.medium.com/max/2000/1*xj9h7pbPF2FSu2G3kYcpdg.jpeg)“Make it simple, but significant”

> According to me, the best way of learning new frameworks or technologies is to get a hands on experience simultaneously, and here in this article you will be learning the basics of MaterializeCSS and build your own portfolio website.

### Materialize CSS

It is a modern responsive front-end framework based on Material Design. 
Read more about material design [here](https://material.io/guidelines/#introduction-principles).

This tutorial will guide you to make your own portfolio website. To view what you will be making, [visit this project on codepen](https://codepen.io/MadhavBahlMD/pen/mXPXep).

### Why Materialize?

Materialize simplifies the life and work of frontend web devevlopers.

*   Speeds up development
*   User Experience Focused
*   Easy to work with

In simple terms, Materialize provides us with a predefined stylesheet, which we can use to make our work much simpler while making responsive web pages. Before proceeding further, a basic knowledge of **HTML, CSS, JS** is required, and a basic idea of Materialize is recommended.
Materialize provides with a very good documentation which is self sufficient to learn how to use it, you can visit the [getting started page](http://materializecss.com/getting-started.html) of the website.
MaterializeCSS provides us with a standard 12 column fluid responsive grid system. The grid helps you layout your page in an ordered, easy fashion. Read more about grid [here](http://materializecss.com/grid.html).

### Getting Started

Getting started with Materialize is very easy, either we can download the complete CSS and JS files they provide and include theme in our project, or we can use the CDN provided them and include it directly.

```
<!-- Compiled and minified CSS --><link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/materialize/0.100.2/css/materialize.min.css"><!-- Compiled and minified JavaScript --><script src="https://cdnjs.cloudflare.com/ajax/libs/materialize/0.100.2/js/materialize.min.js"></script>
```

### Let’s plan our portfolio

Before coding any software, whether it is a website, mobile app, or a desktop app, it’s basic functionality and specifications must be very clear in your mind. It is very important too have a clear picture of the design in your mind, so let’s make a clear picture of what all our portfolio must have.

<iframe data-width="800" data-height="600" width="980" height="735" src="/media/23afd41ebae7914dd022e6c29afa9b2c?postId=61adfb17e308" data-media-id="23afd41ebae7914dd022e6c29afa9b2c" data-thumbnail="https://i.embed.ly/1/image?url=https%3A%2F%2Fs3-us-west-2.amazonaws.com%2Fi.cdpn.io%2F1607089.mXPXep.small.ed31c526-9b09-4247-a3f7-615d995efcd9.png&amp;key=a19fcc184b9711e1b4764040d3dc5c07" allowfullscreen="" frameborder="0"></iframe>See this pen to get an idea of what we will be building :)

Our portfolio will contain the following sections:

*   **Section 1:** Navigation Bar
*   **Section 2:** Landing Screen
*   **Section 3:** Intro and About Me
*   **Section 4:** Quote with Parallax Scrolling Effect
*   **Section 5:** Projects/Work Experience
*   **Section 6:** Skill Set
*   **Section 7:** Footer

Before starting, we will put some custom styles to the body of our portfolio.

<pre name="fb86" id="fb86" class="graf graf--pre graf-after--p">body {
    background-color: black;
    color: rgba(255,255,255,0.8);
}</pre>

This will make the background color to black and the text color to `rgba(255,255,255,0.8);`

### Section 1: Nav Bar

![](https://cdn-images-1.medium.com/max/2000/1*DTlaCrb3ubOzAGbR-Aug1w.png)Navigation Bar connects all important sections in your page.

This type of navigation bar is simply an unordered list with the list elements styled according to client needs and good design. Basically, the list items are displayed inline, and also each list item contains the anchor tags with links to various sections in the page. Read more about navigation bars [here](https://www.w3schools.com/css/css_navbar.asp).
Here, we use the navbar styles as provided by Materialize. [See here](http://materializecss.com/navbar.html) for more complete reference.
Since we want our navbar to remain on fixed position on top, we will use the class `navbar-fixed` to the main div. Then, in the `nav` tag, we will put the class `black` to make the background color black.

<pre name="d1df" id="d1df" class="graf graf--pre graf-after--p">**<!-- Navbar -->**
<div class="navbar-fixed">
    <nav class="black">
        <div class="container">
            <div class="nav-wrapper">
                <a href="#" class="brand-logo">My Portfolio</a>
                <ul class="right hide-on-med-and-down" id="navList">
                    <li><a href="#landing">Home</a></li>
                    <li><a href="#intro">About Me</a></li>
                    <li><a href="#work">Projects</a></li>
                    <li><a href="#contact">Contact</a></li>
                </ul>
            </div>
        </div>
    </nav>
</div></pre>

Here, we use the class `nav-wrapper` to wrap up our nav bar elements inside this div, then we use the class `brand-logo` as provided by Materialize to place the logo on navbar (here, instead of logo we use plain text “My Portfolio”.
Inside `nav-wrapper` we place our unordered list containing the links to various sections in our website.

### Section 2: Landing Screen

A landing screen is the collection of elements that you see immediately as you open a website.

![](https://cdn-images-1.medium.com/max/2000/1*6rasJ83Icj9oompLONRnAg.png)My name is MADHAV **BAHL,** an opensource developer :)

Basically, this section contains of a background image, and some heading tags.

<pre name="a39d" id="a39d" class="graf graf--pre graf-after--p">**<!-- Landing Screen -->**
<div class="section" id="landing">
        <h5 id="mainText" class="center">My Name Is</h5>
        <h1 style="color: white;"  class="center">
            MADHAV <b>BAHL</b>
        </h1>
        <h6 id="mainText" class="center">A Web Developer</h6>
</div></pre>

Here, we use the class `section` which is used for simple top and bottom padding. Also, we add the class `center-align` to each heading tag to align the text at center.
**Note*** We will be using class `section` in every section, it not only adds top and bottom padding at each section, but it also makes our code more clean and readable depicting a new section is going to start.

Also, include these custom styles in your stylesheet to add the background image.

<pre name="84ae" id="84ae" class="graf graf--pre graf-after--p">#landing{
    height: 100vh;
    background-image: url('[URL to your image here!'](https://user-images.githubusercontent.com/26179770/37276818-e3e358f4-2608-11e8-9659-05585e92a588.png%27));
    background-position: center;
    background-size: cover;
    background-repeat: no-repeat;
    background-attachment: fixed;
    z-index: -1;
}</pre>

<pre name="5ccb" id="5ccb" class="graf graf--pre graf-after--pre">#mainText{
    margin-top: 30vh;
}</pre>

### Section 2b: Adding a Fixed Action Button

Basically, a fixed action button is a button which remains fixed at some position on the screen and is meant for a particular purpose, which is generally to contain links to various external sites.
In our portfolio, we will add a fixed floating action button (FAB) to add multiple actions that will appear on hover, those actions will be nothing but the links to various social media accounts. Read more about FABs [here](http://materializecss.com/buttons.html).

<pre name="b28d" id="b28d" class="graf graf--pre graf-after--p">**<!-- FIXED ACTION BUTTON -->**
<div class="fixed-action-btn vertical">
    <a class="btn-floating btn-large  blue-grey darken-4">
        <i class="fa fa-globe"></i>
    </a>
    <ul>
        <li><a class="btn-floating  blue darken-4"><i class="fa fa-facebook"></i></a></li>
        <li><a class="btn-floating cyan lighten-1"><i class="fa fa-twitter"></i></a></li>
        <li><a class="btn-floating grey darken-3"> <i class="fa fa-github"></i></a></li>
        <li><a class="btn-floating blue-grey lighten-1"><i class="fa fa-linkedin"></i></a></li>
    </ul>
</div></pre>

Also, we use the icons provided by font-awesome to display links to the social media accounts. See the complete list of icons provided by font awesome [here](https://fontawesome.com/icons?d=gallery).

Congratulations, we have successfully made the first two sections of our portfolio :)

![](https://cdn-images-1.medium.com/max/1600/0*ERGShVLKQH9UmC9P.gif)

Now we move to the next section of our portfolio, this one is going to involve some knowledge of grids.

### Section 3: Intro and about me

![](https://cdn-images-1.medium.com/max/2000/1*CFDFrvOIlds6UToCUCiT0w.png)Section 3: About me!

In this section, we divide the whole section into 3 parts, 
1\. Header Quote (full length)
2\. Display Picture (1/4th of full width)
3\. About Me (3/4th of full width)

For the header quote, we use the class `row` and `col s12` which depicts that we are going to use all columns of the grid system.
For display picture, we will use the classes `col s12 m12 l3` so that it takes full width on small and medium devices and one-fourth on large screens.
For the about me data, we will use classes `col s12 m12 offset-l1 l8` so that it gives an offset (blank space) of 1/12th and width of 8/12th of full width.

<pre name="1cc7" id="1cc7" class="graf graf--pre graf-after--p">**<!-- Intro and service -->**
<div id="intro" class="section black">
    <div class="container">
        <div class="row">
            <div  class="col s12">
                <h2 class="center header"> "If you love life, don't waste time, 
                        for time is what life is made up of"</h2>
            </div>
        </div>
        <div class="row center">
            <div class="col s12 m12 l3">
                <img class="responsive-img" src="[**Your Picture Here**](https://user-images.githubusercontent.com/26179770/37276853-0092da1a-2609-11e8-9baf-6edbf21afddd.png)">
            </div>
            <dic class="col s12 m12 offset-l1 l8 ">
                <h5 class="center">Madhav Bahl <b>ABOUT ME</b></h5>
                <p>
                    **YOUR BIO**
                    <br />
                    <i>“**Some Awesome Quote To Show Off!**” </i> 
                </p>
            </dic>
        </div>
    </div>
</div></pre>

### Section 4: Quote with parallax effect

Parallax scrolling is a web site trend where the background content (i.e. an image) is moved at a different speed than the foreground content while scrolling. So, the basic idea in this section is to add a quote with parallax effect set to it’s background image. 
See the parallax effect in action [here](https://www.w3schools.com/howto/tryhow_css_parallax_demo.htm).

![](https://cdn-images-1.medium.com/max/1600/1*B2LA4Jzdf1lktXiEUlFgFw.png)

We will approach this section by making a div with class `parallax` and adding the image to it (this image will serve as the background).
Then, we create another container div with the contents inside it.

<pre name="343e" id="343e" class="graf graf--pre graf-after--p">**<!--Parallax-->**
 <div id="p1" class="parallax-container">
    <div  class="parallax">
        <img src="**Path To Image Here**">
    </div>
    <div class="container">
        <div class="row">
            <div class="col s12 center white-text">
                <h1><b>QUOTE</b></h1>
                <h4 >"Don’t be trapped by dogma –
                    which is living with the results of other people’s thinking. <br />
                    Don’t let the noise of other’s opinions drown out your own inner voice."
                </h4>
            </div>
        </div>
    </div>      
</div></pre>

Here, inside the container we created a `row` and set the width to be `col s12` or full width. and inside that div, we wrote our quote which we want to display using `h4`

To use parallax effect, include this code in script tag

<pre name="188d" id="188d" class="graf graf--pre graf-after--p">$(document).ready(function(){
    $('.parallax').parallax();
});</pre>

### Section 5: Projects/Work Experience

In this section, we are going to display our projects or work experience using material cards. Cards are a convenient means of displaying content composed of different types of objects. They’re also well-suited for presenting similar objects whose size or supported actions can vary considerably, like photos with captions of variable length. See complete reference [here](http://materializecss.com/cards.html).

![](https://cdn-images-1.medium.com/max/1600/1*eubTRR0cri1sMByxpinG4Q.png)Cards can display complex content efficiently

In this section we will be using `Card Reveal` feature of materialize. It provides a card with image, title and small info, and whenever the card is clicked, more information is revealed about the project.
Here, we will be using the grids to align the cards, the container will be divided into 3 columns and each column will contain a card, and to make it responsive, we will be using full width on small screen devices. This is implemented by including the classes `col s12 m4` 
Each card will have a base div with class `card` and `hoverable` (it is a hover class that adds an animation for box shadow, it can be used for any element but it is meant for use on cards) and `black` class to make the background color black.
Inside the `card` div, there will be 3 divs, one for image, one for content and one for content that will be revealed on click.
1\. `card-image` — This div will contain the image of project
2\. `card-content` — This div will contain the title and link to the project.
3\. `card-reveal` — This div will contain the hidden informtion which is to be revealed on click.

<pre name="cb34" id="cb34" class="graf graf--pre graf-after--p">**<!--Work-->**
<div class="section" style="background-color: #141414;" id="work">
    <div class="container">
        <h3 class="header text_b center">My Projects </h3>
        <div class="row ">
            <div class="col s12 m12 l4">
                <div class="card hoverable black">
                    <div class="card-image waves-effect waves-block waves-light">
                        <img class="activator" src="**Path To Image Here!**">
                    </div>
                    <div class="card-content">
                        <span class="card-title activator purple-text text-lighten-5">Project Title <i class="mdi-navigation-more-vert right"></i></span>
                        <p><a class="purple-text text-lighten-5" href="#">Project link</a></p>
                    </div>
                    <div class="card-reveal  black">
                        <span class="card-title purple-text text-lighten-5">Project Title <i class="mdi-navigation-close right"></i></span>
                        <p>Here is some more information about this project that is only revealed once clicked on.</p>
                    </div>
                </div>
            </div>              
        </div>
    </div>
</div></pre>

This code snippet shows only one card, you can add as many cards as you want, keeping in mind the grids for alignment.

### Section 6: Skill Set

![](https://cdn-images-1.medium.com/max/1600/1*vFy5mkOljoEUk1ZIwX95vg.png)

Again, this section is totally based on the grid system.
Firstly, in a row we will write a center aligned header “My Skills” and then in next row, we divide the row into 4 equal columns (on largescreen sizes and full width on small screens) by using `col s12 m3` and placing the images of languages in it.
Also, we use the `img-responsive` class to make the image responsive to the size of parent div.

<pre name="0dad" id="0dad" class="graf graf--pre graf-after--p">**<!-- Skill Sets -->**
<div class="section" style="background-color: #101010;" id="skillsets">
    <div class="container">
        <div class="row">
            <h1 class="center white-text">
                My Skills
            </h1>
        </div>
        <div class="row center">
            <div class="col s12 m12 l3">
                <img class="responsive-img" src="img/cpp.png">
            </div>
            <div class="col s12 m12 l3">
                <img class="responsive-img" src="img/node.png">
            </div>
            <div class="col s12 m12 l3">
                <img class="responsive-img" src="img/py.png">
            </div>
            <div class="col s12 m12 l3">
                <img class="responsive-img" src="img/shell.png">
            </div>
        </div>
    </div>
</div></pre>

We are done with all main sections on our portfolio, just the footer is remaining and it is the most simple section, we just have to add our name and copyright details in the footer.

### Section 7: Footer

![](https://cdn-images-1.medium.com/max/1600/1*_kqQZLBWPFgfMj93QOZydQ.png)

<pre name="4f4d" id="4f4d" class="graf graf--pre graf-after--figure"><footer class="section page-footer black">
    <div class="container center-align">
        &#169; Madhav Bahl 2017
    </div>
</footer></pre>

Here, we use `section` for the : bottom and top padding and then we center align the main text.

**Congratulations, you have developed your own portfolio website. Time to party :)**

![](https://cdn-images-1.medium.com/max/1600/0*7DfYk8N4xzLpoS0m.gif)

### Concluding Words

I hope this article helped you :)
In case of any doubts, feel free to send me an email. Also, I would recommend trying out different frameworks like Bootstrap and Skeleton CSS, it is always great to learn new technologies.
We can connect on [GitHub](https://github.com/MadhavBahlMD) or [LinkedIn](https://www.linkedin.com/in/madhavbahl/) and I would more than happy if you send your feedbacks, suggestions or ask queries. Moreover, I love to make new friends and we can be friends, just drop me a text :)
Just in case you wish to be a web developer, [have a look at this article](https://medium.com/@madhavbahl10/a-practical-approach-to-web-development-1ee37a4ad829), I wrote it to provide a clear road map of how to start and proceed with web development.

* * *

I am trying to build a community of developers called Logic Xcution where we learn, share, develop and grow together. If interested, join the slack workspace today.
Slack: [https://join.slack.com/t/logic-xcution/shared_invite/enQtMzMzMTM4MTQzMTM2LTgwM2IyYjk4ZWIwODNmYmYzYTc1OWFjNDI3NzMwYWEwZjg2MjgwMDQ1MTU4ODhhYjY0MTFjMGJjZTk2OWRlYTE](https://join.slack.com/t/logic-xcution/shared_invite/enQtMzMzMTM4MTQzMTM2LTgwM2IyYjk4ZWIwODNmYmYzYTc1OWFjNDI3NzMwYWEwZjg2MjgwMDQ1MTU4ODhhYjY0MTFjMGJjZTk2OWRlYTE)

[**Logic Xcution**
_Logic Xcution. 81 likes. An open community for all the people who aspire to be a developer, or are currently a…_www.facebook.com](https://www.facebook.com/LogicXcution/ "https://www.facebook.com/LogicXcution/")[](https://www.facebook.com/LogicXcution/)

> Thanks a lot for keeping your calm and reading till end. 
> Now you know what all practises to adopt to have a write good code,
> All the best and Happy coding!
> You can contact me in case of any doubts or if you need any assistance:
> Email: madhavbahl10@gmail.com
> Web: [http://madhavbahl.ml/](http://madhavbahl.ml/)
> Github: [https://github.com/MadhavBahlMD](https://github.com/MadhavBahlMD)
> LinkedIn: [https://www.linkedin.com/in/madhavbahl/](https://www.linkedin.com/in/madhavbahl/)

[![](https://cdn-images-1.medium.com/max/2000/1*i3hPOj27LTt0ZPn5TQuhZg.png)](http://bit.ly/codeburst)

> ✉️ _Subscribe to_ CodeBurst’s _once-weekly_ [**_Email Blast_**](http://bit.ly/codeburst-email)**_,_** 🐦 _Follow_ CodeBurst _on_ [**_Twitter_**](http://bit.ly/codeburst-twitter)_, view_ 🗺️ [**_The 2018 Web Developer Roadmap_**](http://bit.ly/2018-web-dev-roadmap)_, and_ 🕸️ [**_Learn Full Stack Web Development_**](http://bit.ly/learn-web-dev-codeburst)_._