## Website Performance Optimization portfolio project

Get started by either:
1. Check out the repository and run a local server

$> cd /path/to/your-project-folder
$> python -m http.server 8080
Open a browser and visit localhost:8080

Download and install ngrok to make your local server accessible remotely.

$> cd /path/to/where-ngrok-resides
$> ngrok 8080

Forwarding denotes the website where you have published online.
Copy the website given to your browser

2. View the GitHub Pages link to the project:

http://cgolden.github.io/udportfolio/views/pizza.html

Cam's Pizzeria website allows viewing and selection of pizzeria information
and menu of a wide variety of ingredients. Also, size selection (small, medium, and large) is allowed by moving the size bar left or right.  Scroll through the page to review the many options!

Cam's Pizzeria Website Optimizations
Pizza.html
1. Resized and compressed the pizzeria image
2. Compressed the pizza image
3. Modified style.css, adding -webkit-backface-visibility:hidden to .mover
3. Minified bootstrap-grid.css and style.css
4. Inlined style.css
6. Changed bootstrap-grid.css link reference to bootstrap-grid-min.css

Main.js
1. Use compressed pizza.png images
2. Modified updatePositions function:
	Moved modvalue and phase calculation outside of for loop to eliminate
	unnecessary calculations.
	Replaced querySelectorAll with getElementsbyClassName
	Utilized transform translateX for scrolling pizza position updates
3. Modified the sliding pizza when page load function to reduce unnecessary
	for looping. Reduced the condition to < 22.
4. Modified changePizzaSizes function:
	Moved dx and width calculation outside of for loop to avoid unnecessary
	processing with each iteration.
	Replaced querySelectorAll with 
	Cache randompizza array length outside of for loop
	Select the randomPizzaContainer element once for pizza resizing outside of function

Tools & References:

http://optimizilla.com/
https://compressor.io/

http://cssminifier.com/
http://jscompress.com/

http://jshint.com/

https://wordpress.org/support/topic/eliminate-external-render-blocking-javascript-and-css-in-above-the-fold-content?replies=23

https://developers.google.com/speed/docs/insights/OptimizeCSSDelivery

http://matthewjamestaylor.com/blog/adding-css-to-html-with-link-embed-inline-and-import

stackoverflow.com

https://developer.mozilla.org/en-US/docs/Web/CSS/backface-visibility

http://www.w3schools.com/cssref/css3_pr_transform.asp

https://plus.google.com/events/c8eah6f0d0t9eretebpm7dqi0ok?authkey=CKaNhtb0quvqKA

https://developers.google.com/speed/pagespeed/insights/



