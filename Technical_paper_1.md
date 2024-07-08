
## 1. What is the difference between (==) and (===) operator?

- The == operator compares the values of two variables after performing type conversion if necessary. On the other hand, the === operator compares the  values of two variables without performing type conversion.

## 2. Console.log(typeof []) is equal to 'object' why?

- typeof [] is an object in javascript because it internally stores indices as keys and supports object methods also.

## 3. What are the disadvantages of using closure?

- The disadvantage of closure is that the garbage collector cannot remove the space allocated by the closure variable.

## 4. Why using global variables is bad in JS?

- Global variables can be modified from anywhere in the code, making it difficult to track changes.

## 5. How to extract certain properties from an array of objects to create a new array?

- The `reduce()` method can be used to extract a property into an array by accumulating values in an initial array. 

## 6. Difference between the charAt() and at() methods in js?

- The at() allows negative indexes while charAt() do not. Now you can use myString.at(-2) instead of charAt(myString.length-2) 

## 7. How to reset the initial or 1st commit in git, if it's possible?

- It is not possible to revert the first commit instead we can create a new branch make changes and commit and delete the old one.

## 8. If console.log(typeof []) returns 'object', then why can not we use the (.) operator in the array to access its values just like objects, where we use the (.) operator in objects for accessing keys and values?

- There are certain differences between the arrays and objects and the main difference is array key is numerical indices and the object keys are in the string form.

## 9. Why 'forEach' loop skip 'not defined' whereas the 'for' loop gives 'undefined'?

- for loops traverse by indexes so when the element is absent then it will be treated as undefined and for loops traverse from element to element so it does not take care of the absent element.

## 10. How can we mimic the action Array? splice and 'Array. slice' on objects?

- mimicing the method for the object may requires to create the custom functions and return it explicitly.

## 11. What is the "Callback Hell" problem and how to avoid it?

- callback hell is a situation where one callback function calls another callback and so on. To avoid this we can use promises.

## 12. Question:-

   let ar = [1,2,3];
console.log("Hello");
module. exports.ar = ar;

// file2.js
const {ar} = require('file1.js');
let print = ar;
console.log(print);

Output: "Hello"
        [1,2,3]

- why "Hello" is also printed? when we have exported array('ar') only?

## Explanation:-

- when we export any module the execution of the module happens regardless of what we imported so all the statements got executed. We may limit this behavior by making a function and making a call when needed.
