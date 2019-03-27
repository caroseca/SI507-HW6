blah blah blah # JavaScript assignment

## Some useful resources
* Some [JavaScript tutorials](https://www.htmldog.com/guides/javascript/)
* The complicated [resources in the You Don't Know JS](https://github.com/getify/You-Dont-Know-JS) series, including [your reading last week](https://github.com/getify/You-Dont-Know-JS/blob/master/up%20%26%20going/ch2.md)
* [A resource for CSS/style/colors](https://htmlcolorcodes.com/)  
* [An excerpt from a specific workshop site](https://witny-summer-guild-2018.github.io/day_4_exercise_2.html) (for a different audience than yourselves) which addresses some common questions about jQuery
* [The simple JSFiddle example from class](https://jsfiddle.net/2of65j8q/)
* A [W3Schools resource on JavaScript output](https://www.w3schools.com/js/js_output.asp)
* Google, Piazza, your classmates, office hours, lab time!

## Included files
* This `README.md`, which you should edit with answers to the questions
* `jsPracticeLab.html`, which you'll need to edit and try out
* `jquerylib_submit_example.html`, which you'll need to edit and try out

## Your goals for this lab

### Broadly
The aim for this lab is to practice adapting to and understanding code in a new-to-you (or not) language and its own libraries/packages -- JavaScript, in this case.

The programming skills you have built up till now are useful for *Python programming*, but, more than that, they extend to fundamentals of many kinds of programming.

This experience is *not in any way* about becoming an expert JavaScript programmer. Instead, it is about using what you *do* have experience with -- and your skills in *learning new things* that relate to programming -- in order to make educated judgments about some brand new-to-you code, even if you haven't learned in detail about it yet. That's part of what being in technology -- or even technology-adjacent -- will often mean.

### Specifically

Below are a bunch of questions and indications of things to do. For each indication of something to do with code, there is also an accompanying question to answer or brief explanation to give.

**To complete and submit this assignment, you should:**

* ~~Fork (and clone) this repository~~
* ~~Add our instructional team as a collaborator to your fork (see instructions for adding collaborators on Canvas)~~
* Edit this `README.md` file with answers to the questions/prompts, briefly, using Markdown formatting so that the questions appear in bulletpoints and the answers appear clearly below each respective question, *not* as bulletpoints.
* Add all names of those who worked on this (as indicated below)
* Make the changes that are indicated below to each of the `.html` files with JavaScript programs provided. (You'll probably do this concurrently with answering questions)
* Commit (as you go) and push your changes to all three files to your GitHub forked repository.
* Submit a link to your repository on Canvas. (This HW doesn't have an autograder -- it will be graded by hand/by humans this time.)

### Important notes
* You are *more than* welcome to work together on this, but **you must <b><u>each</u></b> submit a repo to be graded on it**, so if you do work together, you should do the following:
	* Make sure each one of you understands all the work -- YOU are responsible for using and knowing this information
	* Write each person's name & uniqname who worked on the assignment together on your submitted `README.md` file (you'll see a space for this below)

* In answering questions, please make sure the formatting is clear to read and that you have updated the names of everyone who worked with you, with your name first (see below).

* In answering questions, assume all of the questions include a *explain briefly* note -- you do NOT have to, and should not, write extended paragraphs. Be as concise as you can and explain in your own words. Don't worry about "whether it's enough" -- just worry about conveying your understanding so you can read it later, or even give it to someone else, and the answers will help/make sense.

* It is not acceptable to copy and paste answers from the internet and submit them as your own. If you cite things, make sure you provide a citation, including to links. If you get information from a resource and rephrase it so you're basically explaining an idea, that's just fine for an explanatory purpose in this assignment, but you *must* cite any quotes or examples that aren't yours.

* **For grading:** we are grading on...
	* Following the instructions
	* Approximate correctness of the code edits
	* Careful & clear answers to the questions
	* Correct answers to the questions
	* Slightly more than half the 1000 points will come from answering the questions. The rest will come from your edits to the code.

### Names of people you have worked with on this assignment
* List everyone's names and uniqnames who have worked on this assignment with you, **including your own name, but make sure YOUR name is first and bold**
* Like this:
* **Jackie Cohen (jczetta)**
* Yea-Ree Chang (cyearee)
* Ruchi Ookalkar (ruchido)
* Innocent Obi (innoobi)
* Zhen Wang (alejwang)
* etc.

## Questions & code instructions

### The first questions address the `jsPracticeLab.html` file.

* **This is just an example question.**

This is what an example answer should look like. If you want to include some code, which you probably don't have to do, you can, like this:

```js
Some JavaScript code
```

* **What does a code comment look like in JavaScript? What character/s do you have to put before a comment?**

Comments look like this: ```//``` (forward slashes)

* **Explain what needs to happen to get a JavaScript program to "run", given the JavaScript you've seen in this assignment.**

First, the script type needs to be identified as such ```<script type="text/javascript">```. Also, in this particular code, everything starts to get moving with the onload function: ```<body onload = "displayInformation();">```.

* **What functions in JavaScript seem to be similar in function to the `print` function in Python? (There are two.) Why might you use one and not the other? Explain briefly.**

Seems to be like ```console.log()``` and potentially ```alert(hello)```. console.log will print out some statements in the browser's console, but alert will display a pop-up in the browser window. The latter may be annoying and not in the scope of the design for the webpage, so that may not be the outcome that you want.

* **What code would have to comment out to get rid of the pop-up box when you load the page? (Related to the last question.) ~~Do that in the code file, and then, add code so that a text box will appear that contains the current date and time! *HINT:* Look through the rest of the code first...~~**

Commented out line 11, ```alert("hello");```.
* **How can you put your own name at the top where it currently says "A name"? Explain very briefly how to do so, and ~~replace `A name` in the web page with your own name.~~**

The javascript code that targets the h1 tag needs to/did change: ```document.querySelector('h1').innerHTML = "CARA R. CANADY";```

* **What does the word `document` represent in this code? Explain briefly.**
Using https://www.w3schools.com/js/js_htmldom_document.asp on 03/19/2019 to inform my answer. The DOM is the document object module. Using this targets/controls elements/items in the HTML document and allows javascript to modify those objects/elements.

* **What is happening in line 12 (**
		`document.querySelector('#items').innerHTML = document.getElementsByTagName('li').length`
)? **Explain, briefly (<= 2 sentences).**

This line finds out how many items are contained within the list tag and identifies those items with an ```#items``` tag.

* **What color would the background of this page be <u>if there were no JavaScript in this page</u>?**

The background color of this page is white without javascript; the CSS stylesheet gives a grayish color to the <p> tag only.

* **Why are there a couple of gray boxes on the screen with a different colored border? How could you edit this code to make them a different color? Explain briefly. ~~Then edit the code to make those boxes some shade of blue, of your choosing.~~**

The <p> tag is included in the CSS stylesheet, so it only targets those HTML elements with that tag. The border size, type, and, color are also included in that styling. Changed the color of the boxes to blue.

* **Edit the code so that, if you highlight `McGill University` and copy it, you see the text `O Canada` near the bottom of the page. Briefly explain why you made the edits that you did -- how did you know/figure out what to do?**

Done! I referenced the oncopy() event handler for Umich and created something similar for McGill.

* **In the original code, when you click the button that says `Wow`, you see a text box! Wow. Explain briefly in your own words why the following code causes that to happen:**

```js
function handleClick(){
	alert("hello");
}
```
**and**

```js
<button onclick=handleClick() id="wow-button">Wow</button>
```

First, the function handleclick() creates the alert. Second, the button element creates an HTML button, which contains an onclick event that executes the handleClick function when the button is depressed. This button is given an id called "wow-button" for stylization/further targeting, and the text inside the button reads "Wow".

* **Knowing what you learned from the previous question, ~~add code/markup to the `jsPracticeLab.html` file *so that* there is a button with the text `Spring Equinox 2019` on it somewhere on the page, and when that button is clicked, a text box containing the text `March 20, 2019` appears.~~ (There's no function -- that I am aware of -- to automatically get this info, you've got to type it yourself.)**

Done! Also gave it a pretty color. :)

### The next few questions address the `jquerylib_submit_example.html` file.

* **Check out the file `jquerylib_submit_example.html`. This is an example of code that uses a package called `jQuery` (and this will need you to have an internet connection to run it properly, although the other file does not). Check out resources above for more on jQuery!**

Done. I've worked with jQuery before, so this is a good refresher. jQuery allows javascript and HTML to interface more seamlessly imo.

* **When you enter input that isn't valid, you see an error that is red. Why is the error in red? Why is the response for valid inputs blue?**

There's a  conditional statement set up that checks to see if the currentValue is one word. If it isn't, the paragraph that appears falls into the class "error"; the CSS indicates that the text should turn red. The javascript indicates that the html should show and then fadeout. Similarly, if the test **is** true, the 'else' part of the conditional statement kicks in and the paragraph with the "nice!" text is assigned a class value of "good" - this also appears and then fadeouts according to the jQuery in line 25. The CSS (or <style> tags) dictate that anything assigned to this class should turn blue.

* **What is this line `var regex = /^[a-zA-Z]+$/;` helping with? And if you googled something to figure that out, what did you google, and what, briefly, did you learn? (If you didn't need to google, you can leave that out, but explain briefly what that line is helping the program do, anyway.)**

I actually looked this up when I was trying to figure out some sql at work that would allow me to find values (strings) that start with a number and filter them out. Here's where I looked: https://docs.oracle.com/cd/B12037_01/server.101/b10759/conditions018.htm, and I googled "character match string sql oracle."


* **What's different about the syntax of conditional statements in JavaScript, compared to Python?**

A few things: (1) so many curly brackets in javascript (2) no colon (:) in javascript (3) I found out the hard way that indentations matter in python (reraise error after reraise error).

* **What do you think the `10000` refers to in the code `.fadeOut(10000)`?**

That's the time before it fades away (duration). I knew this from my previous front-end bootcamp.

* **What do you think is going on with the following code at the beginning of the program? Note that the most important thing to do for answering this question is to be thoughtful and clear, not to be absolutely correct:**

```
js
$(document).ready(function(){
$("form").submit(function(event){
```
This seems to call a function when the document is ready. This function targets the `form` element specified in the HTML. The submit method that is attached to `$("form")` executes a function when the form is submitted (button is pressed) - this leads to the valid/not valid text that appears.

~~ * **Add some code to the `jquerylib_submit_example.html` file so that, if the input is valid and is specifically the text `hello`, rather than the visible output being `Nice!` in blue, the visible output should be `Hello to you too!`, also in blue, just like `Nice!` is.** ~~
~~ * *HINT:* You'll have to make some changes to the conditional statement, and possibly look up some JavaScript conditional syntax. You'll also need to look carefully at what generates visible output right now. ~~

```
hello
