# CSS Part 1

# CSS Selectors

CSS selectors are used to "find" (or select) the HTML elements you want to style.

We can divide CSS selectors into five categories:

- Simple selectors (select elements based on name, id, class)
- [Combinator selectors](https://www.w3schools.com/css/css_combinators.asp) (select elements based on a specific relationship between them)
- [Pseudo-class selectors](https://www.w3schools.com/css/css_pseudo_classes.asp) (select elements based on a certain state)
- [Pseudo-elements selectors](https://www.w3schools.com/css/css_pseudo_elements.asp) (select and style a part of an element)
- [Attribute selectors](https://www.w3schools.com/css/css_attribute_selectors.asp) (select elements based on an attribute or attribute value)

# The CSS element Selector

The element selector selects HTML elements based on the element name.

# Example

```css
p {

text-align: center;

color: red;

}
```

Here, all <p> elements on the page will be center-aligned, with a red text color:

p {  text-align: center;  color: red;}

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_syntax_element)

---

# The CSS id Selector

The id selector uses the id attribute of an HTML element to select a specific element.

The id of an element is unique within a page, so the id selector is used to select one unique element!

To select an element with a specific id, write a hash (#) character, followed by the id of the element.

# Example

The CSS rule below will be applied to the HTML element with id="para1":

```css
#para1 {  

text-align: center;

  color: red;

}
```

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_syntax_id)

**Note:** An id name cannot start with a number!

---

---

# The CSS class Selector

The class selector selects HTML elements with a specific class attribute.

To select elements with a specific class, write a period (.) character, followed by the class name.

# Example

In this example all HTML elements with class="center" will be red and center-aligned:

```css
.center {  

text-align: center;

 color: red;
}
```

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_syntax_class)

You can also specify that only specific HTML elements should be affected by a class.

# Example

In this example only <p> elements with class="center" will be red and center-aligned:

```css
p.center {  
text-align: center;
  color: red;
}
```

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_syntax_element_class)

HTML elements can also refer to more than one class.

# Example

In this example the <p> element will be styled according to class="center" and to class="large":

```css
<p class="center large">This paragraph refers to two classes.</p>
```

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_syntax_element_class2)

**Note:** A class name cannot start with a number!

---

# The CSS Universal Selector

The universal selector (*) selects all HTML elements on the page.

# Example

The CSS rule below will affect every HTML element on the page:

```css
*{
 text-align: center;
 color: blue;
}
```

