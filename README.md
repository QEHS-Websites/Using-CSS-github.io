# CSS Notes and Lessons
Inline, Styles in HTML, .CSS File

**UNDER CONSTRUCTION**

---

Helping Hyperlinks
- Intermediate Boilerplate, <a href="https://github.com/MercersKitchen/Webpages-Sites/tree/master/Boilerplate%20Intermediate">Click Here</a>

---

Progression of Learning
- Summary for CSS - Looking at Vocabularies
- Three Ways of Writing CSS (Best Practice of Loading a Page, see Intermediate Boilerplate folder for illustration)
- Lesson: progression from inline to ID (in <style></style>) to ID in .css
- CSS DOC, beginning a .css DOC: main.css
- Creating a Legend
- Note: Combining HTML Elements with CSS Class: element.class syntax
- Example using Classes and Tags
- Example using DIVs and CLASSES
- Using CSS with Images
- Interaction of HTML DIVs and CSS IDs and classes
- Position of Elements in CSS
- Layout in CSS: Box Method
- Summary about colour, foreground & background
- Optional: Using Tables in CSS
- Common Inline Style Properties (See W3 Schools)

---

More Teacher Notes, <a href="https://github.com/QEHS-Websites/CSS-Sandbox">Click Here</a>

When to Include CSS
- Focus on Website Map: navigation works to Child Pages, .js & .css (with debugging lines)
- Focus on Content to Include, according to Case Study: images, videos, audio, text
- Focus on HTML Layout and Incorporating Text with HTML Tags to format and hyperlink text
- Focus on Functionality of Webpage Behaviors
  - For example: what information can be collected from a user and when
- Focus on CSS look and feel of HTML Layout and other HTML tags
  - Choose what is more appropriate: inline, style tag, .css file

---

# Summary for CSS - Looking at Vocabularies

1. A CSS selector targets an HTML element.
2. CSS declarations style HTML elements. Declarations must contain the following two things:
   - property: the property you want to style.
   - value: the value for the property you are styling.
3. CSS declarations must end in a semicolon (;)
4. A CSS rule consists of a CSS selector and the declarations inside of the selector.
5. Multiple element selectors can be used to style multiple elements at once.
6. Comments keep code easy to read and allow you to experiment with new code without having to remove old code.
7. CSS follows certain best practices for spacing and indentation:
   - One line of spacing between a selector and the opening curly brace.
   - No spacing between CSS declarations and the opening and closing curly braces of the CSS rule.
   - Two spaces of indentation for CSS declarations.
   - One line of spacing between CSS rules.

---

# Ideas to Include
Rewrite CSS Examples
- Simple Textfield linked to JavaScript to output the next number when adding 12

Rewrite table examples to be like HELLO WORLD Exemplars (inline, style-tag, classes)

See Text Documents and Incorporate Here with Code Boxes to illustrate

End of the Year HTML5
- Embedding Processing-Java in Webpage using CSS to promote Processing-Java Programming
- Notes about what is emphasized

---

CSS Lessons in JS Fiddle
- HTML Tags with CSS File over written with inline style
  - color with hexadecimal
  - fonts from Google Fonts


  - create more examples using CSS

Exemplars of CSS
- What does CSS Overwritting look like (website legend, page exceptions, inline exceptions).

---

Three Ways of Writing CSS (Best Practice of Loading a Page, see Intermediate Boilerplate folder for illustration)
1. Loading External Document
  - Internal Link
    - Example for Linking HTML to CSS
    - Linking HTML to CSS with absolute and relative paths

    ```HTML
    <link href="/style.css" type="text/css" rel="stylesheet">
    ```
    - href: address or path to the file (vocab for outside or inside computer)
    - type=”text/css”, type of file
    - rel=“stylesheet”, relationship
    - Caution: not sure what "/style.css" does, might be related to Internet CSS Pathway in Example below
  - External Link
    - Example of exterior link:
    ```HTML
    <link href="https://www.codecademy.com/stylesheets/style.css" type="text/css" rel="stylesheet">
    ```
    - Note: this link references a .css file on a separate server, different than a path in a folder

    - Commenting in a file: `/* … */`

