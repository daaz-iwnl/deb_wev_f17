FINAL DOCUMENTATION

LIVE SITE: https://daaz-iwnl.github.io/index.html ****D3.v3.min.js is not HTTPS enabled--ENABLE UNSAFE SCRIPTS****

======== PT 1: HOMEPAGE ========

The new site is a rebuild of the midterm portfolio site, though instead of using Bootstrap, it is a creative-JS redesign. Because a large part of my work is drawings/illustrations, I wanted a site that would reflect that. This site is meant to be weird, unique, inner-machinations-of-the-mind kind of site unlike other sites. The theme is "hand drawn" images and whimsy. 

In comparison to the midterm, the new homepage has gone through the most drastic changes, as it is almost completely JS-based. It is functional but not without issues. The bulk of the HOMEPAGE calls upon the D3.js data visualization library, and especially the use of D3.force and D3.nodes.

The nodes contain data from an external JSON file that includes images of drawings I made and their respective native dimensions. These nodes--with drawings of "feathers, ribs, spines, leaves, whatever"--repel from the mouse due to the D3.force and otherwise float around the canvas. Clicking anywhere on the page moves to the PORTFOLIO page.

======== PT 2: PORTFOLIO ========

Aside from eliminating the ABOUT page and incorporating it into the HOMEPAGE, the PORTFOLIO page actually remains similar. It simply has undergone a visual redesign with the appropriate color scheme of the new site--black, white, and #e91919 version of red. However, the portfolio page has a fixed button that downloads the resume. Because this page incorporates the same elements as some of the things on the resume, it has been moved to the portfolio page as a text alternative to a webpage.

======== PT 3: ISSUES/LEARNING EXPERIENCES ========

One of the biggest issues was being unable to reference the image files for dimensions, and the JSON was thus a workaround where the information was manually put in.

Another nuisance was the way in which the D3.force interacted with the nodes in conjunction with RECTANGULAR COLLISION. When on the site, the images usually--but not always--repel from the mouse, and sometimes to varying degrees. In testing dozens of combinations of "gravity" and "charge" (attributes of D3.force), it was difficult to find an aesthetically appealing, fluid looking behavior. The goal was to ensure that no feathers ever touch, and they never touch the mouse--however, it is still unsolved.

Often, the issues that were encountered were some combination of svg elements (nodes, rectangles, circles) being unable to support images or the force behaving incorrectly with the rectangular collision. Also because of the large amount of processing and loading that must happen on this page, I discovered quadtrees could be used to speed up the process.

Looking back, it may have been easier to program images with GSAP/JS animations instead of using D3 Force, but for what I would want the site to be later on seems only possible with D3 or other external libraries. However, attempting to learn D3 from the available examples and documentation was exceptionally stressful.

A minor issue is that the CSS styles for the PORTFOLIO page are completely messed up when run anywhere but on github pages and I have not been able to figure out why, so the site will stay at daaz-iwnl.github.io.

======== PT 4: NEXT STEPS ========

From this, I've experimented and learned a lot about the D3.js library, SVG drawings through JS, and using JSONs. If I had more time and resources, I would want to smooth out the movement of the D3 nodes, and find a better way to organize the images into elements while having good collision behavior. Furthermore, I would want to incorporate the portfolio page INTO the nodes or into the feathers in some way to make it weirder and more unique.
 
