# HTML-Elements
The differences between Block or Inline HTML Elements.

There are 2 basic types of HTML elements:
<ol>
  <li>Block level elements</li>
  <li>Inline elements</li>
</ol>


#### Block Level Elements<br>
###### Block level tags take up as much horizontal (width) space as possible and push the next block level element down. They always start on a new line and stack down the page.<br>
The browsers automatically adds some space (a margin) before and after the element.<br>
To eliminate the margins between block elements set their margins to zero:<br>
 
`p { margin: 0; }`

###### A paragraph is a block level element. Each new paragraph tag will stack vertically. <br>
In a horizontal writing mode: <br>
![image](https://github.com/nafizjiwa/HTML-Elements/assets/56348190/c7d9de13-c2bd-4e36-b546-ee9fe4d8414e)<br>


#### Examples of block level elements:<br>
<ul>
  <li>Paragraphs</li>
  <li>Ordered and Unordered Lists</li>
  <li>All headings: h1 -> h6 </li>
  <li>Div, footer, section, nav, table etc...</li>
</ul><br>


#### Inline Elements<br>
###### Inline elements display in a line. They <em>do not force the text</em> after them to a new line.<br>

###### An anchor (or link) is an example of an inline element. You can put several links in a row, and they will display in a line.<br>

#### Examples of inline elements:<br>
<ul>
  <li>Anchors</li>
  <li>Strong and Emphasis (em)s</li>
  <li>Code</li>
  <li>Anchors</li>
  <li>Strong and Emphasis (em)s</li>
  <li>Code</li>
</ul><br>

###### Why is this important?<br>
###### Inline elements cannot contain block level elements<br>
###### For example, a link cannot be wrapped around a header:<br>
    <a href="http://example.com/"><h1>This is invalid HTML</h1></a>	← Incorrect 
<br>

###### The correct way to do this would be to put the inline element inside the block element:<br>
    <h1><a href="http://example.com/">This is invalid HTML</a></h1>	← Correct 
<br>
