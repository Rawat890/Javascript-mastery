🔢 Output-Based Questions (1–30)
1. What will be the output?
jsconsole.log(typeof null);
2. What will be the output?
jsconsole.log(0.1 + 0.2 === 0.3);
3. What will be the output?
jsconsole.log([] + []);
console.log([] + {});
console.log({} + []);
4. What will be the output?
jslet a = 1;
let b = a++;
console.log(a, b);
5. What will be the output?
jsconsole.log(1 == "1");
console.log(1 === "1");
6. What will be the output?
jsfor (var i = 0; i < 3; i++) {
  setTimeout(() => console.log(i), 0);
}
7. What will be the output?
jsfor (let i = 0; i < 3; i++) {
  setTimeout(() => console.log(i), 0);
}
8. What will be the output?
jsconsole.log(typeof undefined);
console.log(typeof NaN);
console.log(typeof function(){});
9. What will be the output?
jsconsole.log(null == undefined);
console.log(null === undefined);
10. What will be the output?
jsconst obj = { a: 1 };
const obj2 = obj;
obj2.a = 99;
console.log(obj.a);
11. What will be the output?
jsconsole.log("5" - 2);
console.log("5" + 2);
12. What will be the output?
jslet x = 10;
function foo() {
  console.log(x);
  let x = 20;
}
foo();
13. What will be the output?
jsconsole.log(false || "Hello" || true);
14. What will be the output?
jsconsole.log(!!null, !!0, !!"", !!undefined, !!NaN);
15. What will be the output?
jsconst arr = [1, 2, 3];
arr[10] = 99;
console.log(arr.length);
16. What will be the output?
jsfunction foo() {
  return
  {
    name: "JS"
  };
}
console.log(foo());
17. What will be the output?
jsconsole.log(typeof class {});
18. What will be the output?
jslet a = [1, 2, 3];
let b = [...a];
b.push(4);
console.log(a, b);
19. What will be the output?
jsconst p = new Promise((resolve) => {
  resolve(1);
  resolve(2);
});
p.then(console.log);
20. What will be the output?
jsconsole.log(+true);
console.log(+"");
console.log(+null);
console.log(+undefined);
21. What will be the output?
jsconst a = [1, 2, 3];
console.log(a.map(Number.isInteger));
22. What will be the output?
js(function() {
  var x = y = 10;
})();
console.log(typeof x);
console.log(y);
23. What will be the output?
jslet obj = { a: 1, b: 2, c: 3 };
let { a, ...rest } = obj;
console.log(rest);
24. What will be the output?
jsconsole.log([1, 2, 3].reduce((acc, val) => acc + val, 10));
25. What will be the output?
jsconst foo = () => arguments[0];
console.log(foo(1));
26. What will be the output?
jsconsole.log(3 > 2 > 1);
27. What will be the output?
jsasync function fetchData() {
  return 42;
}
const result = fetchData();
console.log(result);
28. What will be the output?
jslet a = { name: "Alice" };
let b = JSON.parse(JSON.stringify(a));
b.name = "Bob";
console.log(a.name);
29. What will be the output?
jsconsole.log(typeof (() => {}));
30. What will be the output?
jsconst nums = [1, [2, [3, [4]]]];
console.log(nums.flat(Infinity));

