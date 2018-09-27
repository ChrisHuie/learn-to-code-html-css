# Introduction to HTML and CSS

## Repo short URL [htmlrepo.sage.codes](https://github.com/sagecodes/learn-to-code-html-css)

## Do these things first!
- Download and install a text editor
    - [VS Code](https://code.visualstudio.com/)
    - [Atom](https://atom.io/)
    - Or use an onlone editor like [codepen](https://codepen.io/) 
- I also recommend using [chrome](https://www.google.com/chrome/) as a web browser.


<!--###### Download the files for this class:
1. Go to [https://github.com/GalvanizeOpenSource/l2c-html-css-2018](https://github.com/GalvanizeOpenSource/l2c-html-css-2018)
2. Click on the button on the right-hand side that says "Download ZIP"
3. Go to your downloads folder and double click on the .zip file to unzip it
4. IMPORTANT! Leave all the individual files in the downloaded folder (if you would like to move it out of the downloads folder move the entire folder, not individual items)
5. From Atom: File > open, select the folder and then click "Open"
6. From Atom: If the file tree does not appear on the left hand View > Toggle Tree View -- this will show you the entire folder within Atom
7. *Now if you already know some of what we're talking about,* you're all set to poke around in the files -- `index.html` and `CSS/style.css` are the two files we will using.
8. The `examples` folder contains an example of a simple web page using HTML and CSS. If you get stuck you might want to refer to the example page.
-->
 
## What this workshop is

A super friendly introduction to web development with HTML and CSS! No previous experience expected! 

You can't learn EVERYTHING in ~2 hours. But you can learn enough to get excited and comfortable to keep working and learning on your own! Come to our weekly code hours [meetups](https://www.meetup.com/Learn-Code-Seattle/events/) to ask questions if you get stuck and show off what you've been working on!

- This course is for absolute beginners
- Ask Questions!
- Answer Questions!
- Its ok to get stuck, just ask for help!
- Feel free to move ahead
- Help others when you can
- Be patient and nice


## About me:
Hello I'm [Sage Elliott](http://sageelliott.com/). I'm a Technology Evangelist at Galvanize Seattle. Previously I've worked as a software and hardware engineer with Startups and Agencies in Seattle, WA and Melbourne, FL. I love technology! I'm currently learning more about how to build AI and VR projects (I can't wait to do a workshop round these topics)! 

*caveat* I'm not an Galvanize instructor, they're much better at teaching than I am!

If you have an event you would like to see or put on let me know! I'm always looking for ideas. Talk to me after the workshop or find me online at one of these:

- Website: [sageelliott.com](http://sageelliott.com/)
- Twitter: [@sagecodes](https://twitter.com/@sagecodes)
- LinkedIn: [sageelliott](https://www.linkedin.com/in/sageelliott/) 
- Email: [sage.elliott@galvanize.com](mailto:sage.elliott@galvanize.com)


## About you!

Give a quick Intro!

- Whats your name?
- Whats your background?
- Why are you interested in Web Development?

## What is HTML and CSS?

Two of the main building blocks of the web!

- HTML (Hyper Text Markup Language)
- CSS (Cascading Style Sheets)

An analogy you can think of for the scope of this workshop:

HTML is sort of like bones. Its the structure of the web page.

CSS is similar to skin. It adds style and changes the appearance of the page. 

JavaScript is like the Muscle. It can change and move elements around on the page(not covered in this workshop). 

Is there a "brain"? Yes! There are many languages that can used to access databases, perform complicated calculations and send/receive information. Some common languages: Javascript, Python, Ruby, PHP. 

### Who uses HTML & CSS?


## HTML Basics

###### Some common Tags(Elements):

- `<html>`	designates an HTML document
- `<head>`	contains undisplayed information about the document
- `<title>`	Creates a title for the document
- `<body>`	contains displayed information
- `<header>, <main>, <footer>` denotes which part of the page elements belong

- `<h1> - <h6>` create section headings (h1 biggest, h6 Smallest)
- `<p>` creates paragraphs
- `<a href=""></a>` (anchor), activates a link in the page
- `<ul>, <ol>` creates lists
  - `<li>` contains items in lists
- `<br>`	Inserts a single line break
- `<hr>`	Defines a thematic change in the content

###### Self-closing Tags:
most HTML tags require an opening and a closing tag. There are a few however that do not:

- `<img src="">` creates an image in the page
- `<br>` creates a break in the content
- `<input type="">` creates an input field

###### IDs, Classes
IDs and classes are very similar.
These are used to target specific elements(You'll see more examples in CSS section).
- `<h1 id="profile-header"></h1>`
- `<h1 class="subject-header"></h1>`

- IDs should only be used once on a page. IDs can also be used to bring the user to a specific part of the page. `your-site/#profile-picture` will load the page near the profile picture. 
- Classes can be used multiple times on a page. 


See More tags [here](https://www.w3schools.com/tags/ref_byfunc.asp)

Learn more HTML [here](https://www.w3schools.com/Html/)

## Lets Write some HTML!
- Make a large header with the name of your site using an `<h1>` element
- add a photo using the `<img>` element (remember `img` doesn't need a closing tag)
- make a paragraph using the `<p>` element
- make a smaller page header using the `<h2>` element
- make an ordered or unordered list using the `<ol>`,``ul``, and `<li>` elements

## CSS Basics


###### CSS Examples:

this example targets an element `h1` and changes the font size, font weight, and color. 

```
h1 {
    font-size: 24px;
    font-weight: bold;
    color: #000000;
}
```
This example targets a class `btn` to change the background color and add padding

```
.btn {
  background: #829aa8;
  padding: 10px;
}
```
This example targets an ID `profile-picture` to change the width:

```
#profile-picture {
  width: 200px;
  }
  
```

Learn more CSS [here](https://www.w3schools.com/css/)

###### CSS Grid

Its best practice now days to make sure your site if mobile responsive. It used to be common to use a 3rd party library like Bootstrap to make a grid system to change where content is placed on a website depending on the size of the screen. It was also possible to do this using some simple math and [media queries](https://www.w3schools.com/css/css_rwd_mediaqueries.asp), but now its even simpler and easy to do with [CSS Grid](https://www.w3schools.com/css/css_grid.asp)!



Basic Grid example:

```
  .grid {
    max-width: 800px;
    margin: 45px auto;
    display: grid;
    grid-gap: 20px;
    grid-template-columns: 100px 100px 100px;
    grid-template-rows: 200px 200px 200px 200px;
    padding: 20px;
}

```

Flexible space implicit example:

```
  .grid {
    max-width: 800px;
    margin: 45px auto;
    display: grid;
    grid-gap: 20px;
    grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
    grid-auto-rows: 200px;
    padding: 20px;
}
```

Use repeat function

repeat(3, 1fr)



###### CSS Animations:







Learn more CSS [here](https://www.w3schools.com/css/)

## Lets Write some CSS!
- change the width of your image
- change the background color
- change the font color
- style our link
- align everything center (did everything align center?)

## Congratulations

Awesome job! You made a web page! You're a web developer! :)

you can see the completed codepen example [here](https://codepen.io/sagecodes/pen/PBvLvY?editors=1100) or look in the example folder in this repo.

## Challenge:
The best way to learn is to keep practicing and challenge yourself! Here are some ideas!

- Design a new layout
- Use multiple CSS grids on your site!
- use CSS [transitions](https://www.w3schools.com/css/css3_transitions.asp) and [animations](https://www.w3schools.com/css/css3_animations.asp)

Show off your project at the next [code hours](https://www.meetup.com/Learn-Code-Seattle/events/)!




## Upcoming Events!
We host sooo many events! check out out [calendar](https://www.galvanize.com/seattle/events)

[Learn code](https://www.meetup.com/Learn-Code-Seattle/events/). Thats this meetup! We do workshops and community programming nights! 

Upcoming Learn to code [events](https://www.meetup.com/Learn-Code-Seattle/events/):

- [Code Hours](https://www.meetup.com/Learn-Code-Seattle/events/253455813/) - 8/21 6:30pm
- [Intro to SQL](https://www.meetup.com/Learn-Code-Seattle/events/253466201/) - 8/30 6:30pm 
- [Intro to Javascript](https://www.meetup.com/Learn-Code-Seattle/events/253466275/) - 9/06 6:30pm
- [Intro to Git and GitHub](https://www.meetup.com/Learn-Code-Seattle/events/253466429/) - 9/19 6:30pm
- [More!!!](https://www.meetup.com/Learn-Code-Seattle/events/)

## What is Galvanize?
###### We are a community!
#### Immersive Bootcamp
- [Data Science](https://www.galvanize.com/seattle/data-science)
- [Web Development](https://www.galvanize.com/seattle/web-development)

#### Part-Time Courses
- [Data Analytics](https://www.galvanize.com/seattle/data-analytics)
- [Web Development Foundations with JavaScript](https://www.galvanize.com/seattle/web-development-foundations)
- [Data Science Fundamentals](https://www.galvanize.com/seattle/data-science-fundamentals)



#### Co-working Space
[work in our building!](https://www.galvanize.com/entrepreneur)

## Questions:
Please feel free to reach out to me with any questions!

- Twitter: [@sagecodes](https://twitter.com/@sagecodes)
- LinkedIn: [sageelliott](https://www.linkedin.com/in/sageelliott/) 
- Email: [sage.elliott@galvanize.com](mailto:sage.elliott@galvanize.com)
