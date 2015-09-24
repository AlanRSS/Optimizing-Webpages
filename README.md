## Website Performance Optimization portfolio project

Your challenge, if you wish to accept it (and we sure hope you will), is to optimize this online portfolio for speed! In particular, optimize the critical rendering path and make this page render as quickly as possible by applying the techniques you've picked up in the [Critical Rendering Path course](https://www.udacity.com/course/ud884).

To get started, check out the repository, inspect the code,

### Getting started
*To get the website fork the repository from https://github.com/AlanRSS/frontend-nanodegree-mobile-portfolio
*Download the repository 
*To run the Website Simply open index.html with your favourite browser

Some useful tips to help you get started:

1. Check out the repository
1. To inspect the site on your phone, you can run a local server

  ```bash
  $> cd /path/to/your-project-folder
  $> python -m SimpleHTTPServer 8080
  ```

1. Open a browser and visit localhost:8080
1. Download and install [ngrok](https://ngrok.com/) to make your local server accessible remotely.

  ``` bash
  $> cd /path/to/your-project-folder
  $> ngrok 8080
  ```
  1. Copy the public URL ngrok gives you and try running it through PageSpeed Insights! Optional: [More on integrating ngrok, Grunt and PageSpeed.](http://www.jamescryer.com/2014/06/12/grunt-pagespeed-and-ngrok-locally-testing/)

*Happy Browsing!
####Part 1: Optimize PageSpeed Insights score for index.html


*Optimized image sizes
*Deleted web Fonts and minified the page scripts
*JS running Async and inlined critical CS
*minified scripts
*PageSpeed 95 mobile - 98 Desktop

####Part 2: Optimize Frames per Second in pizza.html
Steps to get 60 FPS:
1st Problem: FSL on pizza resize
Fix:
*Change the Method to update sizes using percentages instead of making the insane calculation that were unnecessary.
*Read the layout properties outside of the loop and batch changes after

2nd Problem: Janky scrolling 
Fix:
*Ilya's method was reading properties inside the loop causing a lot of jank
*Create a variable to store the layout properties batch changes in loop
*add will-change property to let the browser know that an animation will take place
*method that creates background pizzas now dinamically generates the right amount to fill the screen size based on resolution of browser



60FPS Achieved 
Other optimizations:
*Use strict on all functions
*moving variables declared inside loops to outside in order to reduce redundancy
*removed queryCollector and inserted getElementbyId on moving Pizzas in the Update position method 
Profile, optimize, measure... and then lather, rinse, and repeat. Good luck!

### Sample Portfolios

Feeling uninspired by the portfolio? Here's a list of cool portfolios I found after a few minutes of Googling.

* <a href="http://www.reddit.com/r/webdev/comments/280qkr/would_anybody_like_to_post_their_portfolio_site/">A great discussion about portfolios on reddit</a>
* <a href="http://ianlunn.co.uk/">http://ianlunn.co.uk/</a>
* <a href="http://www.adhamdannaway.com/portfolio">http://www.adhamdannaway.com/portfolio</a>
* <a href="http://www.timboelaars.nl/">http://www.timboelaars.nl/</a>
* <a href="http://futoryan.prosite.com/">http://futoryan.prosite.com/</a>
* <a href="http://playonpixels.prosite.com/21591/projects">http://playonpixels.prosite.com/21591/projects</a>
* <a href="http://colintrenter.prosite.com/">http://colintrenter.prosite.com/</a>
* <a href="http://calebmorris.prosite.com/">http://calebmorris.prosite.com/</a>
* <a href="http://www.cullywright.com/">http://www.cullywright.com/</a>
* <a href="http://yourjustlucky.com/">http://yourjustlucky.com/</a>
* <a href="http://nicoledominguez.com/portfolio/">http://nicoledominguez.com/portfolio/</a>
* <a href="http://www.roxannecook.com/">http://www.roxannecook.com/</a>
* <a href="http://www.84colors.com/portfolio.html">http://www.84colors.com/portfolio.html</a>
