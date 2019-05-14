# Array Cardio Day 1

## Table of contents

- [General info](#general-info)
- [Code Overview](#Code-Overview)
- [JavaScript Function explain](#JavaScript-Function-explain)
- [HTML layout](#HTML-layout)
- [CSS style](#CSS-style)

## General info

![Image]()

## Code Overview

### Summary

- [Array.prototype.map()](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/map)
- [Array.prototype.reduce()](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/Reduce)
- [Array.prototype.sort()](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/Sort)
- [Array.prototype.filter()](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/Filter)

# Array.prototype.filter()

- The filter() method creates a new array with all elements that pass the test implemented by the provided function. **i.e array.filter(function)**

- Returning filtered number of array

- console.table() ==> creating a table for the console

```
const fifteen = inventors.filter(function(invetor) {
  if (invetor.year >= 1500 && invetor.year < 1600) {
  return true; // Keep the value
}
});

console.table(fifteen);
```

ES6 arrow function for simplifly the code

```
  const fifteenSort = inventors.filter(inventor => inventor.year >= 1500 && inventor.year <= 1600);
      console.table(fifteen);

```

![Image](./imgs/filter.png)

# Array.prototype.map()

- The map() method creates a new array with the results of calling a provided function on **every element** in the calling array.

- return same amount of array

# Array.prototype.sort()

- The sort order can be either alphabetic or numeric, and either ascending (up) or descending (down). By default, the sort() method sorts the values as strings in alphabetical and ascending order.This works well for strings ("Apple" comes before "Banana"). However, if numbers are sorted as strings, "25" is bigger than "100", because "2" is bigger than "1".You can fix this by providing a "compare function" (See "Parameter Values" below).

* Ascending Order

       function(a, b){return a-b}

      var points = [40, 100, 1, 5, 25, 10];
      points.sort(function(a, b){return a-b});

* Descending Order

        var points = [40, 100, 1, 5, 25, 10];
        points.sort(function(a, b){return b - a});

# Array.prototype.reduce()

- The reduce() method executes a reducer function (that you provide) on each element of the array, resulting in a single output value.

```
const array1 = [1, 2, 3, 4];
const reducer = (accumulator, currentValue) => accumulator + currentValue;
// const reducer = function ()
// const reducer = (a,b) => a + b;

// 1 + 2 + 3 + 4
console.log(array1.reduce(reducer));
// expected output: 10
```

```
   const totalYear = inventors.reduce((total, inventor) => {
        return total + (inventor.passed - inventor.year);
    });

```
