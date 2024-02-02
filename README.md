[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-24ddc0f5d75046c5622901739e7c5dd533143b0c8e959d652212380cedb1ea36.svg)](https://classroom.github.com/a/GDPVb20V)
# Mystery Function

What does the `mystery()` function in the following piece of code do? Add your
answer to this markdown file.

```javascript
function mystery(a) {
    if(a.length == 1) return a[0];
    var foo = mystery(a.slice(1, a.length))
    if(foo > a[0]) return foo;
    else return a[0];
}
```
This function finds and returns the maximum element of the parameter array. 

   if(a.length == 1) return a[0]; -> if the size of array is 1 return element

   var foo = mystery(a.slice(1, a.length)) -> foo is recursive call of fucntion with array - first elemnt

   if(foo > a[0]) return foo; -> compare foo value with first element of original array if foo > a[0] return foo else return a[0]

   
