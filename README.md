# HTML-Elements
The differences between Block or Inline HTML Elements.

There are 2 basic types of HTML elements:
<ol>
  <li>Block level elements</li>
  <li>Inline elements</li>
</ol>


###### Block Level Elements
#### They take up space by default. They will stack down the page.

A paragraph is a block level element. Each new paragraph tag will stack vertically. Block level tags take up as much horizontal space as possible and push the next block level element down.

Examples of block level elements:

Paragraphs
Ordered and Unordered Lists
All headings
Inline Elements
Inline elements display in a line. They do not force the text after them to a new line.

An anchor (or link) is an example of an inline element. You can put several links in a row, and they will display in a line.

Examples of inline elements:

Anchors
Strong and Emphasis (em)
Code
See Demo
Why is this important?
When we get to CSS layouts, this will become very important. For now, remember this:
Inline elements cannot contain block level elements
For example, a link cannot be wrapped around a header:
<a href="http://example.com/"><h1>This is invalid HTML</h1></a>	← Incorrect
The correct way to do this would be to put the inline element inside the block element:
<h1><a href="http://example.com/">This is invalid HTML</a></h1>	← Correct
