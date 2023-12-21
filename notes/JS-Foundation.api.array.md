---
id: 82vl0fa7hym6d2o4k8jl0r4
title: Array Methods
desc: ""
updated: 1703161931078
created: 1702882547716
---

#### Push/Pop

```js
const arr = [1, 2, 3];
arr.push(4); // arr: [1,2,3,4]

const arr2 = [1, 2, 3];
arr2.pop(2); // arr: [1,2] position
```

#### Shift/Unshift

```js
const arr = [1, 2, 3];
arr.shift(); // arr: [2,3] removes front

const arr2 = [1, 2, 3];
arr2.unshift(5); // arr: [5,1,2,3] puts at front
```

#### Concatenation

```js
const arr1 = [1, 2, 3];
const arr2 = [4, 5, 6];
const ans = arr1.concat(arr2);
//ans : [1,2,3,4,5,6]
```

- `concat` is different from `push` as its second argument is an array

### Special (Callback) Methods:

#### forEach

we give forEach an array and for every element of that array, it runs the function given in arguments.

```js
const items = ["item1", "item2", "item3"];
const copyItems = [];

items.forEach((item) => {
  copyItems.push(item);
});

// Will work same as:

for (let i = 0; i < items.length; i++) {
  copyItems.push(items[i]);
}
```

#### Map

Calls a given function on each element of the passes array.

```js
const array1 = [1, 4, 9, 16];

// Pass a function to map
const map1 = array1.map((x) => x * 2);

console.log(map1);
// Output: [2, 8, 16, 32]
```

#### Filter

- The `filter()` method creates a new array filled with elements that pass a test provided by a function.

- Does not execute the function for empty elements.

- The filter() method does not change the original array.

```js
const array1 = [1, 4, 9, 16];

// only keeps the elemets that pass th check
const filtered_arr = array1.filter((num) => num % 2 == 0);

console.log(filtered_arr);
// Output: [4, 16]
```
