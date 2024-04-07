# What I learned in CSS today

So to start 

so in my words 90 **viewport height** takes up 90% of the viewable screen.

also to create a **border** i would just type border then a certain px to show how thick or thin i ant the line 
(smaller is thinner, bigger is thicker)

To make the contents or "elements" of a container or class move horizontally on the page with less coding 
flex can help with that.

by default the flex-direction is set to row which make my content appear horizontally across 
the page.

so row-reverse keeps the horizontal look but changes the order. So if i had numbers as 1, 2, 3, 4
it now literally reverses the order to 4, 3, 2, 1.

to arrange these element to go up and down vertically we can use a FLEX-DIRECTION as column. One
will be at the top and 4 will be the bottom. Column reverse will just reverse the order of the numbers so opposite.
the 4 will be that the top and one will be at the bottom. 

next we have justify content property. it sets the alignment on the MAIN-AXIS. Think of the MAIN-AXIS as a 
refference to math. The MAIN-AXIS beig the X-AXIS according to planes and graph.

by deafult it will be 1-4 horizontally which will justify or align the numbers on the left which is 
default or known as FLEX-START. 
]
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

