# Fundamentals of Big Band Drumming
## Portfolio Project 1: HTML/CSS Essentials
![images of website on different devices](assets/images/responsive-screens-website.jpg)

This project is built as part of the Code Institute Full Stack Software Development course. For this course, 
Dirk Ornée had to build a first Portfolio Project. He choose to build a project that combines his knowledge as a professional musician, with his knowledge gained troughout the course. 

## Live Site
[Fundamentals of Big Band Drumming](https://dodrums.github.io/PortfolioProjectOne/index.html)

## Repository
https://github.com/DOdrums/PortfolioProjectOne

***

## Table of Contents

- [Fundamentals of Big Band Drumming](#fundamentals-of-big-band-drumming)
        - [Table of Contents](#table-of-contents)
  - [UX](#ux)
    - [Business goals](#business-goals)

# UX
## Business goals
The main goal for this project, is to develop a valuable resource for drummers and conductors, to learn about big band drumming. The website should be able to provide a helicopter view of what big band drumming is like, how it should be approached and what it should sound like. This should help conductors in giving pointers to drummers during rehearsals and should improve the playing of big band drummers who aren't very experienced yet.
The second goal is to show my competency as a developer using HTML & CSS.

## Target Audience
Drummers and Conductors are the main target audience, since the website really aims to help them specifically in understanding the function of a big band drummer better. However, anybody with some knowledge or just a general interest in big band music should be able to enjoy this website and learn something.

## User Stories

### As the owner:

* I want to share my knowledge about big band drumming and keep everything I have learned over the years in one place (the website).
* I want the user to really dive in, get interrested in the topic and get inspired to do more research by themselves.
* I want the user to learn the fundamentels of big band drumming through this website, so they can use this information in a pragmatic way to develop their own style and preferences. 
* I want to build a relationship with users, where they can contact me through the contact form if they have more questions, so I can help them out with anything drumming related. 

### As a new user:
* I want to navigate the site easily and intuitively, without having to wonder what the purpose of the site is.
* I want to be redirected through the pages in an intuitive way, having a logical hierarchy to follow in order to learn everything I can from the website 
* I came to this website specifically to learn about big band drumming, especially about topics within big band drumming which are hard to find recources for.

### As a returning user:
* I want to return to the information, to see if I'm already incorporating everything in my playing or conducting. 
* I want to re-listen to the audio, to see if now that I have tried to use the information in pracitce, I start to recognize more of the information learned in the audio itself.
* I want to contact the author, for any further questions I have.

# Structure of the website

The website is designed to give a good hierarchical flow. This means that after reading the homepage, the user will go to the second page (Reading & Playing) and read through this information. On the bottom of that page they will be prompted to continue to the Three Drummers page, which is the logical place to continue, as it builds on the information read in the Reading & Playing page. The pages however can also be used just by themselves, they both contain enough information to stand on their own. 
Furthermore, the website is made fully responsive, so it functions on any device. That being said, as you'll be reading sheet music on the Reading & Playing page, a bigger screen is more fitting for that type of content. 

## Credits

To be able to build this project in gitpod, I used the template made by Code Institute, as found here: [full template](https://github.com/Code-Institute-Org/gitpod-full-template)

Other websites I used for inspiration and general coding examples and knowledge:
* [w3schools](https://www.w3schools.com/)
* [awwwards](https://www.awwwards.com/)
* 

### Code
* Nav bar inspiration and hero-image animation was taken from the love running walkthrough project
* The CSS code `margin-left: calc((100% - 600px) / 2);` to center paragraphs on page 2 and 3 was taken from the NYtimes website, which uses this code to center text in their articles
* The CSS code to make the youtube video responsive for screen sizes 767px and under, was taken from this website: [make youtube video responsive](https://avexdesigns.com/blog/responsive-youtube-embed) 

## Bugs
* After finishing page 2 of the website, I noticed that the line underneath the nav bar was suddenly cut in half. This was caused by a bottom-margin property being added to the main font selector (which includes the nav element). This was solved by making a selector that contains a negative bottom-margin to the ul and il child elements of the nav element and by adding a nav selector that contains a bottom-margin of 0.
* The thumbnail of the youtube video would dissapear in and out of frame partially when resizing the window. After some playing around in the chrome dev tools, I discovered this was due to the width being set to a percentage setting instead of pixels. I changed it to pixels and now the thumbnail stayed sized the same no matter the window size.
* There was a problem with the hero image after resizing it to fit tablet sizes. The hero image was now zooming into the div below instead of behind it. This was because I changed the height setting of hero-image id but not of the hero-outer id.
* There was a problem with the figcaption under the count basie image not aligning. This happened because I moved around CSS rules insize the media query section, and misplaced a bracket because of that. This misplaced bracket made two CSS rules fall outside of the media query and were now applied project-wide. It took a while to find what caused this, but Chrome Developer tools made it quite easy to see that the wrong styles were being applied at bigger screen sizes.