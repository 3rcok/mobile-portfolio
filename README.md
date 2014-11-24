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
* I used a variable to cache the scrolltop value on line 508 of the main.js file to improve the frames per second
