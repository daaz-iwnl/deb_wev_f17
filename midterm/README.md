MIDTERM DOCUMENTATION

** TEMP LINK TO SITE: https://daaz-iwnl.github.io/index.html **

BLOG POST: http://sites.bxmc.poly.edu/~danielli/iwd/index.php/2017/10/30/midterm-intro-web-dev/

======== PT 1: HOMEPAGE ========

Functionally, I wanted the homepage to be essentially an interactive splash page and focus on capturing the attention than being functional. In settling on a theme, I went with something simple, and I chose the nostalgia look through the type and images. Since the site only has two other pages, I linked them to different parts of the splash page. The homepage only has a title/subtitle, and a graphic--which hopefully will invite people to click somewhere on the graphic. The photographs link to the portfolio, and the handwriting leads the user to an "about me" page. Initially, I was going to make a navbar that would show and hide--however, the homepage started to feel like just a glorified table of contents. All pages use 996 grid, and scale to device.

======== PT 2: PORTFOLIO ========

The portfolio page is the most advanced of the three. Aesthetically, it is still a simple page with a title header, and different projects are separated based on category--animation, graphic design, photography, video--each contained in a different row. Each thumbnail is 300x300, and upon hover, displays the project name and description over a red to blue-green gradient--the image underneath turns greyscale so the gradient is clean. In keeping with the nostalgia theme, the color palette is pulled from the splash page image. Clicking on each thumbnail would open a modal window that provides more details on each project and a gallery of images of the project. The title links back to the splash page. One issue was nesting grid_4 elements into one grid_12 element, which ended up messing with the media queries.

======== PT 3: ABOUT ========

The about page is relatively simple at the moment, since it only contains text and a mailto and download link. I wanted to keep the lines horizontally constrained to make reading easier, and also ensure that it was responsive. At first, I made the containing elements fluid in size, but then later realized that using the grid_8 from 996 would be much easier.

======== PT 4: Thumbnail/Modals Source Code ========

In this section of the portfolio page contains the code for the thumbnails and test modal. The cluster class simply clears the margins on the category header, and the h2 sits on a different row from the thumbnails. Each thumbnail occupies a grid_4 size column, with a max-width of 300px--the width that each of the images are set to. mask is a class that contains several hover properties and transitions including the gradient and text that pop up when hovering.

The modal window here only works with the animated youtube video as of now, since it is hard-coded for that exact project. It has a close button that eventually ideally will work with keypresses such as escape later on. #mediaWindow is the left-hand, black div where #mediaObj is contained. the media objects that would appear in the modal window would either scale fully width or lengthwise 100%, if not both. Meanwhile, #mediaDesc provides descriptions/details of the project.



======== PT 5: Issues and Onwards ========

In trying to make a modal that changes content depending on the project, I realized that I'd either have to hard code all the modals each time or use javascript to pull data. Instead of hard coding all of the modals individually, I decided one of the things that I would try to learn next would be doing it through javascript. I would also like to make the homepage more eye-catching and intuitive, either with some hover effects like pencil drawn outlines around the text or photos or hand drawn arrows that point to each part of the image that indicate to the user that this is something they can click on. Otherwise, I'd then work on making the backgrounds or regions outside the 996 some graphics to make it feel more complete. Mostly, I've become familiar with 996, and trying to make the pages work on all screens properly--and how to make interesting interactive effects like hover.