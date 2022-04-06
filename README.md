# FreeCodeCamp-Technical-Documentation-Page
JS Technical Documentation Page

This is a solution to the [Build a Technical Documentation Page](https://www.freecodecamp.org/learn/responsive-web-design/responsive-web-design-projects/build-a-technical-documentation-page). 

## Links

- Solution URL: [https://github.com/macdeesh/FreeCodeCamp-Technical-Documentation-Page]
- Live Site URL: [https://macdeesh.github.io/FreeCodeCamp-Technical-Documentation-Page/]

## What I learned

- I have to set the viewport and default zoom if media queries work on desktop and not on mobile devices :

  ```<meta name="viewport" content="width=device-width, initial-scale=1"/>```
  
- The HTML ```<code>``` element  is used to define a piece of computer code. The content inside is displayed in the browser's default font.
  The ```<code>``` element does not preserve extra whitespace and line-breaks.To fix this, you can put the ```<code>``` element inside a ```<pre>``` element.

- To divide the whole webpage into two sections, i used the display Grid:

 ```css
   .features-grid {
      display: grid; 
      grid-template-columns: minmax(350px , auto) 1fr; 
      <!--  The grid-template-columns CSS property defines the line names and track sizing functions of the grid columns -->
      grid-template-areas: "navbar mainContent";
      <!--  Each section will have one of the two areas names: grid-area: navbar; and grid-area: mainContent; -->
      grid-gap: 0.5rem;   
   }
   ```
  
- For the navigation bar :
  
  ```css
   .navigation-bar {
      border-right: 5px solid;
      position: fixed;
      height: 100%;
      grid-area: navbar;
   }
  ```
  
- To target a list inside a section, i used: ``` #sections li { ```

- If I want the scrollbar to appear I have to use ```overflow: auto;``` :

  ```css
   .navigation-bar {
      display: block;
      overflow: auto;
      position: relative;
      width: 100%;
      max-height: 200px;
      border: none;
   }
  ```
  
## Author

- Github - [Macdeesh](https://github.com/macdeesh)
- Twitter - [@Macdiish](https://twitter.com/Macdiish)
