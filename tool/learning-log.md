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
  ![Row Gap](https://github.com/user-attachments/assets/6a989f17-5575-41c3-bf14-ee0f8de1ba95)
  ```css
  .container {
  display: grid;
  row-gap: 50px;
  grid-template-columns: auto auto auto;
  background-color: rgb(205, 98, 93);
  padding: 10px;
  }
  
   ```

 ### 3/16/25: 
 As I continue to see how I can format a grid and how I can make it to a design I like I learned about another way i can edit each grid item.The column start and end property is as its name suggest you can state where you want your column to start and where you want your column to end.

 <img width="452" alt="image" src="https://github.com/user-attachments/assets/887cb198-b2ce-4100-9ffb-96e1c9485ff6" />
 
  ```css
  .item1 {
  grid-column-start: 1;
  grid-column-end: 3;
}
  ```

* By adding `column-end: 3;` it means that the end of the column was at the beginning of column 3
* If you had written `column-start: 2;` and `column-end: 4;` it would remove the first item in column 1 and extend until the end of the first row.

![Screenshot 2025-03-16 230429](https://github.com/user-attachments/assets/3d13fcab-7099-4668-b649-2d85bc90378e)

  
* Code :
  ```css
  .item1 {
  grid-column-start: 2;
  grid-column-end: 4;
  }

 ```


 


<!-- 
* Links you used today (websites, videos, etc)
* Things you tried, progress you made, etc
* Challenges, a-ha moments, etc
* Questions you still have
* What you're going to try next
-->
