# HTML-Elements
The differences between Block or Inline HTML Elements.
Every HTML element has a default ```+display``` value based on the type of element it is:<br>

There are 2 basic types of HTML elements:
<ol>
  <li>Block level elements display block</li>
  <li>Inline elements display in-line</li>
</ol>


#### Block Level Elements<br>
###### Block level tags take up as much horizontal (width) space as possible and push the next block level element down. They always start on a new line and stack down the page.<br>
The browsers automatically adds some space (a margin) before and after the element.<br>
To eliminate the margins between block elements set their margins to zero:<br>
 
`p { margin: 0; }`<br>

###### A paragraph is a block level element. Each new paragraph tag will stack vertically. <br>
In a horizontal writing mode: <br>
![image](https://github.com/nafizjiwa/HTML-Elements/assets/56348190/c7d9de13-c2bd-4e36-b546-ee9fe4d8414e)<br>

Since block elements will consume all of the space in the inline direction a paragraph will spread out and get as big as it can inside their containing block.
However, if we give them a width, they will continue to lay out one below the other - even if there is space for them to be side by side. <br>
![image](https://github.com/nafizjiwa/HTML-Elements/assets/56348190/727ac119-b160-4059-bc54-9ef3e2c3dcde)<br>


#### Examples of block level elements:<br>
<ul>
  <li>Paragraphs</li>
  <li>Ordered <ol>, Unordered Lists <ul> and their list items <li> </li>
  <li>All headings: h1 -> h6 </li>
  <li>Div, footer, section, nav, table etc...</li>
</ul><br>


#### Inline Elements<br>
###### Inline elements display in a line, one after the other in that direction. They <em>will not force the text</em> after them to a new line.<br>
###### They only take up the width or space they need, no more.<br>

###### An anchor (or link) is an example of an inline element. You can put several links in a row, and they will display in a line.<br>

#### Examples of inline elements:<br>
<ul>
  <li>Anchors <a></li>
  <li>Strong <strong> and Emphasis (em)s</li>
  <li>Span <span></li>
  <li>Button</li>
  <li>Imput <input></li>
  <li>Image <img></li>
</ul><br>

###### Why is this important?<br>
###### Inline elements cannot contain block level elements<br>
###### For example, a link cannot be wrapped around a header:<br>
    <a href="http://example.com/"><h1>This is invalid HTML</h1></a>	← Incorrect 
<br>

###### The correct way to do this would be to put the inline element inside the block element:<br>
    <h1><a href="http://example.com/">This is invalid HTML</a></h1>	← Correct 
<br>

# Override The Default Display Value
So, every element has a default display value either block or inline. However, you can override this.<br>
Changing an inline element to a block element, or vice versa, is helpful to make a page look a specific way.<br>

An example is making inline <li> elements for horizontal menus:<br>
<li> is a block element and to make it inline we change its display property to inline from block.<br>
  
    <li>list 1</li>
    <li>list 2</li>

The above displays:<br>

`list 1`<br>
`list 2`<br>

To make the list display horizonal we add a display property to it CSS with a value of inline and not block do as so:<br>

`li {`<br>
  `display: inline;`<br>
    `}`<br>

The result is :<br>

`List 1 List 2`<br>

Another example is making an inline element <span> display as block. <br>

     <span>A display property with</span> <span>a value of "block" results as </span>

###### It displays as:<br>
`A display property with a value of "block" results`

To display as a block element on a seperate lines we add this code to the CSS style:<br>

`span {`<br>
  `display: block;`<br>
      `}`<br>

###### It displays as:<br>
`A display property with`<br>
`a value of "block" results`


