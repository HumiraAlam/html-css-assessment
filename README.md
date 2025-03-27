# html-css-assessment-

# Q1: What is axis in CSS Flexbox? Explain with an example.#

In CSS Flexbox, an axis refers to the direction in which flex items are placed. There are two axes:

Main Axis: 
The primary axis along which flex items are laid out. It is determined by the flex-direction property (e.g., row or column).
Cross Axis: 
The perpendicular axis to the main axis. It is used for alignment (e.g., align-items).
# example
.container {
    display: flex;
    flex-direction: row; /* Main axis is horizontal */
    justify-content: center; /* Align items along the main axis */
    align-items: center; /* Align items along the cross axis */
}

<div class="container">
    <div>Item 1</div>
    <div>Item 2</div>
    <div>Item 3</div>
</div>

Q2: Can I use multiple CSS Background images in a div? Explain with an example.
Yes, we can use multiple background images in a single div using the background-image property. we can specify multiple images by separating them with commas.
# example
.div {
    width: 300px;
    height: 300px;
    background-image: url('image1.jpg'), url('image2.png');
    background-position: center, top right;
    background-size: cover, 50px 50px;
    background-repeat: no-repeat, no-repeat;
}

Q3: Code

Q4: Explain CSS Specificity
CSS specificity determines which CSS rule is applied when multiple rules target the same element. It is a way to calculate the importance of a selector.

Specificity Calculation:
Inline Styles: Highest specificity (e.g., style="color: red;").
IDs: More specific than classes (e.g., #id).
Classes, Attributes, and Pseudo-classes: Less specific than IDs (e.g., .class, [attr], :hover).
Elements and Pseudo-elements: Least specific (e.g., div, h1, ::before).
# example
/* Specificity: 0, 0, 1 (Element) */
div {
    color: blue;
}

/* Specificity: 0, 1, 0 (Class) */
.container {
    color: green;
}

/* Specificity: 1, 0, 0 (ID) */
#main {
    color: red;
}

Q5: Explain CSS Box Model

Q6: Code

Q7: Code

Q8: What are pseudo selectors? According to you explain 5 important pseudo selectors.

Q9: What are media queries? Min-width or max-width which will be more helpful on Mobile First Approach? Explain.

Q10: What is float property and why do we use clear property with float?