✍️ Write the Code Questions (31–70)
31. Write a function to deep clone an object without using JSON.parse/stringify.
32. Write an async function to fetch users from https://jsonplaceholder.typicode.com/users and filter those whose name starts with "L".
33. Create an async function to fetch user data and filter users whose dob is 11-02-2007.
34. Write a debounce function from scratch.
35. Write a throttle function from scratch.
36. Write a function to flatten a nested array without using .flat().
37. Write a custom implementation of Array.prototype.map.
38. Write a custom implementation of Array.prototype.filter.
39. Write a custom implementation of Array.prototype.reduce.
40. Write a Promise.all implementation from scratch.
41. Write a function that memoizes another function.
42. Write a function to curry any given function.
43. Write a function to compose multiple functions (right to left).
44. Write a function to pipe multiple functions (left to right).
45. Write a function to chunk an array into groups of n.
jschunk([1,2,3,4,5], 2) // [[1,2],[3,4],[5]]
46. Write a function to remove duplicates from an array using a Set.
47. Write a function to group an array of objects by a given key.
jsgroupBy([{type:'fruit', name:'apple'}, {type:'veggie', name:'carrot'}], 'type')
48. Write a custom bind function without using Function.prototype.bind.
49. Write a function to deep compare two objects.
50. Create a linked list in JavaScript with insert and print methods.
51. Write a function to find the longest word in a string.
52. Write a function to check if a string is a palindrome.
53. Write a function to count the frequency of characters in a string.
54. Write a function to flatten a nested object.
js{ a: { b: { c: 1 } } } // → { 'a.b.c': 1 }
55. Write a function that retries a failed promise up to n times.
56. Implement a rate limiter — allow only n function calls per second.
57. Write a binary search function.
58. Write a function to sort an array of objects by multiple fields.
59. Implement an event emitter (on, emit, off) from scratch.
60. Write a stack and queue using arrays in JavaScript.
61. Write a function to find all anagrams in an array of strings.
62. Write a function that returns a new object with only the specified keys.
jspick({ a:1, b:2, c:3 }, ['a','c']) // { a:1, c:3 }
63. Write a function to convert a flat array to a tree structure.
64. Write a function that delays execution by n milliseconds using a Promise.
65. Write an observer pattern in JavaScript.
66. Write a function that takes a URL and query params object and returns a full URL string.
67. Write a function to capitalize the first letter of every word in a sentence.
68. Implement Promise.race from scratch.
69. Write a function to find the second largest number in an array.
70. Write a function that parses a JWT token and returns the payload (without a library).

🧠 Conceptual / Tricky Questions (71–100)
71. What is the difference between == and ===? Give examples where == causes unexpected results.
72. Explain hoisting in JavaScript. How does it differ for var, let, const, and functions?
73. What is a closure? Give a real-world use case.
74. What is the difference between call, apply, and bind?
75. What is the event loop? How do the call stack, microtask queue, and macrotask queue interact?
76. What is the difference between microtasks and macrotasks? Give examples of each.
77. What is prototypal inheritance? How does it differ from classical inheritance?
78. What is the difference between __proto__ and prototype?
79. What is this in JavaScript? How does its value differ in arrow functions vs regular functions?
80. What is the difference between shallow copy and deep copy? Which methods produce each?
81. Explain Promise chaining. What happens if you forget to return inside a .then()?
82. What is async/await? How does it relate to Promises under the hood?
83. What is the difference between null, undefined, and undeclared?
84. What is a generator function? What is yield and when would you use generators?
85. Explain the difference between for...in and for...of.
86. What are WeakMap and WeakSet? How do they differ from Map and Set?
87. What is temporal dead zone (TDZ)?
88. What is the difference between function declarations and function expressions? How does hoisting affect each?
89. What is optional chaining (?.) and nullish coalescing (??)? How do they differ from ||?
90. What is garbage collection in JavaScript? What is a memory leak and how can closures cause one?
91. What is the difference between Object.freeze() and const?
92. What are Proxy and Reflect in JavaScript? Give a practical use case.
93. What is symbol in JavaScript and why is it useful?
94. Explain IIFE (Immediately Invoked Function Expression) and its common use cases.
95. What is the difference between Array.isArray() and instanceof Array? Which is more reliable and why?
96. What is tree shaking in JavaScript bundlers? Why does it matter?
97. What are tagged template literals? Write an example.
98. Explain the concept of immutability in JavaScript. How can you enforce it?
99. What is the difference between concurrency and parallelism in the context of JavaScript?
100. You have three async API calls — A, B, and C — where C depends on the result of B, and B depends on the result of A. Write the code using Promises and then rewrite it using async/await. Which is more readable and why?
