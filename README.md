# Slice-and-Splice-
In JavaScript, slice() and splice() are two array methods that perform different operations on arrays.

1) Slice()
   
The slice() method returns a shallow copy of a portion of an array into a new array. It takes two parameters: the starting index (inclusive) and the ending index (exclusive). The original array is not modified.

const fruits = ['apple', 'banana', 'cherry', 'date', 'elderberry'];

// Slice from index 1 to 3 (exclusive)
const slicedFruits = fruits.slice(1, 3);

console.log(slicedFruits); // Output: ['banana', 'cherry']
console.log(fruits); // Original array is unchanged

In this example, slice(1, 3) returns a new array containing elements from index 1 to 2 (exclusive) of the original array.

2) Splice()

The splice() method, on the other hand, is used to change the contents of an array by removing or replacing existing elements and/or adding new elements. It takes three parameters: the starting index, the number of elements to remove, and optional elements to add.

const fruits = ['apple', 'banana', 'cherry', 'date', 'elderberry'];

// Remove 2 elements starting from index 1 and add 'orange' and 'grape'
const removedFruits = fruits.splice(1, 2, 'orange', 'grape');

console.log(removedFruits); // Output: ['banana', 'cherry']
console.log(fruits); // Output: ['apple', 'orange', 'grape', 'date', 'elderberry']

In this example, splice(1, 2, 'orange', 'grape') removes two elements starting from index 1 ('banana' and 'cherry') and adds 'orange' and 'grape' in their place.

To summarize:

i) slice() returns a new array with selected elements from the original array without modifying the original array.
ii) splice() modifies the original array by removing, replacing, or adding elements.
