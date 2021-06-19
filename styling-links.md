## Styling Links to look like Buttons

### Order of styling (*pseudo classes*)

- *a:link* (default)
- *a:visited*
- *a:focus*
- *a:hover*
- *a:active*

### General Rules

- It should be obvious that a link can be interacted with, change color on hover and focus.
- Leave the text-decoration as it is, and if you remove it, ensure that it is still obvious that the link is a link.
- Remember to include styles for *focus* along with *hover* for accessibility purposes.

### Styling Buttons

- The styling should be on the **link** itself, not on a wrapper element.

  ```html
  <!--RIGHT-->
  <a class"button" href="#">My Link</a> 
  
  <!--WRONG-->
  <span class="button"><a href="#">My Link</a></span>
  ```

- Inline elements cannot render top and bottom stuff properly, so use inline-block.

  ```css
  display: inline-block;
  ```

- NEVER set width & height, instead use padding and use a **1 : 2.5** ratio for top and sides padding.

- Look for inspiration online to design beautiful buttons.