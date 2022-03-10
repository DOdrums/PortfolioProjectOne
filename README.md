# Fundamentals of Big Band Drumming

This project is build as part of the Code Institute Full Stack Software Development course. For this course, 
Dirk Ornée had to build a first Portfolio Project. He choose to buil a project that combines his knowledge as a professional musician, with his knowledge gained troughout the course. 

click here to go to a working link of the website

##### Table of Contents

- [Fundamentals of Big Band Drumming](#fundamentals-of-big-band-drumming)
        - [Table of Contents](#table-of-contents)
  - [UX](#ux)
    - [Business goals](#business-goals)

## UX
Some text about UX

### Business goals

## Credits

To be able to build this project in gitpod, I used the template made by Code Institute, as found here: [full template](https://github.com/Code-Institute-Org/gitpod-full-template)

Other websites I used for inspiration and general coding examples and knowledge:
* [w3schools](https://www.w3schools.com/)
* [awwwards](https://www.awwwards.com/)
* 

### Code
* Nav bar inspiration was taken from the love running walkthrough project
* The code `margin-left: calc((100% - 600px) / 2);` to center paragraphs on page 2 and 3 was taken from the NYtimes website, which uses this code to center text in their articles

## Bugs
* After finishing page 2 of the website, I noticed that the line underneath the nav bar was suddenly cut in half. This was caused by a bottom-margin property being added to the main font selector (which includes the nav element). This was solved by making a selector that contains a negative bottom-margin to the ul and il child elements of the nav element and by adding a nav selector that contains a bottom-margin of 0.