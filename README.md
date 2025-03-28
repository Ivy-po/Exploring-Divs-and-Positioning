# Exploring Divs and Positioning
There are several items for you to explore today.

1) The images do not currently work. Look at the code for the images and fix the mistakes so that the Ghost images are properly displayed. This is a common mistake that many students are making...
2) Examine at the `style.css` stylesheet. What properties and values have we not learned yet?
    * Take some time with your partner to modify some of the new values to figure out what they do.
    * You can always use the history to undo changes that you don't want to save.
    * You could also use the inspect tool to do this without actually modifying the `style.css` document.
    * Finally which property would you like us to discuss?
4) Currently the section on Blinky has a `.blinky` class applied to it. This is why the Blinky section has some style.
    * Fix the **Inky** section with your partner to match the Blinky section (only with colors that apply to Inky).
    * Do the same for **Pinky** and **Clyde**.

This looks pretty good. Try modifying the `width` of the images in the .CSS document to `25%` instead of `100px`. What happens? Why do you think it happened? How could you fix it?

Make your fix then try adjusting the size of the screen. What happens?

Let's try it a different way now. Remove the 3 lines of CSS code that have comments `/* <-- old way */`


## Divs and flex
A `<div></div>` element represents a division of the page. It is used to group elements together. This is a common way to position and style elements on a webpage.

The CSS property of `display` can be set to `flex` which allows us to place elements on the page horizontally. It also provides better options for spacing elements.

1) Create a new CSS rule as follows:
    ```
    .ghost{
        display: flex;
    }
    ```
2) Create a sets of `<div></div>` tags for the the Blinky section as shown below.
    ```
    <div>  <!-- Outer Div -->

    </div>
    ```

3) Next move the code from the Blinky section to between the opening and closing `div` tags. This looks close to what we want because the image, h2, and paragraph elements are all horizontally aligned. But what we really want is the image, next to the h2 and paragraph, with the h2 and paragraph stacked.

4) Then add a `class="ghost"` attribute to the opening `<div>` tag of the outer `<div>`. This will put all of the Blinky code in a division of the page for that specific ghost. 
5) Create 2 more sets of `<div></div>` tags for the the Blinky section as shown below.
    ```
    <div>  <!-- Outer Div -->
        <div>
            <!-- Inner Div 1 -->
        </div>
        <div>
            <!-- Inner Div 2 -->
        </div>
    </div>
    ```
6) Move the Blinky image and text code into the inner `<div>`s
   1) Place the image inside the the 1st inner `<div>`.
   2) Place both the Heading and paragraph in the 2nd inner `<div>'.

Since the outer <div> with the `class="ghost"` has the `display: flex` property, it displays elements horizontally. When we moved the image, heading and paragraph into the `<div>`s now there are only 2 children to be placed horizontally and the element inside the inner `<div>`s are stacked vertically.
