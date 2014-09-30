#Tasks

-- What are the different types of selectors?
-- What are the different types of combinators?
-- What is the specificity of div#data > div + [placeholder] span
0 1 1 3
-- What is the difference between div.data and div[class="data"]
div.data is a class selector whereas div[class="data"] is attribute selector
-- What is the difference between div#data and div[id="data"]
div#data is id selector whereas div[id="data"] is attribute selector
-- Is specificity more imp or cascade
specificity
-- What are the different ways of adding CSS to your page?
Style as an in-line attribute, link and style


--Notes
CSS
How to add CSS - 3
1.Style as an attribute, link and style

Types of CSS selectors
Element selectors
Class
Attribute
Id

HTMLElement class - div is subclass of HTMLElement class

Combinators
Child div > div
Descendant div div
Adjacent sibling - always goes down li + li
Grouped selectors - using comma. div,span,#intro

Combinators dont affect specificity

Specificity
0 0 0 0
inline id class/attribute element

specificity is more important than order


span/divs

span is not a block element. It is inline element.

inline elements don’t have concept of a height

display:block converts inline element to block.

display is applicable to all elements.

display:inline - no height
display:block - has width
display:inline-block

To stack block elements next to each other : use float

float:left

overflow:auto

----Next
1.Element selector -- selects entire HTML element
 div { /* 0 0 0 0   */
            /*background-color: red;*/
        }

2.ID selector <div id ="intro">
So id selector uses # to access
#intro {
font-size: 130%;
border: 1px solid black;
}

3.Class selector
Class ssleector uses dot or period to access .
<div class ="intro">
.class{
background-color:yellow;
}

Difference: Class Selectors are very similar to ID Selectors. The major difference is that while a certain ID should only be
 assigned to one element, we can assign the same class to as many elements as we want.

4.Descendant selectors
Descendant Selectors are similar to family trees; you start with the parent element you wish to select, add a space, and continue
  naming any interior elements until you’re arrived at the specific element you wish to select
#intro .important em {
color: white;
}


Combinators
Child div > div
Descendant div div
Adjacent Sibling like li +