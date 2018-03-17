The purpose of this document is to gather all evidence and materials regarding SVG. How to make them, how to include them in a web page, how to animate them.

There's a lot of ground to cover, so let's get going.

# Making SVG

There are a few pieces of software out there to create and edit SVG files. Sure you can manufacture SVG directly through HTML tags, but for the ease of implementation, these tools are helpful in the learning stages.

I personally use [Inkscape](https://inkscape.org/en/), you may prefer [Illustrator](https://www.adobe.com/products/illustrator.html), [Sketch](https://www.sketchapp.com/) or any other tool. The important trait that all software should share is the following: you can create and edit your own concoction and save it in an SVG format.

Once saved, you can open the SVG file in any text editor. The final result may look a little heavy on text, especially heavy on tags and lines which don't seem to serve a purpose. You can either remove them manually or use a tool to optimize your creation (optimization tools are discussed in a later section).

Looking at the code behind the SVG is nevertheless useful to get acquainted with its syntax and the role of the different attributes.

# Displaying SVG

To include SVG files in your document there are multiple, available routes. Each has some advantages on their side, and I'll spend a line or two on each option, right after the list of all possibilities.

- `<img>` HTML element.

  You can reference an SVG file directly in the `src` attribute of an image element.

  ```HTML
  <img src="svg-doc.svg"/>
  ```

- `background` CSS property.

  In CSS, the SVG file can be referenced to be the background of an HTML element.
  
  ```CSS
  .container {
    background: url("svg-doc.svg");
  }
  ```
  
- `<svg>` HTML element.

  It is possible to directly inject the SVG file in the HTML document. Simply open the SVG in a text editor, copy-paste the syntax you find in between body tags.

  ```HTML
  <body>
    <?xml version="1.0" encoding="UTF-8" standalone="no"?>
    <!-- Created with Inkscape (http://www.inkscape.org/) -->

    <svg
       xmlns:dc="http://purl.org/dc/elements/1.1/"
       xmlns:cc="http://creativecommons.org/ns#"
       xmlns:rdf="http://www.w3.org/1999/02/22-rdf-syntax-ns#"
       xmlns:svg="http://www.w3.org/2000/svg"
       xmlns="http://www.w3.org/2000/svg"
       xmlns:sodipodi="http://sodipodi.sourceforge.net/DTD/sodipodi-0.dtd"
       xmlns:inkscape="http://www.inkscape.org/namespaces/inkscape"
       width="117.64108mm"
       height="54.816246mm"
       viewBox="0 0 117.64108 54.816246"
       version="1.1"
       id="svg8"
       inkscape:version="0.92.2 (5c3e80d, 2017-08-06)"
       sodipodi:docname="svg-doc.svg">
      <defs
         id="defs2" />
      <sodipodi:namedview
         id="base"
         pagecolor="#ffffff"
         bordercolor="#666666"
         borderopacity="1.0"
         inkscape:pageopacity="0.0"
         inkscape:pageshadow="2"
         inkscape:zoom="0.7"
         inkscape:cx="112.64435"
         inkscape:cy="16.156943"
         inkscape:document-units="mm"
         inkscape:current-layer="layer1"
         showgrid="false"
         fit-margin-top="0"
         fit-margin-left="0"
         fit-margin-right="0"
         fit-margin-bottom="0"
         inkscape:window-width="1366"
         inkscape:window-height="705"
         inkscape:window-x="-8"
         inkscape:window-y="-8"
         inkscape:window-maximized="1" />
      <metadata
         id="metadata5">
        <rdf:RDF>
          <cc:Work
             rdf:about="">
            <dc:format>image/svg+xml</dc:format>
            <dc:type
               rdf:resource="http://purl.org/dc/dcmitype/StillImage" />
            <dc:title></dc:title>
          </cc:Work>
        </rdf:RDF>
      </metadata>
      <g
         inkscape:label="Layer 1"
         inkscape:groupmode="layer"
         id="layer1"
         transform="translate(-52.645022,-127.23546)">
        <g
           id="g843">
          <path
             sodipodi:nodetypes="sssscs"
             inkscape:connector-curvature="0"
             id="rect10"
             d="m 137.65475,137.49405 c 4.986,0 9,4.014 9,9 v 18.28571 c 0,4.986 -4.12432,10.04303 -9,9 L 52.845234,155.63691 c -4.986,0 84.809516,-18.14286 84.809516,-18.14286 z"
             style="fill:#ff8021;fill-opacity:1;stroke-width:0.26458332" />
          <g
             style="stroke:none;stroke-opacity:1"
             id="g834">
            <rect
               style="fill:#46dd46;fill-opacity:1;stroke:none;stroke-width:0.26511249;stroke-miterlimit:4;stroke-dasharray:none;stroke-opacity:1"
               id="rect819"
               width="28.726189"
               height="8.6934528"
               x="-130.27333"
               y="160.33"
               ry="4.3467264"
               transform="rotate(-80.514908)" />
            <rect
               transform="rotate(-50.514908)"
               ry="4.3467264"
               y="203.98653"
               x="-32.655014"
               height="8.6934528"
               width="28.726189"
               id="rect821"
               style="fill:#46dd46;fill-opacity:1;stroke:none;stroke-width:0.26458332;stroke-opacity:1" />
            <rect
               style="fill:#46dd46;fill-opacity:1;stroke:none;stroke-width:0.26458332;stroke-opacity:1"
               id="rect823"
               width="28.726189"
               height="8.6934528"
               x="205.74078"
               y="9.9500694"
               ry="4.3467264"
               transform="rotate(43.402266)" />
            <rect
               transform="rotate(77.077198)"
               ry="4.3467264"
               y="-107.2576"
               x="181.55429"
               height="8.6934528"
               width="28.726189"
               id="rect825"
               style="fill:#46dd46;fill-opacity:1;stroke:none;stroke-width:0.26458332;stroke-opacity:1" />
            <rect
               transform="rotate(9.727334)"
               ry="4.3467264"
               y="122.35964"
               x="165.69971"
               height="8.6934528"
               width="28.726189"
               id="rect827"
               style="fill:#46dd46;fill-opacity:1;stroke:none;stroke-width:0.26458332;stroke-opacity:1" />
          </g>
        </g>
      </g>
    </svg>
  </body>
  ```

### Considerations

**Background**: the HTML elment needs to have a width and height in order to display the SVG. You need to here be careful with the size of the container and the measures of the SVG, which are specified in the SVG file under the attributes of width and height. You may end up with an SVG that is either cropped or repeated, if the element is too small, too big in comparison to the SVG.
 
**SVG Inline**: as mentioned, the SVG files are often text intensive. This is where optimization tools come into play. After the SVG tags are "cleaned up" of unnecessary elements, the SVG elements are drastically improved. 


Out of the mentioned opportunities the `<img>` approach is the easiest to implement. Epecially with a local project, it is possible to reference the SVG by path. It is then possible to style the image element in CSS like any HTML element. This with the added benefit of having a sharp-looking asset.

The `background` option is useful to lay the SVG asset beneath the content of the HTML element.

The `inline` route allows to have direct control on the SVG as a whole as well as its components. Moreover, the HTML document *does not* go through an additional HTTP request. The file is inside the document and there is no need to "fetch" it.

Personally, unless the SVG is included purely for aesthetics, I opt to include SVG assets inline. Otherwise, the `<img>` element is a quick and easy way to include SVG graphics.

As it will be explained later, it is possible to gather multiple SVG inline files together in an SVG system, declaring all files in one place and using them later as needed. This route allows to maintain read-able HTML while preserving the possibilities of inline SVG.

Finally, there are other HTML elements which allow to include SVG files in the web page (object, iframe, embed), but I find the mentioned alternatives to be much easier to understand, implement and manage.

