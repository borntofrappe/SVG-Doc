The purpose of this document is to gather all evidence and materials regarding SVG. How to make them, how to include them in a web page, how to animate them.

There's a lot of ground to cover, so let's get going.

# Making SVG

There are a few pieces of software out there to create and edit SVG files. Sure you can manufacture SVG directly through HTML tags, but for the ease of implementation, these tools are helpful in the learning stages.

I personally use [Inkscape](https://inkscape.org/en/), you may prefer [Illustrator](https://www.adobe.com/products/illustrator.html), [Sketch](https://www.sketchapp.com/) or any other tool. The important trait that all software should share is the following: you can create and edit your own concoction and save it in an SVG format.

Once saved, you can open the SVG file in any text editor. The final result may look a little heavy on text, especially heavy on tags and lines which don't seem to serve a purpose. You can either remove them manually or use a tool to optimize your creation (optimization tools are discussed in a later section).

Looking at the code behind the SVG is nevertheless useful to get acquainted with its syntax and the role of the different attributes.

# SVG on a web page

To include SVG files in your document there are multiple available routes. Some have more advantages over the other, and I'll spend a line or two on the options I found most advantageous, right after the list of all possibilities.
