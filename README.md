# Fundamentals of Big Band Drumming
## Portfolio Project 1: HTML/CSS Essentials
![responsive images of website](assets/images/responsive-screens-website.jpg)

This project is built as part of the Code Institute Full Stack Software Development course. For this course, 
Dirk Ornée had to build a first Portfolio Project. He choose to build a project that combines his knowledge as a professional musician, with his knowledge gained troughout the course. 

[click here to go to a working link of the website](https://dodrums.github.io/PortfolioProjectOne/index.html)

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
* Nav bar inspiration and hero-image animation was taken from the love running walkthrough project
* The CSS code `margin-left: calc((100% - 600px) / 2);` to center paragraphs on page 2 and 3 was taken from the NYtimes website, which uses this code to center text in their articles
* The CSS code to make the youtube video responsive for screen sizes 767px and under, was taken from this website: [make youtube video responsive](https://avexdesigns.com/blog/responsive-youtube-embed) 

## Bugs
* After finishing page 2 of the website, I noticed that the line underneath the nav bar was suddenly cut in half. This was caused by a bottom-margin property being added to the main font selector (which includes the nav element). This was solved by making a selector that contains a negative bottom-margin to the ul and il child elements of the nav element and by adding a nav selector that contains a bottom-margin of 0.
* The thumbnail of the youtube video would dissapear in and out of frame partially when resizing the window. After some playing around in the chrome dev tools, I discovered this was due to the width being set to a percentage setting instead of pixels. I changed it to pixels and now the thumbnail stayed sized the same no matter the window size.
* There was a problem with the hero image after resizing it to fit tablet sizes. The hero image was now zooming into the div below instead of behind it. This was because I changed the height setting of hero-image id but not of the hero-outer id.
* There was a problem with the figcaption under the count basie image not aligning. This happened because I moved around CSS rules insize the media query section, and misplaced a bracket because of that. This misplaced bracket made two CSS rules fall outside of the media query and were now applied project-wide. It took a while to find what caused this, but Chrome Developer tools made it quite easy to see that the wrong styles were being applied at bigger screen sizes.