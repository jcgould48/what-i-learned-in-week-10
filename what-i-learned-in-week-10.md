## What I learned in week 10

### CSS Grid
Alternative to flex-box to put items into grid boxes.

Example:
```CSS
#app {
  display: grid;
  grid-template-columns: 1fr 50%  3fr;
  grid-template-rows: repeat(5, 50px);
}
#space-8 {
  grid-row: 4/6;
  grid-column: 1/4;
}
```
With this method, you can assign an object a specific column/row or have the object stretch across multiple.
