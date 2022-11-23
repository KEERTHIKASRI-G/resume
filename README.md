# Build a Website to Showcase your Resume

## Overview

Want to make your application stand out to recruiters? let me walk you through how to code a resume website. The best part is that you don't have to download any coding tools or know any programming languages to get started. 

Using the power of **github.dev**, a service that allows you to work with files in GitHub, and GitHub Pages, you'll code a resume website using only your browser window. By the end of the workshop, you'll be able to send anyone a link where they can view your resume online. 

#What will you learn
 Basics of HTML and CSS to showcase your skills in an online resume
#What you'll need
A modern web browser like [Microsoft Edge](https://www.microsoft.com/edge?WT.mc_id=academic-51109-ornella) or [Google Chrome](https://www.google.com/chrome/) and a [GitHub account](https://github.com)

## Final Project
By the end of this workshop, you'll have created a resume web site that will look like this:

![microsoft resume](https://user-images.githubusercontent.com/111286854/203629378-7966e474-a38d-479c-8fc4-efc3b3430aca.png)

## Outline
In this workshop, you will: 
* Set up your coding environment
* Learn basic HTML to outline your resume
* Fill in your resume content
* Style your resume with CSS
* Create your resume website with GitHub Pages

Let's get started!


# Steps For Creating the HTML Code
# Create an HTML page

HTML stands for Hypertext Markup Language, and is used to "markup" the text to be displayed on a webpage. More specifically, HTML is used to describe the hierarchy and function of the text in a page. With HTML you can indicate a header, create a link to another page, or indicate where an image should be placed.

HTML consists of what are called "tags" or "elements". While there is a technical difference between the two, you will find many developers use the terms interchangeably and generally doesn't impact how you create your code. These tags are read by a browser and are used to determine how to display and interpret the information in a page.

You will begin to build your resume by creating an HTML file and adding the code. You may notice that the page won't appear to be very structured or robust; you will make it look better when you add some styles.

## Create an HTML file with CodeSwing

You will use CodeSwing to create and edit your HTML and CSS in Visual Studio Code. CodeSwing has a variety of templates you can use and includes support for advanced pages as well. Start by creating your first "swing" using the core HTML template.

1. Open the **Command Palette** by selecting the three parallel lines icon in the left-hand side Activity Bar, then navigating to **View > Command Palette**. You can also quickly open the Command Palette by using the keyboard shortcut **Control+Shift+P** on a PC, or **Command+Shift+P** on a Mac.
1. Type **CodeSwing**, then select **CodeSwing: Initialize Workspace as Swing**.
1. Choose the option for **Basic: HTML-Only** and your new swing will appear, with your HTML file on the left and a browser window on the right.
1. This will create an **index.html** file in your root directory.

> **IMPORTANT** If you accidentally close the wrong windows, you can re-open CodeSwing by navigating to your repository in github.dev, opening the Command Palette with **Control+Shift+P** (or **Command+Shift+P** on a Mac), typing **CodeSwing**, selecting **CodeSwing: Open Swing...**, and selecting the directory with your files.

You now have the HTML file created for your resume site!

## Create the HTML structure

Let's start adding the HTML for our page. Every HTML page includes three main tags - `html` which contains all the HTML, `head` which includes information about the page, and `body` which contains the contents to display on the page. Tags can also contain **attributes**, which allow us to change how a tag behaves. Attributes are key/value pairs such as `rel="stylesheet"`.

> **Note:** You may notice some of the names are a little cryptic or not necessarily intuitive. This is partly due to the history of HTML. HTML was originally used by scientists and academics as a way to structure documents. As a result, the names or abbreviations used might not always be as clear as we might like.

Most tags have an open (`<tag>`) and a close (`</tag>`), and contain information. So `<title>Demo title</title>` indicates the title of the page. Others will only have a single tag, such as `<link rel="stylesheet" href="style.css">`. These types of tags behave much like a command, telling the browser to perform a particular task.

> **Tip:** Don't try to memorize every tag available. Just as memorizing a dictionary isn't a good way to learn a spoken language, memorizing a set of keywords isn't going to aid you in your growth as a developer. As you continue to create pages you'll learn more tags and how they behave.

You're going to use these three tags (and a couple of others) to begin the creation of your resume. We'll explain the tags we're using after we create the page.

1. Inside the **index.html** window, add the following code to create the initial structure of your page, replacing **Your Name** in the `<title>` tag with your name:

    ```html
	<html>
	<head>
        

		<link href="style.css" rel="stylesheet">
		<title>keerthika resume</title>
        <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.4/css/all.min.css">
	</head>

	<body>
		<header id="header">
			<!-- resume header with your name and title -->
			<div class="profile_profileImg">
            </div >
            <div class="h"><h1>KEERTHIKASRI</h1></div>
			<hr>
			<h2 style="border:2px solid rgb(103, 195, 241);background-color: white;color: rgb(76, 177, 213);">SOFTWARE ENGINEERING STUDENT</h2>
			<hr>

		</header>

		<main>
			<article id="mainLeft" style="background-color:rgb(80, 193, 222)">
				<section>
					<h2><b>CONTACT</b></h2>
					<!-- contact info including social media -->
                    <p>
                        <i class="fa fa-envelope" aria-hidden="true"></i>
                        <a href="mailto:your-email@example.com">2012115@nec.edu.in</a>
                    </p>
                    <p>
                        <i class="fab fa-github" aria-hidden="true"></i>
                        <a href="github.com/gh-username">gh-keerthikasri</a>
                    </p>
                    <p>
                        <i class="fab fa-linkedin" aria-hidden="true"></i>
                        <a href="linkedin.com/linkedin-username">KEERTHIKASRI</a>
                    </p>
				</section>
				<section>
					<h2><b>SKILLS</b></h2>
					<ol>
                        <li>drawing</li>
                        <li>leadership skills</li>
                        <li>management skills</li>
                        <li>communication skills</li>
                    </ol>
				</section>
				<section>
					<h2><b>EDUCATION</b></h2>
					<!-- your education -->
                    <h3><b>College:</b></h3>   
                    <p>National Engineering College</p>
                    <p>2020 - 2024</p>   
                    <br>      
                    <p>Bachelor of Engineering in 
                        Computer Science <b>(Pursuing) </b> Kovilpatti – 628 503. |
                         <i>CGPA : 8.48<i></i>
                         </i></p>
                         <br>
					<h3><b>Secondary:</b></h3>	
					<p>Mahatma Baba Building Mat. Hr. Sec. School, Madurai – 628 107.</p>
				</section>
			</article>
			<article id="mainRight">
				<section>
					<h2><b>ABOUT</b></h2>
					<!-- about you -->
					<p>To commit a professional job where I can utilize my field of study and work experience, share, and at the same time
					 cultivate my humble knowledge order to expand my understanding of discipline that I have chosen. To enable me to grow 
						intellectually, morally and emotionally in new working environment.</p>
				</section>
				<section>
					<h2><b>WORK EXPERIENCE</b></h2>
					<!-- your work experience -->
                    <ul>
                        <li>Student Lean Ambassador | Microsoft</li>
                        <li>Campus Ambassador | Interestopedia</li>
                        <li>Campus Ambassador | People North</li>
                        <li>Campus Ambassador | Skil Lync</li>
                        <li>Campus Ambassador | Learneca</li>
                    </ul>

                    <h2><b>ACHIEVEMENTS
                    </b></h2>
					<ul>
						<li>Emerging participant award as a entrepreneur in ryla organized by the rotatory clud of virudhunagar</li>
						<li>best volunteer award by National service scheme
						</li>
						<li>Recognised as a WINNER in the IITB-ISRO-AICTE Mapathon, an initiative of the FOSSEE project,IIT Bombay in association with ISRO and AICTE</li>
					</ul>
		
				</section>
			</article>
			<article>
				Phone number: +91 -6374821748
			</article>
		</main>
		</body>
        </html>
         ```

1. Notice how as you type (or copy and paste), the browser window on the right automatically updates with the information you've added.

### Exploring the code

You used several tags to display your new page. Below is a table that describes each of these tags and what it is used for. As you look at the code, notice that the HTML is in all lower case letters, and that you use tabs to create an outline for the code. While this isn't required, it does make your HTML much more readable.

| tag                          | description                                                                                                                                                                                                      |
| ---------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `html`                       | Container for all HTML in an HTML page.                                                                                                                                                                          |
| `head`                       | Contains metadata, or information about the page.                                                                                                                                                                |
| `link`                       | Used to tell the page what CSS stylesheet to use. `rel="stylesheet"` indicates we are using a stylesheet, and `href="style.css"` loads **style.css** (which is the name of the stylesheet we'll create in the CSS section of the workshop). |
| `title`                      | Indicates the title of the page to display on the toolbar. This is **not** displayed on the page itself. Every page you create should have a title.                                                              |
| `body`                       | The contents of the page to be displayed to the user.                                                                                                                                                            |
| `header`, `main`, `article`, `section` | These are "semantic" tags. See the description below for more information.                                                                                                                                              |
| `h1`                         | A level 1 header. Header tags go from `h1` to `h6`, with `h1` being the highest level, to `h6` being the lowest level. These are used to create structure for the outline of the page. |
| `p` | A paragraph tag. Paragraph tags are where the body text of your page goes.
| `hr` | Creates a horizontal line. The tag stands for "horizontal rule".
| `id` | `id` is an attribute that allows you to assign a unique id for an HTML element. This will come in handy when we style the HTML. 
| `<!-- comment -->` | These are HTML comments. They are useful for making notes or setting reminders to yourself.

> **Note:** Comments are a great way to take notes as you're learning HTML. You can put a comment right above a section of code, and describe what the section does. But do remember comments **are not** hidden from browsers, so don't store sensitive information in comments as anyone who views the source of your code can read your comments.

#### Semantic tags

Semantic tags are a relatively new addition to HTML. You may notice on the page there is a difference in size between `h1` and `h2`. This is because besides just indicating a level, header tags also modify how content is displayed. Semantic tags such as `header`, `main`, `article` and `section` are only used to group information together. Semantic tags are useful to structure a large HTML document, and later use CSS to control how the content will actually get displayed.

You can use semantic tags however you wish, but a common hierarchy is:

- `header`
- `main`
    - `article`
        - `section`

> **Note:** Semantic tags are also very important in making your web pages 'accessible', or more easily read by screen readers so that all users, including those with disabilities, can access your web pages. Read more about making your web pages accessible [in this article](https://developer.mozilla.org/docs/Learn/Accessibility/HTML).

## Summary and next steps

You've now created your first HTML page! Next, [add additional content](./2-add-content.md) such as your email address and sections for your professional experience.
