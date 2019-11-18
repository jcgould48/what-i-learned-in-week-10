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

To make it more user friendly there is also the ability to name the columns and rows.

```CSS
grid-template-rows: [start] 1fr [top-middle] 2fr [middle] 2fr [bottom-middle] 1fr [end];
grid-template-columns: [start] 70px [left-middle] 300px [right-middle] 100px [end];

#header { 
  grid-row: start / top-middle;
  grid-column: start / end;
}

```

***

Another way is using grid areas command to set the grid areas. Each line of string that is enclosed in quotes represents a new row.

```CSS
grid-template-areas:
    "area-1 area-2"
    "area-3 area-4"
  ;


#square-1 {
  grid-area: area-1
}
```

***

