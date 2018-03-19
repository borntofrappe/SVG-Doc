All about **S**harp **V**ector **G**raphics: making, including in a web page, animating SVG. 

# Index

- [x] [Making SVG](#making-svg)

- [ ] SVG in the web page(#svg-in-the-web-page)
  - [x] [Displaying SVG](#displaying-svg)
  - [x] [Data URI](#data-uri)
  - [x] [SVG System Set](#svg-system-set)
  - [x] [SVG Optimization](#svg-optimization)
  - [ ] SVG Accessibility
  
- [ ] SVG Animation
  - [ ] CSS Animation
  - [ ] SMIL Animation
  - [ ] JS and Libraries


# Making SVG

There is more than one software out there to create and edit SVG files. Theoretically you can manufacture SVG directly through HTML tags, but for the ease of implementation, these tools are helpful in the learning stages. (more on this later)

I personally use [Inkscape](https://inkscape.org/en/), you may prefer [Illustrator](https://www.adobe.com/products/illustrator.html), [Sketch](https://www.sketchapp.com/) or any other tool. The important trait that all software should share is the following: *you can create and edit your own concoction and save it in an SVG format*.

Once saved, you can open the SVG file in any text editor. The final result may look a little heavy on text, especially heavy on tags and lines which don't seem to serve a purpose. 

You can either remove them manually or use a tool to optimize your creation (optimization tools are discussed in a later section).
Looking at the code behind the SVG is nevertheless useful to get acquainted with its syntax and the role of the different attributes.


# SVG in the web page

## Displaying SVG 

To include SVG files in your document there are multiple, available routes. Each has some advantages on their side, and I'll spend a line or two on each option, right after the list of possibilities.

- `<img>` HTML element.

  An SVG file can be directly referenced in the `src` attribute of an image element.

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

  Back in HTML, it is possible to directly inject the SVG file in the document. Simply open the SVG in a text editor, copy-paste the syntax you find in between body tags.

  ```HTML
  <body>

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

**Background**: the HTML elment needs to have a specified `width` and `height` in order to correctly display the SVG. You need to here be careful with the size of the container and the measures of the SVG, which are specified in the SVG file under the attributes of `width` and `height`. You may end up with an SVG that is either cropped or repeated, if the HTML element is too small or too big in comparison to the SVG.
 
**SVG Inline**: as mentioned, the SVG files are often text intensive. This is where an SVG set and optimization tools come into play. After the SVG structure is "cleaned up" of unnecessary elements and presented in a concise set, inline SVG elements are drastically improved. 

Out of the mentioned opportunities:

- the `<img>` approach is the easiest to implement. Epecially with a local project, it is possible to reference the SVG by path. It is then possible to style the image element in CSS like any HTML element. This with the added benefit of having a sharp-looking graphic.

- the `background` option is useful to lay the SVG asset beneath the content of the HTML element.

- the `inline` route allows to have direct control on the SVG as a whole as well as its components. Moreover, the HTML document *does not* go through an additional HTTP request. The file is inside the document and there is no need to "fetch" it.

Personally, unless the SVG is included purely for aesthetics, I opt to include SVG assets inline. Otherwise, the `<img>` element is a quick and easy way to include SVG graphics.

As it will be explained later, it is possible to gather multiple SVG inline files together in an SVG system, declaring all files in one place and using them later as needed. This practice, along with other optimization options, allows to maintain read-able HTML while preserving the possibilities of inline SVG.

Finally, there are other HTML elements which allow to include SVG files in the web page (`object`, `iframe`, `embed`), but I find the mentioned alternatives to be much easier to understand, implement and manage.

## Data URI

The `<img>` and `background` approaches accept a reference to the SVG file. That being said, both alternatives can also include an encoded string which directly references the syntax of the asset, much alike with SVG included inline.

All that is required is to include the following string before injecting the SVG syntax, in a single line argument.

```HTML
data:image/svg+xml;utf8,
```

This syntax is nested in the `src` attribute of an image element or in the URL of a `background` property.

```HTML
<img src='data:image/svg+xml;utf8,<svg>...</svg>'/>
```

```CSS
.container {
  background: url('data:image/svg+xml;utf8,<svg>...</svg>');
}
```

Allowing the inclusion of the SVG asset without HTTP request or direct reference to a local path. 

**Potential Issues**: the call to the SVG needs to be included in a single line, without carriage returns. Moreover, the SVG syntax uses quotes for the different attributes it accepts. As the `src` attribute, or the `background` property, makes use of quotes itself, you can either escape all SVG quotes or use single quotes for one and double quotes for the other.

```HTML
<img src='data:image/svg+xml;utf8,<svg width="500px">...</svg>'/>
```

## SVG System Set

Including SVG inline allows to directly interact with the SVG, its components and all their respective properties. That being said, including each SVG file with all the connected syntax may result an HTML structure which is difficult to ready and hardly sustainable.

What can be done with this regard is split the SVG declaration from its use. Simply put:

- declare all SVG files in a common block, with all connected attributes and often verbose syntax;

- use each file as needed, with a simplified tags.

The split is allowed thanks to the tags of `<defs>` and `<use>`, as will be shortly explained.

**Define SVG Set**

At the top of the `<body>` element, it is possible to build an SVG set by placing `<defs>` tags inside of a wrapping `<svg>` element. 
  
To avoid the browser from pre-emptively occupying space, a property of `display:none;` is specified for this wrapping element. Without it, the browser will allocate space reuired by the SVG(s), without actually displaying the SVG assets, resulting in unnecessary white space. 
  
```HTML
<body>

<svg style="display:none;">
  <defs>
  
  </defs>
</svg>

</body>
```

Inside the defining tags, any and all SVG assets are then included with their syntax. Include here `<g>`, `<path>` elements which describe the different graphics.

Each graphic should contain the following attributes:

- id;

- viewbox.

The former is required to later reference each graphic when needed, while the latter is a defining attribute which describes the space occupied by the SVG (literally, the viewbox in which the SVG graphic is crafted). It is therefore possible to gather multiple SVG assets with different structures, in terms of viewbox as well. 

With a couple of examplary SVG files, the defs block looks as follows:

```HTML
<svg style="display:none;">
  <defs>

   <g id="timer-icon" viewBox="0 0 26.458 26.458" transform="translate(-31.082 -144.97)">
    <rect transform="matrix(.73691 -.67599 .65904 .75211 0 0)" x="-72.427" y="131.57" width="3.6309" height="2.1467" fill="#fff" stroke-width=".39495"/>
    <path transform="matrix(.26458 0 0 .26458 31.082 144.97)" d="m50 0a50 50 0 0 0-50 50 50 50 0 0 0 50 50 50 50 0 0 0 50-50 50 50 0 0 0-50-50zm0 9.7012a40.299 40.299 0 0 1 40.299 40.299 40.299 40.299 0 0 1-40.299 40.299 40.299 40.299 0 0 1-40.299-40.299 40.299 40.299 0 0 1 40.299-40.299z" fill="#fff" stroke-width="1.97"/>
    <circle transform="rotate(141.82)" cx="62.947" cy="-151.75" r="10.514" fill="none" stroke="#fff" stroke-dasharray="1.8678617, 3.73572337" stroke-width=".46697"/>
    <path d="m44.214 148.57 0.88034 9.6044-1.5663 0.0197z" fill="#fff" stroke-width=".28933"/>
    <circle transform="rotate(141.82)" cx="62.947" cy="-151.75" r="10.063" fill="none" stroke="#fff" stroke-dasharray="1.78778218, 3.57556438" stroke-width=".44695"/>
   </g>


  <g id="heart-icon" viewBox="0 0 5.2917 5.2917" transform="translate(-68.595 -111.29)">
   <g transform="matrix(2.8714 0 0 3.0436 -128.37 -238.24)">
    <path transform="matrix(.092144 0 0 .086931 68.595 114.84)" d="m14.037-0.013672 0.001953 0.0019531c-1.5769 0.057517-3.1759 0.76063-4.4277 2.0879-0.024961 0.023007-0.047305 0.057071-0.072266 0.080078l-0.0039063-0.0019531-0.074219 0.080078c-2.4637-1.8384-5.7468-1.7084-7.8086 0.47656v0.0019531c-2.3294 2.469-2.1911 6.5923 0.3125 9.2461 0.024961 0.023007 0.055117 0.047522 0.080078 0.082032l-0.0039063 0.001953 7.4902 7.9395 0.91992-0.97461 0.001953 0.00586 7.4902-7.9414-0.001953-0.001954c0.026046-0.023006 0.053164-0.045568 0.078125-0.080078 2.5037-2.6538 2.6438-6.779 0.31445-9.248-1.1647-1.2344-2.7199-1.8161-4.2969-1.7559zm-2.2246 5.5195c0.71225-0.027608 1.4154 0.2331 1.9414 0.79102 1.0522 1.1153 0.98826 2.979-0.14258 4.1777-0.010551 0.011184-0.021541 0.023973-0.033203 0.035157l-3.3828 3.5879-0.001953-0.001953-0.41602 0.43945-3.3828-3.5859c-0.010722-0.011184-0.022652-0.023973-0.033203-0.035157-1.1309-1.1988-1.1947-3.0619-0.14258-4.1777 0.93136-0.98699 2.4145-1.0454 3.5273-0.21484l0.033203-0.035156 0.0019531 0.0019531c0.011938-0.011503 0.020398-0.023653 0.03125-0.035156 0.56542-0.59933 1.2877-0.90885 2-0.94336v-0.0039062z" fill="#f55" stroke-width=".47444"/>
   </g>
  </g>

 </defs>
</svg>
```

The code may be verbose, but is indeed separate from the HTML structure of the page which follows. Structure which is more easily manipulated through the `<use>` tags.


**Use SVG Assets**

Once declared and given an identifier, each SVG graphic can be easily injected in the page. All that is required is to nest `<use>` tags in a wrapping SVG element.

The SVG element ought to have an attribute of `viewbox` matching in value with the attribute specified in the defs block. The `<use>` tags instead benefit from the `href` attribute, which is used to target the identified SVG.

**Small note**: in the old implementation for the `<use>` tags, the attribute referencing the SVG asset was `xlink:href`. With the new Web Standard, the attribute was simplified to a more common name, `href`.

Using an SVG from the examplary `defs` block, for instance, the implementation of the SVG looks as follows:

```HTML
<svg class="heart-icon" viewBox="0 0 5.2917 5.2917">
  <use href="#heart-icon"></use>
</svg>
```

Which is a definite improvement in terms of read-ability.

The SVG set is therefore really useful, both in terms of separating logical steps (declare first, use later), and in terms of providing concise, more sustainable code.

## SVG Optimization

As mentioned, SVG syntax is often bloated with unnecessary attributes and, especially for more complex concoctions, expands itself in an almost outrageous amount of code lines.

The inclusion of an SVG set helps improving the read-ability of the code, but the "defs" block defining each asset is still heavy on and difficult-to-comprehend text; with multiple graphics, the risk of a minor error messing up the whole system becomes quite high.

Optimization practices allow to reduce this risk by streamlining the structure of the SVG syntax. It is here possible to remove attributes included by the SVG editor which serve no purpose in the HTML document. Above all, it is possible to present the SVG syntax in a more compact format.

**Inkscape save as**

Inkscape has a built-in functionality which allows to save a concise SVG file. Instead of simply saving the file as-is, the dropdown menu next to `Save as type` offers in fact the option to save as `Optimized SVG`. 

With this selection, the output can be customized as to shorten the length of the SVG, for instance by reducing the precision used for the coordinates of the graphic.

In the "SVG Output" tab it is also possible to remove XML declaration, metadata and comments, removing the default and unnecessary tags.

It is a more manual approach than the following possibility, but one method which allows to better understand how the editor works and which SVG tags are essential for the correct rendering in a web page.

**SVGO**

*Small note*: for the command-line program, Node.js is required to run the detailed prompt.

[SVGO](https://github.com/svg/svgo) allows to change SVG files in an extremely concise format, and in a more automatic approach than the previous alternative.

It also allows to reduce an entire SVG file to a single line. This option may be a little cumbersome when trying to visualize how an SVG file is built, but it is accomplished to further reduce the file size. The improvements in this dimension are remarked (often surpassing the 50% mark of size reduction).

Once installed through the command line:

```
npm install -g svgo
```

SVGO optimizes SVG files through one of following commands:

|Command|Effect|
|---|---|
|`$ svgo file.svg`|Optimize the referenced file, changing the input to the concise format|
|`$ svgo file.svg another-file.svg`|Optimize the referenced files, changing both inputs to the respective concise format|
|`$ svgo file.svg -o file-output.svg`|Save the concise format in a new file, without altering the input|
|`$ svgo *.svg`|Optimize all SVG files referenced file, changing the inputs to the respective concise format|

It is also possible to target multiple SVG files, simply by space separating their name. 

It is always paramount to 1) include the file extension and 2) reference the right path to the file (practically running the prompt in the folder in which the file reside is helpful).

A small example will remark the sensible improvements hereby presented.

- saving a simple icon without optimization produces the following result:


```HTML
<?xml version="1.0" encoding="UTF-8" standalone="no"?>
<svg
   xmlns:dc="http://purl.org/dc/elements/1.1/"
   xmlns:cc="http://creativecommons.org/ns#"
   xmlns:rdf="http://www.w3.org/1999/02/22-rdf-syntax-ns#"
   xmlns:svg="http://www.w3.org/2000/svg"
   xmlns="http://www.w3.org/2000/svg"
   xmlns:sodipodi="http://sodipodi.sourceforge.net/DTD/sodipodi-0.dtd"
   xmlns:inkscape="http://www.inkscape.org/namespaces/inkscape"
   width="100"
   height="100"
   viewBox="0 0 26.458 26.458"
   version="1.1"
   id="svg8"
   sodipodi:docname="star-icon.svg"
   inkscape:version="0.92.2 (5c3e80d, 2017-08-06)">
  <metadata
     id="metadata14">
    <rdf:RDF>
      <cc:Work
         rdf:about="">
        <dc:format>image/svg+xml</dc:format>
        <dc:type
           rdf:resource="http://purl.org/dc/dcmitype/StillImage" />
      </cc:Work>
    </rdf:RDF>
  </metadata>
  <defs
     id="defs12" />
  <sodipodi:namedview
     pagecolor="#ffffff"
     bordercolor="#666666"
     borderopacity="1"
     objecttolerance="10"
     gridtolerance="10"
     guidetolerance="10"
     inkscape:pageopacity="0"
     inkscape:pageshadow="2"
     inkscape:window-width="640"
     inkscape:window-height="480"
     id="namedview10"
     showgrid="false"
     inkscape:zoom="2.36"
     inkscape:cx="50"
     inkscape:cy="50"
     inkscape:window-x="0"
     inkscape:window-y="0"
     inkscape:window-maximized="0"
     inkscape:current-layer="svg8" />
  <g
     transform="translate(0,-270.542)"
     id="g6">
    <rect
       rx="1.306"
       ry="1.944"
       y="270.54199"
       height="26.458"
       width="26.458"
       id="rect2"
       x="0"
       style="fill:#69cfde" />
    <path
       d="m 4.46,281.75 h 6.71 l 2.066,-6.606 2.052,6.595 6.71,-0.031 -5.441,4.077 2.08,6.586 -5.415,-4.075 -5.423,4.102 2.094,-6.596 z"
       id="path4"
       inkscape:connector-curvature="0"
       style="fill:#ffffff" />
  </g>
</svg>
```

- selecting the option of saving the file as Optimized SVG, as mentioned, produces the following result:

```HTML
<svg width="100" height="100" version="1.1" viewBox="0 0 26.458 26.458" xmlns="http://www.w3.org/2000/svg">
 <g transform="translate(0 -270.54)">
  <rect y="270.54" width="26.458" height="26.458" rx="1.306" ry="1.944" fill="#69cfde"/>
  <path d="m4.46 281.75h6.71l2.066-6.606 2.052 6.595 6.71-0.031-5.441 4.077 2.08 6.586-5.415-4.075-5.423 4.102 2.094-6.596z" fill="#fff"/>
 </g>
</svg>
```

- running a command-line prompt with svgo, `$ svgo icon.svg` , the un-optimized file is altered to the following format:


```HTML
<svg xmlns="http://www.w3.org/2000/svg" width="100" height="100" viewBox="0 0 26.458 26.458"><g transform="translate(0 -270.542)"><rect rx="1.306" ry="1.944" y="270.542" height="26.458" width="26.458" fill="#69cfde"/><path d="M4.46 281.75h6.71l2.066-6.606 2.052 6.595 6.71-.031-5.441 4.077 2.08 6.586-5.415-4.075-5.423 4.102 2.094-6.596z" fill="#fff"/></g></svg>
```

Reducing the file size by a whopping 81%.

With the inclusion of one of this methods, alongside the construction of an SVG set, SVG inline become a much more manageable, sustainable alternative. This with the added benefit of having direct control on the SVG files and their components.

## SVG Accessibility


