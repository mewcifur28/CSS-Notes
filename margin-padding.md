## Margins

- The spacing between heading elements, as well as paragraphs is controlled by **margin-top** and **margin-bottom**.
- By default, margin-top and margin-bottom is equal to the font-size (except H1).

### Centre

- To center an element on screen, make the margin-left and margin-right of that element itself, *auto*

### Collapse

- By default margins collapse into one another.
- So if one element has a margin-bottom "*x*" and the next element has a margin-top "*y*", the space between them will be *max(x, y)* **not** *(x+y)*.

### Move the heading down

- **Margins collapse any time they touch each other.** If the first child in the element has a margin-top it can merge with the parent's margin-top.

- If you have a box, and inside the box there is some element, for eg

  ```html
  <div class="card">
      <h1> my heading </h1>
  </div>
  ```

   Now if you want to move the heading down IN the card, changing margin-top of h1 will not work because the margins will collapse, the margin-top of card will also become margin-top of the H1 and the whole card is shifted down.

- In general, the background-color will always be on the parent, so we can **add padding to the parent** to prevent the margins of child and parent merging.

### Consistency

- Turn off the margin-top on typography related elements, this way you can use padding on the parent and know the exact spacing you'll be getting.
- In layouts will flexbox and grids, margins no longer collapse.
- Find the last element and turn the margin-bottom off.

