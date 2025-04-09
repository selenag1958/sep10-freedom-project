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
 ### 3/17/25:
 To continue my previous code, of course not only can you edit the column start and grid but also the rows start and end.

![Screenshot 2025-03-17 174742](https://github.com/user-attachments/assets/88f03029-8353-411e-a9bd-c01e2031cfcb)

 ##### Code :
  ```css
.item1 {
  grid-row-start: 1;
  grid-row-end: 3;
}
  ```
  * similar to the other code `start:1;` and `end:3;` shows which row you want to start in and which row to end.
  * if we also change it to  `start:2;` and `end:4;` it will change the row to take up from the second row to the bottom

![Screenshot 2025-03-17 180447](https://github.com/user-attachments/assets/d9639d8d-5168-4a5a-8eb6-d87fee1393b3)
 ##### Code :

  ```css
 .item1 {
  grid-row-start: 2;
  grid-row-end: 4;
}
  ```
 ### 3/24/25:
While the row and column gap can be useful, there is another way to do it only using one line of code.

 That's the `grid-column` and  `grid-row` property which allows you to state where you want your row or column at beginning or end.

### 3/28/25:
After learnign different code which can help me adjust and customize a grid to my liking i want to try addingthem all together and making a grid adding different items in various sizes.

 First a used the css grid to make a format
 ![grid format](https://github.com/user-attachments/assets/eda367da-7306-471f-a2cf-c7b361c1db69)

 ##### CSS Code 
   ```css
 .grid-container {
  display: grid;
  grid-template-columns: auto auto auto;
  gap: 10px;
  background-color:#dda0dd
;
  padding: 10px;
}

.grid-container > div {
  background-color: white;
  color:black;
  padding: 10px;
  font-size: 30px;
  text-align: center;
}

.item1 {
  grid-column: 1 / span 2;
}

.item2 {
  grid-column: 3;
  grid-row: 1 / span 2;
}

.item5 {
  grid-column: 1 / span 3;
}
```

 The CSS grid allows me to create simple formats which can be helpful when planning how to format a website or project.
 . The `gap: 10px;` is used to add space between them
 . The heading is made with  `grid-column: 1 / span 2;` 
 . Image is made with `  grid-column: 3;` and `grid-row: 1 / span 2;`
 . The ending is made with  `grid-column: 1 / span 3;`

 Then we could simply add content, since this is just example and for learning I am going to add random context.
 ![flower-grid](https://github.com/user-attachments/assets/1d595f3f-a0e8-4f43-bc72-283851361320)
 #### After adding content this us the result

### Date: 4/8/25
<ul>
  <li>justify-self</li>
  <li>justify-items</li>
  <li>justify-area</li>
</ul>

##### justify-self
`justify-self` aligns items along the row axis.
##### justify-items
`justify-items` also helps align items along the row axis however they are also used with the following values:
<ul>
  <li>auto</li>
  <li> start- at the start of the grid item box</li>
  <img src = "https://css-tricks.com/wp-content/uploads/2018/11/justify-items-start.svg" height=200 width =200>
  <li> end - at the end of the grid item box </li>
  <img src= "https://css-tricks.com/wp-content/uploads/2018/11/justify-items-end.svg" height = 200 width = 200>
  <li> center - in the center of the grid item box </li>
  <img src= "https://css-tricks.com/wp-content/uploads/2018/11/justify-items-center.svg" height = 200 width =200>
  <li> stretch - extends all throughout the grid item boxes </li>
  <img src = "https://css-tricks.com/wp-content/uploads/2018/11/justify-items-stretch.svg" height = 200 width = 200>
</ul>

##### grid-area

`grid-area` is a short way of using `grid-row strart` + `grid-column start`+ `grid-row end` + `grid-column end`.   

##### place-self
`place-self` is using both `align-self` and `justify-self` together in one.

For example `place-self: center stretch;` creates : 

<img src = "https://css-tricks.com/wp-content/uploads/2018/11/place-self-center-stretch.svg" height= 200 width= 200>

### 4/9/25
##### place-content
`place-content` connects `align-content` and `justify-content` into one.
`place-content` is written in this format: `align-content`/`justiffy-content`

##### subgrid
A subgrid is when a grid-item has their own grid lines.
<!-- 
* Links you used today (websites, videos, etc)
* Things you tried, progress you made, etc
* Challenges, a-ha moments, etc
* Questions you still have
* What you're going to try next
-->
