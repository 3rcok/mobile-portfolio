## Website Performance Optimization portfolio project

I downloaded the source code from https://github.com/udacity/frontend-nanodegree-mobile-portfolio

### Steps I took to optimise the portfolio

* optimised images by using tinypng.com
* because print.css and style.css are so small it made no sense to have them in separate files, so I combined them into one
* moved js scripts to the bottom of the html file and made them async
* used inline css
* as perfmatters.js is so small, I have integrated it into the html
* I used grunt to minify js and css - the output is in the respective build folders but non-minified versions are also included for better readability
* There were various images that were linked to on the internet. I changed these to local images which have been optimised
* I replaced images on index.html with sprites
* I inlined the css in the pizza.html document
* I used a variable to cache the scrolltop value on line 508 of the main.js file to improve the frames per second
* I cached the variables for width and new width of pizza size on line 455 of the main.js file for faster resizing
* I updated the updatePositions function to only draw pizzas in the viewport and to break the loop if the size is bigger than the viewport on line 515 of the main.js file
* I added a sepparate variable for the basic top height without the px for the faster use of the variable in the updatePosition function on line 549 of the main.js file


###Testing the performance
   
* The improved portfolio can be accessed on http://firzhugh.github.io/mobile-portfolio/project-mobile.html
* To test the page speed I used the following sites:
    * https://developers.google.com/speed/pagespeed/insights
    * http://www.webpagetest.org/
* To check the frames per second I used Google Developer Tools