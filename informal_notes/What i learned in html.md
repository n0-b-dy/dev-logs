# What I Learned in HTML

CTRL + U = displays the html or view page source

<br> = line break only needs one tag does **not** self close

<hr> = tag makes a break in the paragraph by showing a horizontal line. used on paragraphs. Also used to separate content. Also empty tag. (no end tag)

While html ignores the text format when typing, the preformatted text element tag <pre> keeps the text format. Preserves both spaces and line breaks.

## Paragraph Tags

color = text color
font-family = text fonts
font-size = text sizes
text-align = text-alignment


<b> - Bold text
<strong> - Important text
<i> - Italic text
<em> - Emphasized text = kinda like italics 
<mark> - Marked text = highlights the text
<small> - Smaller text = smller text than paragraph
    <del> - Deleted text = provieds a line through the text.
    <ins> - Inserted text = usually underlines the text
    <sub> - Subscript text ex. Subscript text can be used for chemical formulas, like H2O
    <sup> - Superscript text = can be  used for footnotes like <p>WWW <sup>[1]<sup> <p>

<blockquote> = elemetns that is quoted from another source (adds quotations and indents)
<q> = short quotations
<abbr> = it defines an abbreviation or an acronym. so when you mouse over the abbreviated text it defines it. ex.  <p>The <abbr title="World Health Organization">WHO</abbr> was founded in 1948.</p> 

<!-- ctrl + / --> = comment tag

## Links

<a href="url">link text</a>
By default, links will appear as follows in all browsers:

    An unvisited link is underlined and blue
    A visited link is underlined and purple
    An active link is underlined and red

## Target Attribute

target attr = the link you click on will be displaye in the CURRENT browser window.   To open a new window specify a target/

    _self - Default. Opens the document in the same window/tab as it was clicked
    _blank - Opens the document in a new window or tab
    _parent - Opens the document in the parent frame
    _top - Opens the document in the full body of the window

     <a href="https://www.w3schools.com/" target="_blank">Visit W3Schools!</a> 

     absolute links = link to a full web address (https://www.)
     relative link - link to page within website (without https://www.)

     <h2>Relative URLs</h2>
<p><a href="html_images.asp">HTML Images</a></p>
<p><a href="/css/default.asp">CSS Tutorial</a></p>

you can link to an email address using 
 <a href="mailto:someone@example.com">Send email</a> 

you can  also use an image as a link

bookmark link can be useful to skip a huge chunk of reading to the part you need down the page
 ordered lists = numbers
 unordered lists = bullet points 


## Block-level Elements

A block-level element always starts on a new line, and the browsers automatically add some space (a margin) before and after the element.

A block-level element always takes up the full width available (stretches out to the left and right as far as it can).

Two commonly used block elements are: <p> and <div>.

The <p> element defines a paragraph in an HTML document.

The <div> element defines a division or a section in an HTML document.

The <div> element is by default a block element, meaning that it takes all available width, and comes with line breaks before and after.

The <div> element is often used to group sections of a web page together.

## HTML Iframes

Iframes are pretty cool because it allows a we apge to be displayed within a web page.
syntax: 
 <iframe src="url" title="description"></iframe> 


    The HTML <iframe> tag specifies an inline frame
    The src attribute defines the URL of the page to embed
    Always include a title attribute (for screen readers)
    The height and width attributes specify the size of the iframe
    Use border:none; to remove the border around the iframe

you can also can set a target for a link.


Did not know you can use javascript within html.

The viewport is the user's visible area of a web page. It varies with the device - it will be smaller on a mobile phone than on a computer screen.

## semantics

it just describes what it means to the browser and developer.

you want to get used to using semantics in your code. 

Non-semantic elements are div and span - explain nothing about its content.
semantic is form table and article - visibly defines its content.

### section

sections usually group content normally with a heading.
ex. chapters, intro, news items, contact info.

Web could e spplit into intro, content, and contact info.

### articles

This element specifies self-contained content, independent of the web site.
ex. forum posts, blog posts, user comments, products cards, newspaper articles.

### header 

you can introcue something or put nav links in it.
usually contains heading elelements, logo or icon, authorship info.

### Footer

can be used in documentation or section

ex. 
    authorship information
    copyright information
    contact information
    sitemap
    back to top links
    related documents

<nav> 
<a href="/html/">HTML</a> |
  <a href="/css/">CSS</a> |
  </nav>

<aside></aside> element is showing some content aside fromthe the main content off to the side.
It should be used with css for proer styling.

<Figure> tag specifies self-contnained content, like illustrations, diagrams, photos, code listings, etc.
<figcaption> defines a caption for a figure element. 

                (hex code)
<p>fire emoji: &#x1F525;</p>
theres also deciamls for emoji's but i chose hex code

## HTML Images

### Image Maps

<map> tag is used on images to create clickable areas <area> on a image. You can put one or more area tags.


## HTML Bookmarks

you create bookmarks to click and jump to certain sections the webpage or document. i.e. "Jump to chapter 4" You do this by creating id's within the header tags or whatever p tags you want to jump to. Then you add a link within the same page (locally) or you can insert an external link. Dont forget to use the hashtag id within the link.













































### Form

<form></form>

<input type="text"> = displays a single line
<input type="radio"> = displays a radio button for selecting choices
<input type="checkbox"> = displays a checkbox for selecting zero or many more choices
<input type="submit"> = displays a submit button
<input type="button"> = displays a clickable button

<input type="text"> = displays a single-line input field for text input

<label> element
it defines the label for many form elements.
it is also useful for screen-readers and wil read-out loud.
also helps users with difficutly clicking on small regions (radio buutons or checkboxes)
the for attribute of the label element should e equal of the id attribute of the input element to bind them together.

RADIO BUTTONS
let a user select ONE of a limited number of choices.

CHECKBOXES
let user select ZERO or MORE options of a limtied number of choices.

SUBMIT BUTTON
submits form data to a form-handler.
the form-handler is a normally a file on the serve with a script for proccessing data.
the form-handler is specified in the action attr. 

ex. <form action="/action_page.php">

NAME ATTR. FOR <INPUT>
if the name attr is not present the value of the input field will not be sent, so it needs to be there.

















