[Try it Yourself »](https://www.w3schools.com/css/tryit.asp?filename=trycss_syntax_universal)

---

# The CSS Grouping Selector

The grouping selector selects all the HTML elements with the same style definitions.

Look at the following CSS code (the h1, h2, and p elements have the same style definitions):

h1 {  text-align: center;  color: red;}h2 {  text-align: center;  color: red;}p {  text-align: center;  color: red;}

It will be better to group the selectors, to minimize the code.

To group selectors, separate each selector with a comma.

# Example

In this example we have grouped the selectors from the code above:

```css
h1, h2, p {  text-align: center;  color: red;}
```

With CSS, a color is most often specified by:

- a valid color name - like "red"
- a HEX value - like "#ff0000"
- an RGB value - like "rgb(255,0,0)"

# CSS background-attachment

The `background-attachment` property specifies whether the background image should scroll or be fixed (will not scroll with the rest of the page):

```css
body {
  background-image: url("img_tree.png");
  background-repeat: no-repeat;
  background-position: right top;
  background-attachment: fixed;
}
```

# Example

Specify that the background image should scroll with the rest of the page:

```css
body {
  background-image: url("img_tree.png");
  background-repeat: no-repeat;
  background-position: right top;
  background-attachment: scroll;
}
```

## In CSS, there are different attributes that possess various properties. just like it uses first attribute as a parent attribute and second attribute as a descendant.

## 

![Untitled](CSS%20Part%201%208d3448f776f1404db6de58f2641eab11/Untitled.png)

## Isme jo  h1 hai wo parent h aur ho h2 hai wo child aur priority isme h1 ko jyada milegi bajaye ke h2

## There are many type of  css selectors such as

- Child selectors ~~~~
- Descendent selectors
- Chained selectors

```html
/* Child */

.box>p {
    color: firebrick;
}

/* Descendent */

.box li {
    color: blue;
}

/* Chained */

li.done {
    color: green;
}

/* Multiple Combiners */

ul p.done {
    font-size: 0.5rem;
}
```

## Output:

![Untitled](CSS%20Part%201%208d3448f776f1404db6de58f2641eab11/Untitled%201.png)

## CSS Margins

The `margin` property is a shorthand property for the following individual margin properties:

- `margin-top`
- `margin-right`
- `margin-bottom`
- `margin-left`

So, here is how it works:

If the `margin` property has four values:

- **margin: 25px 50px 75px 100px;**
    - top margin is 25px
    - right margin is 50px
    - bottom margin is 75px
    - left margin is 100px
    
    # The CSS Box Model
    
    In CSS, the term "box model" is used when talking about design and layout.
    
    The CSS box model is essentially a box that wraps around every HTML element. It consists of: margins, borders, padding, and the actual content. The image below illustrates the box model:
    
    ![Untitled](CSS%20Part%201%208d3448f776f1404db6de58f2641eab11/Untitled%202.png)
    

## CSS Links ➖

In addition, links can be styled differently depending on what **state** they are in.

The four links states are:

- `a:link` - a normal, unvisited link
- `a:visited` - a link the user has visited
- `a:hover` - a link when the user mouses over it
- `a:active` - a link the moment it is clicked

# Example

```css
/* unvisited link */
a:link {
  color: red;
}

/* visited link */
a:visited {
  color: green;
}

/* mouse over link */
a:hover {
  color: hotpink;
}

/* selected link */
a:active {
  color: blue;
}
```

When setting the style for several link states, there are some order rules:

- a:hover MUST come after a:link and a:visited
- a:active MUST come after a:hover

## CSS positioning

## The `position` property specifies the type of positioning method used for an element.

There are five different position values:

- `static`
- `relative`
- `fixed`
- `absolute`
- `sticky`

HTML elements are positioned static by default.

```css
div.static {
  position: static;
  border: 3px solid #73AD21;
}
```

## Relative :

An element with `position: relative;` is positioned relative to its normal position.

Setting the top, right, bottom, and left properties of a relatively-positioned element will cause it to be adjusted away from its normal position. Other content will not be adjusted to fit into any gap left by the element.

```css
div.relative {
  position: relative;
  left: 30px;
  border: 3px solid #73AD21;
}
```

## Fixed :

An element with `position: fixed;` is positioned relative to the viewport, which means it always stays in the same place even if the page is scrolled. The top, right, bottom, and left properties are used to position the element.

A fixed element does not leave a gap in the page where it would normally have been located.

## Z Index ➖

When elements are positioned, they can overlap other elements.

The `z-index` property specifies the stack order of an element (which element should be placed in front of, or behind, the others).

An element can have a positive or negative stack order:

# Example

```css
img {
  position: absolute;
  left: 0px;
  top: 0px;
  z-index: -1;
}
```

output➖

![Untitled](CSS%20Part%201%208d3448f776f1404db6de58f2641eab11/Untitled%203.png)

# Without z-index

If two positioned elements overlap each other without a `z-index` specified, the element defined **last in the HTML code** will be shown on top.

**Note:** `z-index` only works on [positioned elements](https://www.w3schools.com/css/css_positioning.asp) (position: absolute, position: relative, position: fixed, or position: sticky) and [flex items](https://www.w3schools.com/css/css3_flexbox.asp) (elements that are direct children of display: flex elements).

## Display :

This element helps us to display the elements is a line by using Display inline or block or none for hiding the element.