2. Part of Head
3. Inline
   - Example
   ```HTML
   <p style="color:blue; font-size:46px;"> I'm a big, blue, <strong>strong</strong> paragraph.</p>
   ```

---

Lesson: progression from inline to ID (in <style></style>) to ID in .css
- ID is an identifier
- No two elements in an HTML file should have the same ID, unique only
  This is different than having the same formatting
  Similar formatting is called classes
- Caution: IDs are easier to read inline or in .html <style></style> than .css
- Example
  .html: <h1 id="botswana">Botswana</h1>
  .css: #botswana { background-color: #56ABFF; }

---

CSS DOC, beginning a .css DOC: main.css
- This requires a "Lengend Layout for the HTML file"
- Vocabulary & Syntax: property:value;
- Universal Selector: every element is selected
  `* { property:value; }`
- Single Selector Example
  h1 { color: rgb(22, 34, 88); }
- Single Selector with Redundancy
  Colour example using OPACITY, not supported on older browsers
  Note: all browsers will run the first line, only supported browsers will be able to run the second
  If a line cannot be run it is skipped
  h1 {
      color: rgb(22, 34, 88);
      color: rgba(22, 34, 88, 0.4);
     }
- Multiple Selectors Example
  h1, h2, p { property:value; }

- Note about using Redunancy or "alternate" code
  Similar to img scr & alt
  Provides control over design when delievering to mutliple browsers

---

Creating a Legend
- Using a Venn or Euler Diagram
  What properties are planned?
  Where are the overlaps
- HTML Elements: all are contained in a box with width and height
  Set using one of three units of measurement: pixels, ems, or percentages
  Minimum or Maximum can be set
  If window or display becomes too small, overflow, and controlled with overflow property
  Other methods exist
  Able to style borders of element's box
    - border-style property allows you to change the style of border used
    - border-width property allows you to set the thickness, or width, of a border
    - border-color property allows you to change the color of a border
    - Short-hand: border: [style, thickness, and color] `/* in that order */`
      Note: eliminates bloat code, or individually setting each property
    - border-radius property allows you to change the square corners to rounded corners
- DIVs: groups similar elements together
  Labeled with classes, not IDs
  <div></div> groups elements in HTML file
