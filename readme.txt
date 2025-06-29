HTML(Basics)
Hypertext markup language.
(giving instructions give to computer)
<> :- opening tag
</> :- closing tag.
<button></button> :- used to create button.
<p></p> :- to write a paragraph.
(follows instructions from top to bottom)

button and paragraph are html element.
<> important to write this and </> because these are syntax

How to link to another website?
<a></a> :- 'a' is the anchor element.(link to another website)
(<a href=""></a>)

href="https://www.youtube.com" :- this is html attribute (modifies how an element behaves.)
<a href="" target=""></a> :- target is another html attribute which detrmines whether the link opens in another page or in the same page.
target="_blank"; will open the link in new page.

<p>This      is a paragraph.</p> (in html extra spaces are ignored).

----------------

Now to style the button we move to css (cascading style sheet)
<style>
 {we write css code here}
 button {
       (here button is the css selector which says which part of code we're targeting.)
 } (element name)
 .subscribe{
    (class name)
 }
 we have to class:
 1. open class
 2. retricted class.

</style> :- used to give layout,appearance to a text/button
height:50px; (px->pixels)
(css property:css value).

GENERAL TECHNIQUE:
1. Create a button with html.
2. Style with css one-by-one.

next html attribute; 'class' to specify a particular element of html.

border-radius: is used to make the border edges curve.
font-weight: used to make the font bold;
cursor:pointer :- used to make the cursor as hand button when hover over text.
border-style: solid.
--------------------------------------

Hovers,transitions and shadows;
we gonna create new css block; .subscribe-button:hover (to create a hover over the button)
(This type of class is called pseudo-class).
opacaity (ranges 0-1) o is completely transparent and 1 is opaque.

transition used to smoothly change things.

shadow : we use box-shadow (which takes four values 0 0 0 color)
(horizontal,vertical,blurr,color).

padding: spacing inside of button.
css BOX model:
1. how much space and element takes up.
2. how far is it away from other elements.

we set width in text to force the text onto the next line.
spacing between lines we use: line-height.
for special symbols like dot and tick marks, we create html entity.

p{
        font-family: Arial, Helvetica, sans-serif;
}
(applied to all paragraph)

css specificity:- class name selector>element name selector.

to underline only a specific part of the paragraph we gonna learn text element.
<p>Hello my <strong>name</strong> is asmita roy.</p>, <u></u> (fo underlining particular part of text)
strong element is used to bold, <span></span> element is used to apply our own styles to part of our text and u elemnt is used to underline.

we need a proper html structure.
<!DOCTYPE html> (uses modern version of browser).
<!DOCTYPE html>
<html>
    <head>

    </head>
    <body>

    </body>
</html>
(proper structure of html)
all the paragraph and buttons should go in body and head should contain the name of page.

live server will not work if we don't have proper html structure with us.
the things that show in our web page (like buttons and paragraph) goes in the body element and the things that don't show physically like style goes in the head element.

we require a new element to link the css file into our html code.

called link element. this is a type of void element that don't require a closing element.

<link rel="stylesheet" href="styles/buttons.css">
(file path in href)

we can also load new font to our web page.
some common fonts used are arial and times new roman.
we have used another void element <img src="">. to load image into our html.

when we set the width of the image, the height automatically also changes.
next we're gonna learn how to create a search box.(just like in youtube)
<input> element is another void element used for creating search box.
(either text or checkbox).

Display property:
1. block element (takes up an entire space like paragraph)
2. inline-block element (only takes up as much space as needed)
3. inline element (within a line of text)

display:inline-block (we can change the block property to inline block)

next html element is the <div></div> element:- what is div?? its just a box.
div is a block element just like paragraph.
divs are containers that helps to group elements together.
next thing we're learning is layout techniques. (we have two layouts vertical and horizontal layouts.)
next thing we are learning is inline styles in div element.
which will apply the that block.

1fr:- free space.
div inline style properties display:grid; grid-template-columns: 1fr; row-gap:20px; column-gap:20px.

FLEXBOX:-
-------------------------
Another similar way to create layout just like css grid.
flexbox takes as much space as needed (behaves like inline block element).
(flexible box or flexbox).
in grid for remaining amount of space we used 1fr (in grid-template-columns for how many columns we wanted).
in flex we use flex-direction:row (for positioning of flex box)
flex:1 (for taking remaning amount of space).
in grid if we move the position of columns the width doesn't do any effect to them (the layout doesn't change)
in flexbox the layout changes with the width if we move it.
justify-content:- used to adjust the divs in start,end or anywhere in flexbox.

margin:0 (sets all sides margins to the edges).

align-items:center (flexbox properties).
gap(works both for row and column gap).

margin-left:-1px (for negative spacing to join two elements with edge)
css position (allows us to fix one element at the top of the page and scroll down the rest of it.)
position:absolute (moves with page)
position:fixed (is broser window doesn't move when we scroll down)
z-index: (is used when we wanna put elements one above another)
responsive design: (when we resize our window only two videos appear there and full screen three videos are there)
we use @media for this.
white-space: nowrap; (used to so that text doesn't come on another line).


