- `querySelector`
    - `document.querySelector`, i.e. look in the entire document
    - `element.querySelector`, i.e. within in the `element`
    - Examples
      ```javascript
      // Selects the first <p> element in the document
      const firstParagraph = document.querySelector('p');
      
      // Selects the first element with the class "my-class"
      const firstElementWithClass = document.querySelector('.my-class');
      
      // Selects the first element with the ID "my-id"
      const elementWithId = document.querySelector('#my-id');
      
      // Selects the first <div> element that is a direct child of an element with the class "container"
      const firstDivInContainer = document.querySelector('.container > div');
      
      // Selects the first <a> element within a specific parent element
      const parentElement = document.getElementById('someParent');
      const firstLinkInParent = parentElement.querySelector('a');
      
      // Check if an element was found
      if (firstParagraph) {
        console.log('First paragraph found:', firstParagraph);
      } else {
        console.log('No paragraph found.');
      }
      ```
- `querySelectorAll` finds all matched elements
