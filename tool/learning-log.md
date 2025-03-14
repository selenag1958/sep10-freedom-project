# Tool Learning Log

## Tool: **CSS Grid**

---

### 3/8/25:
* Since I already have a small introduction to grids and what I have been learning in bootstrap using css grid properties I want to try learning and applying new properties
* One property is creating gaps in between your columns.
* The gap property allows you to add space between your rows AND columns.
  Ex: without the gaps
  ![Code example](https://github.com/user-attachments/assets/6be527c7-ec1e-4a7b-937b-bf7cfa4e5a4c)
  
  With the gap property:
  ![Code example](https://github.com/user-attachments/assets/f20dee4d-c913-4850-b5ce-b4a76ccbd38f)
  
  Code used :
  ```css
  .container {
  display: grid;
  gap:50px;
  grid-template-columns: auto auto auto;
  background-color: #FFEBCD;
  padding: 10px;
  }
  ```
* I think this property will be useful in spacing out my content so that everything isn't so close to each other. So that both images and text have space.

### 3/10/25:
* Gap property is all around an item to be more specific you can use:

   * colum-gap
   * row-gap
   * This allows you to be more specific.
  ##### Column Gap:
  ![Column Gap](https://github.com/user-attachments/assets/d5d969e5-dc87-4140-9dba-32b72a17809c)

  
   ```css
   .container {
  display: grid;
  column-gap: 50px;
  grid-template-columns: auto auto auto;
  background-color: #FFEBCD;
  padding: 10px;}
   ```

  ##### Row Gap:
  


<!-- 
* Links you used today (websites, videos, etc)
* Things you tried, progress you made, etc
* Challenges, a-ha moments, etc
* Questions you still have
* What you're going to try next
-->