- CLASS: common IDs
- Multiple element.class similar to VENN Diagram
  Example:
  All books are Georgia font
  Domestic are one colour font, foreign are another colour font
  Example Code in .html:
  <h1 class="book domestic">The Way of the Deep</h1>
  <h1 class="book foreign">A Night in the Sky</h1>
  Example Code in .css
  .book { font-family: Georgia, serif; }
  .domestic { font-color: #0902CC; }
  .foreign { font-color: #B097DD; }

---

Note: Combining HTML Elements with CSS Class: element.class syntax
- All classes are changed with .breaking
- p.breaking requires it to be a paragraph element
- Example Code: this is how you combine formatting ideas into CSS Code
  .breaking { font-family: Georgia, Times, serif; }
  p.breaking { line-height: 1.3em; }
- Multiple element.class syntax declarations
  Example Code: .first, .last { font-size: 20px; }

---

Example using Classes and Tags
Example Code in .html
<h1 class="science">Scientist Discovers Important Cure</h1>
<h1 class="science">New Study Reveals The Importance of Sleep</h1>
Example Code is .css
.science { font-family: Georgia, Times, serif; color: #A3B4C5; text-transform: uppercase; }

Example using DIVs and CLASSES
Example Code in .html
<div class="container">
<h1 class="title">Alice In Wonderland</h1>
<p> ... </p>
</div>
Example Code in .css
div.container {
background-color: rgb(252, 255, 205);
font-family: Roboto, Helvetica, sans-serif
}
h1.title { color: #0D1A2F; }

---

Using CSS with Images

Image dimensions are set using the width and height properties.
A background image can be added to any element using the background-image property.
A background image's repetition is controlled with the background-repeat property.
The position of a non-repeating image can be controlled using the background-positionproperty.
The background property is a shorthand way of setting an image, repetition, and it's position.
The background-image also supports color gradients.

---

Interaction of HTML DIVs and CSS IDs and classes

Code is a lot more readable when it is organized using IDs, classes, and divs.
IDs label HTML elements that are unique to the web page (an element that appears only once).
Classes label elements that will share the same styling. They make styling more efficient.
The <div> groups elements together.
It makes the HTML file easier to read by organizing the web page into logical sections.
HTML elements can be labeled with multiple classes.
Divs are one of the most commonly used HTML elements.
Understanding how they are used is a critical skill for web developers.

---

Position of Elements in CSS

The position property allows you to specify the position of an element in three different ways.
When set to relative, an element's position is relative to its default position on the page.
When set to absolute, an element's position can be pinned to any part of the web page, but the element will still move out of view when the page is scrolled.
When set to fixed, an element's position can be pinned to any part of the web page. The element will remain in view no matter what.
The z-index of an element specifies how far back or how far forward an element appears on the page.
The float property can move elements as far left or as far right as possible on a web page.
You can clear an element's left or right side (or both) using the clear property.

---

Layout in CSS: Box Method

All HTML elements are contained within a box.
Boxes have two dimensions: a width and a height. These dimensions can be modified with the width and height properties.
Width and height dimensions can be set using one of three units of measurement: pixels, ems, or percentages.
A minimum and maximum width or height can be set for a box.
This helps ensure that content remains legible when a user shrinks or expands their browser window.
If an element's box becomes too small, the content may overflow.
The overflowed content can be controlled with the overflow property.

You can style the borders of an element's box.
The border-width property allows you to set the thickness, or width, of a border.
The border-style property allows you to change the style of border used.
The border-color property allows you to change the color of a border.
Individually setting the style, thickness, and color of a border can bloat code.
It's more efficient to use the shorthand border property and specify all three properties at once, in that order.
Box borders don't have to be square. Their corners can be rounded with the border-radius property.

Padding is the spacing between a box's content and the borders of the box.
Padding can be set equally on all sides of the content, or can be set specifically for certain sides of the content only.
Margin is the spacing directly outside of a box's borders.
Margins can be set equally on all sides of a box, or can be set specifically for certain sides of the box only.
The display changes the default behavior of HTML elements.
The visibility property hides an element, but does not remove the amount of space the element takes up on the page.
If you want to hide that element and remove the empty space, use the display property instead.
This lesson completes our overview of the standard box model.
Understanding the box model is important if you want to understand web page layouts.

Unfortunately, the standard box model has a minor limitation: unreliable box dimensions.

---

Summary about colour, foreground & background

Foreground color refers to the actual color of an element, styled with the color property.
Background color refers to the color behind an element, styled with the background-color property.
There are 147 named colors available.
RGB and hexadecimal colors offer over 16 million color possibilities.
HSL is a new way of defining colors in CSS3.
You can modify the opacity of a color with RGBa or HSLa colors.
Not all browsers support newer CSS features, like opacity or HSL,
so additional declarations should be made to support a wide audience of users.
There are many color picker resources available on the Internet to help you select specific colors,
as well as provide colors in different formats.

---

Optional: Using Tables in CSS

The <table> element creates a table.
The <tr> element adds rows to a table.
To add data to a row, you can use the <td> element.
Table headings clarify the meaning of data. Headings are added with the <th> element.
Table data can span columns using the colspan attribute.,
Table data can span rows using the rowspan attribute.
Tables can be split into three main sections: a head, a body, and a footer.
A table's head is created with the <thead> element.
A table's body is created with the <tbody> element.
A table's footer is created with the <tfoot> element.
All the CSS properties you learned about in this course can be applied to tables and their data.

---

Common Inline Style Properties (See W3 Schools)
- Foreground colour
```
color: rgb(0-255,0-255,0-255) | hexadecimal | named; /* 147 named colors available, over 16 million for RGB or HEX */
color: rgba(0-255, 0-255, 0-255, 0-<1); /* Note: 0 -< 1 means between zero and less than 1, represents a percentage of 100%
```

  Note: redundant color with opacity
  color: rgb(22, 34, 88);
  color: rgba(22, 34, 88, 0.4);

  Note: HSL is a new way of defining colors in CSS3
  color: hsl (?, ?, ?);
  color: hsla (?, ?, ?, ?);
  Not all browsers support newer CSS features, like opacity or HSL,
    so additional declarations should be made to support a wide audience of users.

- background-color
  background-color:
- font
- font-size
  font-size:medium|xx-small|x-small|small|large|x-large|xx-large|smaller|larger|length|initial|inherit;
  font-size: pixels, ems, or percentages
- font-weight (i.e. bold
  font-weight: word: bold, normal | Numbers: 100 (thin); 200, 300, 400 (normal);
               500, 600, 700, 800, 900 (bold) |
  Reminder: font-wieght is able to be set when a font is imported, might need to play with this
- font-style (i.e. italics)
  font-style: normal | italics
- font-family: [main], [alternate], [ (default browser font with) serif | sans serif]
  font-family property changes the typeface of text

Common HTML DOC <style></style> Properties
- background-color
- background-image (url or fileName.extension), for a page or an element
  body { background-image: url("https://www.example.com/leaf.jpg"); }
  Default behavior for images is a repeating the image for the length of the scroll, tiled effect.
  Controlling tiled effect needs background-repeat property
  ShortHand for background-repear property
    body { background-image: url("#"); background-repeat: no-repeat; background-position: right center; }
    Becomes
    body { background: url("#") no-repeat right center; }
    Note: background image, repetition, and position (in that order)
    Syntax: similar to Command line Arguments using white space
    Another example - using advanced image properties, below
    body { background: url("#") no-repeat right center; background-attachment: fixed; }
  Code Explained
  background-repeat: [ repeat | repeat-x | repeat-y | no-repeat ]
    repeat - the default value — the image will repeat horizontally and vertically.
    repeat-x - the background image will be repeated only along the x-axis (horizontally).
    repeat-y - the background image will be repeated only along the y-axis (vertically).
    no-repeat - the background image will not be repeated at all and will appear only once.
  Caution: will need a layer of colour under image if image doesn’t repeat
  Consider colors that add to the contrast of the text there
  background-position: [ paired-word position ];
    Uses a 3 by 3 grid (three rows, three columns), meaning there are 9 total possible positions for the image:
    left top - top left corner of the element's box.
    center top - top center of the element's box.
    right top - top right corner of the element's box.
    left center - left column, center row.
    center center - the center of the element's box.
    right center - right column, center row.
    left bottom - bottom left corner of the element's box.
    center bottom - bottom center of the element's box.
    right bottom - bottom right corner of the element's box.
  Caution: if only one value is used, default 2nd value is CENTER
  Question: what happens with the rule of thirds?
    Answer: this is a background image, not foreground; rule of 3rd’s is for foreground
  When an image is not repeated, no-repeat, then it must be positioned (hopefully with colour)
-

Color Lesson Ideas
- Foreground and Background colour vocabulary
  Color pairings, color families, color wheels
- Answers "Basically what looks good?"
- RGB, Hexidecimal, using google to know the values
- Search "Named Colors", http://www.colors.commutercreative.com/grid/
- Search how colors are organized, see https://color.adobe.com/create/color-wheel/
- Values
  named colors
  RGB or RGBA, an alpha value (256 values, 8 bit-color, 1 byte colour, base 10)
  hexidecimal (6 values in groups of 2 for RGB, written in hexidecimal, 32 bit colour, 3 bytes, base 16 values)
  HSL (Hue - 0-360 chooces from colour wheel, Saturation - amount of grey, Lightness - amount of white)
  or HSLA, also alpha value supported in CSS3
- Example Code
  ```
  color: red
  color: rgb(54,74,101) /* Comment the approximate color */
  color: rgba(22, 34, 88, 0.4) /* Comment the approximate color */
  color: #452F73 /* Comment the approximate color */
  color: hsl (182,20%,50%) /* Comment the approximate color */

  background-color: #1c1c1c;
  background-color: rgba(0, 0, 0, 0.6);
  ```
-  Example Code using redundancy code: if supported, the latter code is written
  h1 {
      color: rgb(22, 34, 88);
      color: rgba(22, 34, 88, 0.4);
     }

- Other Examples to imagine even more examples (with color or background-color)
  border-color: #004E89;
  in an element showing text use color

Font Lesson Ideas
- Example vocabulary for font: “font”, “line”, “word”, “letter”, “text”
- Video for Helvetica and Fonts? (from Ross Sheppard?)
- Default Font on browsers for all elements is Times New Roman
- Only pick 2-3 fonts on a page
- Font must be installed or it must be given
  Example Font: Helvetica, Times New Roman
  Code Redundancy: using fallback notation when font is not installed on a computer
  Fallback fonts are used when a certain font is not installed on a user's computer
  Example Code using fallback fonts (guessing what is installed on a browser)
  h1 { font-family: Garamond, Times, serif; }
  h1 { font-family: Georgia, Garamond, serif; }
  h1 { font-family: Helvetica, Arial, sans-serif; }
- Serif-fonts: Times New Roman, Georgia (easier to read in paragraphs for eye movements, etc.)
  Serif fonts have extra details on the ends of each letter
- Sans-Serif: Arial, Helvetica (easier to read in low resolution screens, modern looking, attention grabbing)
  Sans-Serif fonts do not
- See: https://en.wikipedia.org/wiki/Typography for more information

- Finding Fonts, installing
  Using Google Fonts: https://fonts.google.com/
  Google Fonts provides free fonts that can be used in an HTML file with the <link> element
  Combine the following coding examples
  Example
  Index.html
<head>
<link href=" https://fonts.googleapis.com/css?family=Roboto:100" type="text/css" rel="stylesheet" >
</head>
In the style.css file
h1 { font-family: Roboto, Georgia, serif; }
note: the Roboto: 100 specifies an optional font weight

- Example Font: Helvetica, Times New Roman
  Serif-fonts: Times New Roman, Georgia (easier to read in paragraphs for eye movements, etc.)
  Sans-Serif: Arial, Helvetica (easier to read in low resolution screens, modern looking, attention grabbing)
  See: https://en.wikipedia.org/wiki/Typography for more information

- More Advanced Font Properties
  line-spacing (vertical line spacing)
  word-spacing (horizontal spacing between words)
  letter-spacing (spacing between letters)
  text-transform (text can appear in all upper or all lower case for emphasis and changed easily,
                  but originally written normally so web-developer can read it,
                  or, typed once but represented differently on different pages)
  text-transform: [ uppercase | lowercase]
  text-align (example left, center, right; default is left)
  text-align: [ LEFT | CENTER |  RIGHT]

- Example Code: line-height: 1.5 em
  Best practice here is em, but pixel is ok
  Bigger spacing means easier to read
  Line Height is the addition of leading space (leading space) + font size
  Thus the leading space is the space between the lines
  Easy to set double spaced, 1.5 spacing, etc.

- Example Code: word-spacing: 0.3em
  Default word spacing is 0.25em, also best practice unit choice

- Example Code: letter-spacing: 0.3em
  Called Kerning
  Can increase the readability of UpperCase Letters

General Adding Images
- Images should be saved at the dimensions they will be used at in the webpage
  Needs a lesson on Aspect Ratio and scaling
- Use Web Resizer for image size and dimensions (also has an API)
  http://webresizer.com/
- All images have width and height of elements, similar to previous width and heights
- Example Code about Products and Resizing Images (Skills Canada)
- Example
  Centering an Image – must be a block level element
    Default behavior of image is in-line
    This must be changed
  img.leaf { width: 300px; height: 200px; display: block; }
    Now it can be centered as a block level element
  Example code to center image left and right
    Note: this is an img element using .leaf class
  img.leaf { width: 300px; height: 200px; display: block; margin: 0px auto; }
  To align images to the left and right, use the float property discussed in Positioning of Block Elements
  See CSS_Block-levelSpacing_Float.txt

Adding Images Advanced Codes
- background-size: [ cover | contain ]
  Modifies the size, two most common ways are below
  Cover - expands the image as large as possible to cover the full width or height of a container.
          If the dimensions of the container (say, a div) are larger than the dimensions of the image,
          the image will become distorted.
          This value is best for images that don't communicate important content to the user,
          like background images.
  Cover, Caution: original image dimensions are important
  Contain - expands the image as large as possible, but the image will be letterboxed,
            which means it won't cover the full width or height of a container.
  Contain, Caution: image will seem like a wide-screen
- background-attachment: [ scroll | fixed ]
  scroll - image moves up and down as a user scrolls the web page (default value)
  fixed - pins the image's position on the page, in scrolling element
- Adding colour gradients to the background image
  With this work with a Z_property so colour gradients can be added around an image?
  Example Code: background-image: -webkit-linear-gradient( HexColourFrom, HexColourTo ] )
  First Hex Colour is the colour at the top or on the left
  Second Hex Color is on the other side


Block-level spacing for images

Block level elements seem to count starting from (0,0) and set out space in width and height
First coded block level element works from (0,0), then second coded elements count from there
All units for block level elements are pixels, ems, or percentages

If using classes in .css, block level elements seem to be like a loop
(actually similar to class-level or object-oriented programming)
Each element added to the page that uses these classes will the width and height
but will start counting where the other element stopped
Presumption: top to bottom, left to right

Example Code: position: [ static | relative | absolute | fixed ]
•	static - the default value (it does not need to be specified)
•	relative – relative to static position
•	absolute – the rest of the page ignores the element and acts like it is not on the page,
  but will scroll out of the page
•	fixed – moved to the back of the layers, able to scroll over top of the element
  (navigation bars do this, titles, sections headers, summaries, etc.
•	Note: fixed is often coded with the z-index property

Example, Notice how
box-bottom { width: 100%; height: 60px; position: static; }
Turns into
.box-bottom { width: 100%; height: 60px; position: relative; top: 20px; left: 50px; }
Moving the box down 20 and right 50
“Starting place is static and start counting”

Relative has four offset properties.
Will only work if position is set to relative
Definitions of Offset Properties
•	top - moves the element down.
•	bottom - moves the element up.
•	left - moves the element right.
•	right - moves the element left.

Static and Relative count together, absolute does not count where the other left off
Absolute starts at (0,0)

Fixed elements will not scroll on the page and other elements will scroll underneath them
Fixed elements start counting at (0,0)

Will all these positions, elements will start overlapping each other
Z-Index Property specifies a level to layer of elements
Thus, elements coded later (should be on top) can be placed underneath

Example Code: second .box is underneath the first
.box-top { position: relative; z-index: 2; }
.box-bottom { position: absolute; top: 20px; left: 50px; z-index: 1; }

Float Property – moving elements as far left or as far right as possible
Example code: { float: [ left | right ] }

Problem: elements will start bumping into each other
Solution: set details of what happens on the sides of the bumping

The clear property specifies how elements should behave when they bump into each other on the page. It can take on one of the following values:
•	left — the left side of the element will not touch any other element within the same containing element.
•	right — the right side of the element will not touch any other element within the same containing element.
•	both — neither side of the element will touch any other element within the same containing element.
•	none — the element can touch either side.

Example code: {clear: [ left | right | both | none ] }

---
