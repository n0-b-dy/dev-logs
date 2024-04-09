# What I learned in CSS today

So to start 

so in my words 90 **viewport height** takes up 90% of the viewable screen.

## Percentages vs Pixels

*Pixels* can cover certain amount the the available screen or *viewport*. But they may take longer to calculate. Whereas, Percentages may be easier to estimate because they take up a larger portion faster. For example, 50% of the width of the screen would take up more and be faster and easier to estimate i your head versus pixels. I think percentages are dynamic, which means they automatically stretch and shrink dependant on the viewport (vh). Pixels stay fixed on the screen, so they literally go off the edge and are more difficult to estimate.

A little nugget of extremly helpful info came from reddit about when to use a spcific unit measurement. This came from n9iels on reddit, 

> *"Pixels are fixed and percentage are (mostly) relevant to the parent element. I would use pixels only if it always needs to be that size. So for example breakpoints. But there is much more than pixel and percentages these days :)*
I personally like to use rem whenever possible. This makes it relative to the font-size of the body. So if the font-size is 16px then 2rem will be 32px. This is nice because when someone sets a custom font size it always looks good."

> *"The goal is to become familiar with the material and understand it, not to memorize it. All great developers have reference material they regularly refer to" :)* -Smoljames on YouTube



also to create a **border** i would just type border then a certain px to show how thick or thin i ant the line 
(smaller is thinner, bigger is thicker)

To make the **contents** or **"elements"** of a container or class move horizontally on the page with less coding 
flex can help with that.

by default the **flex-direction** is set to row which make my content appear horizontally across 
the page.

so **row-reverse** keeps the horizontal look but changes the order. So if i had numbers as 1, 2, 3, 4
it now literally reverses the order to 4, 3, 2, 1.

to arrange these element to go up and down vertically we can use a **FLEX-DIRECTION** as column. One
will be at the top and 4 will be the bottom. Column reverse will just reverse the order of the numbers so opposite.
the 4 will be that the top and one will be at the bottom. 

next we have justify content property. it sets the alignment on the **MAIN-AXIS**. 
Think of the MAIN-AXIS as a refference to math. The MAIN-AXIS beig the X-AXIS according to planes and graph.

by deafult it will be 1-4 horizontally which will justify or align the numbers on the left which is 
default or known as FLEX-START. 

**FLEX-END** will justify all of the content at the END or right justified.
it will move all of the contents and the bottom of the page.

by justifying the content in the center it will literally just center whaevter content i have in the literal center of the 
page. Pretty easy to remember hopefully.

by JUSTIFYING the CONTENT with the SPACE-BETWEEN value it will increase the space between the 
numbers 1  2  3  4 instead of 1234. And when i expand the page it will the keep the numbers spaced.

the SPACE-AROUND value includes the area outside of the element.

the container is all the content within that is being mainpulated. The BORDER usually outlines the container and shows both the 
margin and padding. Visually it helps to show that for me.

When selecting an id you use the hashtags symbol '#'. When reffering to a class use a period '.'

**align-items** property with the **center** value will move all of the contents to the CENTER of the page.
The **baseline** value will align the text horizontally.

**align-content** is used with flex-wrap property.

## FLEX-WRAP Property

The flex wrap property with the **wrap** value will allow the text to wrap the page by sending the text that is touching the border to start a new line.
By default it is set to to no wrap and **wrap-reverse** is starting the elements at the bottom and sending the remaining to the top.

## Main Concept To Understanding Styling

So whenever I think of styling an element it should be paramount that I first think of the element I want to style as an onion because it has a few layers that affect the way it looks.

So the **element** is on the inside of the onion, then working one layer outward is the **paddding**, after that we have the **border**, working outward once more to the last layer we have **margin**. That is the main concept that you should understand when looking into styling the elements using CSS. 

On default the CSS styling does have a border because the letters do not touch the end of the page. So to fix that you would create a class selecting the body and creating a **margin** property with the **value** set to 0 px. Then you will have the the words touching the end of the pages effectively. All that margin will be is the area outside the element.

