-------------------Mobile Portfilio Read Me -----------------

This web page is hosted at the following address https://j8298c.github.io/optimization
to run simply click on the link, or copy and paste in your browser of choice. There are several links on the home page just click and go.

In Cam's Pizzeria there are several options to choose from theres a slider which you use to
pick out what size pie you want Small Medium or Large.

I have made several optimizations to both the homepage and and the pizza webpage
Index.html
____________

1. Compressed all Images to bring down overall size of index.html
2. minified and inlined style.css to index.html to prevent it from render blocking
3. moved all JavaScript to bottom of index.html to also prevent it from render blocking the page
4. Added async to all Script tags to load JS asynchronously
5. Moved google fonts.css to bottom as well to prevent it from render blocking the page.
6. Added media="print" attribute to print.css to it is only loaded by browser when user needs to      prints.

Pizza.html
___________

1. Line 447 function changePizzaSizes pulled var dx and newwidth out of for loop as the numbers stay the same there was no need to keep recalculating them while the loop ran.
2. line 505 changed number of pizzas from 200 to 35 since 200 was far too many pizzas to create for the page.
3. line 527 function updatePositions added var scroll as placeholder for scrollTop/1250 calculation
4. line 532 created phase array and used for loop on 534 to push values into phase[]
5. line 533 pulled var items out of loop n 537 so that it wouldnt be called every time user scrolled and triggered for loop.