inline = means you apply the style the as an attribute to the opening elements within the html file. 
internal = you apply the style within the HEAD element in the html tags with style tags. (ex: <style></style>)
external = you create a styles.css file and link in it with a link to in the html file.
the best method is external.

CSS colors
for colors there are three types listing the literal color i.e black, rgb values (ex: rgb(0, 0, 0)), or 
hexadeciaml values: which ALWAYS star with a hashtag '#' followed by a six-digit number, letters, or both. (ex: #000000 = black, #FFFFFF, #4287f5)

CLASSES AND IDENIFIERS
To target specific elements within your html file you use a unique identifier. (ex: 'id='). Then to select the
element in your css file you would use the hashtag followed by the element. (ex: '#p1').

Similarly, yoiu can taarget a group of elements using a CLASS attribute (ex: 'class=""'). Now to target an element by class
it is similar to id's, but instead of hashtags you would use periods '.' (ex: '.odd')

FONTS
FONT-FAMILY changes the fonts on the page. the most commonly used is sans-serif. It's good practice to use two 
fonts because some web browser's may not support one then they will use  another. Think of them like contingencies.

some fonts are font-family: "consolas", sans-serif;
fonts.google.com is a good web site to use. (ex: 'Press Start 2P')
click on "select this style". Click on "View your selected families. Then copy the api stylesheet link.
within the head of the html document paste the api stylesheet link.

within your stylesheet use the FONT-FAMILY property simply type in the quotations press start 2p.

(ex: 'font-family: "Press Start 2P", "consolas", "sans-serif" ')

there are also different stylistic featuers you can add to text such as 
font-styles: italics;
font-weight: bold;
text-decoration: cyan dotted underline;
font-size: 18px;

Borders

Borders create a box around the content or usually text. 

border-style:
solid
dashed
dotted
double
ridge
groove 
inset
outset

Border-width will cahnge the thickness of the line or border.

Border-color will change the color of the border.

Border-readius will smooth the corners of the borders. the higher the number-the smoother the rounding.

padding provides spacing between letters and border.

Border-top
Border-bottom
Border-left
Border-right

you ca also add sttyle such as border-top-style: dotted
specifically you specify what sides as well.

Border-left-style:double;
Border-left-width:10px;
Border-left-color:silver;

Borders are your boundaries of your body. Wherever the border is.


properties commonly used:

border
width
height
font-size
text-align
background
background-color
transform
animation


BACKGROUND

you can add different colors to background property in css and also add gradients

ex: background: linear-gradient(skyblue, lightgreen);
To stop it from repeating add another css property:

background-repeat: no-repeat; 
to stretch the backgrond add a thrid property.

ex: background-attachment: fixed;

you can change the direction the color changes.

ex: 	background: linear-gradient(*to top*,skyblue, lightgreen);
	background: linear-gradient(*to left*,skyblue, lightgreen);
this would reverse the colors. Green at the top, blue at the bottom.


if you were to apple the linear gradient properties to just the border of the text you can 
remove it from the body and put it in the html element that contain the text.
Such as h1 elements and paragraph elements, essentially anything that contains text.

SETTING IMAGE AS BACKGROUND

grab an image fro the web or wherever then add it to your folder conatining the html and css files then within
the body css file add background-image property.

ex: background-image: url("insert_image_filename_here.jpg"); *you can place an external url in the parentheses*

the image may not form to the page properly so here are some fixes.

copy and paste:
background-repeat: no-repeat;
background-attachment: fixed;
background-position: center;

but for it to dynamically shrink and expand to the page you have to add one more property:

background-size: cover;
Now the image will resize dyanmically.

Margin is the space outside the Border

Padding is the space between the border and the content inside the border.

you can add percentages instead of pixels, in that way it can react dynamically.

TRICK:
margin-left: auto;

will push the content to the right  of the page automatically.
 if you set both margin left and right it will keep the content centered in the middle.
if you need help, you can  always right click, then click on inspect and it will show a helpful diagram.

FLOAT PROPERTY.

Float = positions an element to the left or right side of a container.
ex. Popular for wrapping elements around images.

ex. img{float: left;}

ex. clear property = stopping point where the elemetns are no longer floating.

clear value should match float value to stop it.

Postion property
 is a property that will format the layout of an element.

position: relative;


absolute = any element will be taken out of the flow of the document.
fixed = will stay in the position of your viewport. think of annoyin popup adds.
relative = will off-set the position of the element of it original spot or origin.
think of covering words
position: relative;
*top: 50px 
left: 50px*
static = normal state; default
sticky = will stick to your viewport when your scroll past.

PSEUDO-CLASSES

elements can be in a special state forexample you can hover over them or click on them.

create a hyperlink to test.
you can change the color of a link 

ex. a:link{ color:lawngreen; }

anything that is visited is also a pseudo class 

ex. a:visitedC

a:hover { color:tomato; }

a:active = means the link is clicked actively
ex. once you click and hold

button:hover {background-color; }

tip: its good to chaange the background to a color to let the user know they can click something.

nth child pseudo class just means an element nested within an elemnent. if you have a list then all the elements
nested withing will be siblings.

li:nth-child(even){background-color: yellow}
li:nth-child(odd){background-color: yellow}

3n = every third element highlighted.
5n+0 = every fifth element or offset to specific number

SHADOWS

text-shadow: 5(x-axis) 0 (y-axis) 0 (spread) color;
 negative numbers will move shadows opposite.
 (x) positivte number to the right.neg to left
(y)  pos = shasdow above the text, neg below

the higher the number the further the spread.
 you can add multiple shadows and separating them with commas

text-shadow: 5(x-axis) 0 (y-axis) 0 (spread) color, text-shadow: 5(x-axis) 0 (y-axis) 0 (spread) color

box-shadow
same as text shadows but you may want to set width and height properties.

you can add a hover selector.

ICONS
copy the html and paste it into file then style by using class name.

ex. '.fa-twitter{color: aqua}' 

you can turn them into hyperlinks.

ANIMATIONS

To use an animation we must create one.

In CSS, use @keyframesInsert_Unique_Name
ex. @keyframes mySlide{ from{margin-left: 100%} to{margin-left: 0%} }

from{} = beginning or start
to {} = ending or finish

So, the animation propertty must be also set in the css property you want to animate. 

animation: mySlide;
animation-duration: 5s; = how long it takes

animation-iteration-count: 1 2 3 or infinite;
infinite = looping

animation-play-state: running (default)
paused = will pause the animation
animation-delay: 0s;
animation-timing-function: ease-in; accelerate
ease-in = does not slow down
ease-out = slows down
ease = both
linear = constant animation

shortcut

animation: 3s linear 0s infite running myslide;

duration
timing funtion
delay
iteration
play_state
animation_name

can add pseudo selectors 
box#1:hover = will activate the animation on mouse hover
box#1:hover = will play if clicked on

@keyframes myRotate {

100%{transform: rotateX(360deg)} = will flip the text

100%{transform: rotateY(360deg)} 

100%{transform: rotateZ(360deg)} = will rotate like like a clock
}

@keyframes myOpacity{ = this will just fade in/out the text
50%{opacity: 0;}
}

@keyframes myScale{ = this will just shrink and enlarge the content
50%{transform: scale(0.5, 0.5);}
}

@keyframes myColorChange{ = this will change the color
20%{background-color: orange;}
40%{background-color: yellow;}
60%{background-color: green;}
80%{background-color: blue;}
100%{background-color: purple;}
}

animation: 3s linear 0s infite running insert_name_here;

mySlide = whatever you name after the '@keyframes'

animation will loop back to what color your 'background: red;' property is in the selected class or id.



