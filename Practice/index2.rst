!

🔢 Output-Based Questions (1–35)
1. What will be the output?
jsconsole.log(1 + "2" + 3);
console.log(1 + 2 + "3");
2. What will be the output?
jsconst obj = {};
obj.a = 1;
Object.freeze(obj);
obj.a = 99;
console.log(obj.a);
3. What will be the output?
jsconsole.log([1,2,3] == [1,2,3]);
console.log([1,2,3] === [1,2,3]);
4. What will be the output?
jslet a = 5;
console.log(a++, ++a);
5. What will be the output?
jssetTimeout(() => console.log("timeout"), 0);
Promise.resolve().then(() => console.log("promise"));
console.log("sync");
6. What will be the output?
jsfunction outer() {
  let count = 0;
  return function inner() {
    count++;
    console.log(count);
  };
}
const fn = outer();
fn();
fn();
fn();
7. What will be the output?
jsconst arr = [1, 2, 3];
const [first, , last] = arr;
console.log(first, last);
8. What will be the output?
jsconsole.log(typeof NaN === "number");
console.log(NaN === NaN);
console.log(Number.isNaN(NaN));
9. What will be the output?
jsclass Animal {
  constructor(name) { this.name = name; }
  speak() { return `${this.name} makes a sound.`; }
}
class Dog extends Animal {
  speak() { return `${this.name} barks.`; }
}
const d = new Dog("Rex");
console.log(d.speak());
console.log(d instanceof Animal);
10. What will be the output?
jsconst promise = new Promise((resolve, reject) => {
  reject("error");
  resolve("success");
});
promise
  .then(val => console.log("Resolved:", val))
  .catch(err => console.log("Caught:", err));
11. What will be the output?
jslet x = 1;
const obj = {
  x: 2,
  getX: function() { return this.x; },
  getXArrow: () => x
};
console.log(obj.getX());
console.log(obj.getXArrow());
12. What will be the output?
jsfunction* gen() {
  yield 1;
  yield 2;
  yield 3;
}
const g = gen();
console.log(g.next());
console.log(g.next());
console.log(g.next());
console.log(g.next());
13. What will be the output?
jsconst map = new Map();
map.set("a", 1);
map.set("b", 2);
map.set("a", 99);
console.log(map.size);
console.log(map.get("a"));
14. What will be the output?
jsconsole.log([] == false);
console.log([] == 0);
console.log([] == "");
15. What will be the output?
jsasync function foo() {
  console.log("A");
  await Promise.resolve();
  console.log("B");
}
console.log("C");
foo();
console.log("D");
16. What will be the output?
jslet obj = { a: 1, b: 2 };
let copy = Object.assign({}, obj);
copy.a = 99;
console.log(obj.a);
17. What will be the output?
jsconst sym1 = Symbol("id");
const sym2 = Symbol("id");
console.log(sym1 === sym2);
console.log(typeof sym1);
18. What will be the output?
jsfunction foo(a, b = 5, c) {
  console.log(a, b, c);
}
foo(1, undefined, 3);
19. What will be the output?
jsconst obj = {
  name: "Alice",
  greet() {
    const inner = () => console.log(this.name);
    inner();
  }
};
obj.greet();
20. What will be the output?
jsconsole.log(Object.keys({ a: 1, b: 2, c: 3 }));
console.log(Object.values({ a: 1, b: 2, c: 3 }));
console.log(Object.entries({ a: 1, b: 2, c: 3 }));
21. What will be the output?
jstry {
  null.name;
} catch(e) {
  console.log(e instanceof TypeError);
  console.log(e.message);
}
22. What will be the output?
jslet a = [1, 2, 3];
let b = a;
a = [4, 5, 6];
console.log(b);
23. What will be the output?
jsconst fn = (function() {
  let x = 10;
  return {
    getX: () => x,
    setX: (val) => { x = val; }
  };
})();
console.log(fn.getX());
fn.setX(99);
console.log(fn.getX());
24. What will be the output?
jsconsole.log("start");
async function main() {
  const result = await new Promise(resolve => {
    setTimeout(() => resolve("done"), 1000);
  });
  console.log(result);
}
main();
console.log("end");
25. What will be the output?
jsconst a = [1, 2, 3];
const b = [4, 5, 6];
const c = [...a, ...b];
console.log(c);
26. What will be the output?
jsfunction test() {
  console.log(a);
  console.log(b);
  var a = 1;
  let b = 2;
}
test();
27. What will be the output?
jsconst double = x => x * 2;
const square = x => x ** 2;
const result = [1, 2, 3].map(double).map(square);
console.log(result);
28. What will be the output?
jsconsole.log(+"3.14");
console.log(+false);
console.log(+true);
console.log(+[]);
console.log(+{});
29. What will be the output?
jslet obj = { x: 10 };
let { x: renamed } = obj;
console.log(renamed);
console.log(typeof x);
30. What will be the output?
jsconst arr = [3, 1, 4, 1, 5, 9];
console.log(arr.sort());
console.log([10, 9, 2, 1, 100].sort());
31. What will be the output?
jsclass Counter {
  #count = 0;
  increment() { this.#count++; }
  get value() { return this.#count; }
}
const c = new Counter();
c.increment();
c.increment();
console.log(c.value);
console.log(c.#count);
32. What will be the output?
jsconst p1 = Promise.resolve(1);
const p2 = Promise.resolve(2);
const p3 = Promise.reject("error");

Promise.allSettled([p1, p2, p3]).then(console.log);
33. What will be the output?
jsconst handler = {
  get(target, key) {
    return key in target ? target[key] : `Property "${key}" not found`;
  }
};
const obj = new Proxy({ name: "Alice" }, handler);
console.log(obj.name);
console.log(obj.age);
34. What will be the output?
jsfunction foo(...args) {
  console.log(args);
  console.log(arguments[0]);
}
foo(1, 2, 3);
35. What will be the output?
jsconst nums = [1, 2, 3, 4, 5];
const result = nums.reduceRight((acc, val) => acc + val, 0);
console.log(result);

✍️ Write the Code Questions (36–75)
36. Write an async function to fetch posts from https://jsonplaceholder.typicode.com/posts and return only posts where userId is 1.
37. Write a function to sequentially execute an array of promises (one after the other, not in parallel).
38. Write a custom Promise.allSettled from scratch.
39. Write a function that converts a callback-based function to a Promise-based one (promisify).
40. Write a LRU Cache (Least Recently Used) with get and put methods.
41. Write a function that polls an API every 2 seconds until it returns a successful result, then stops.
42. Write a function to find all permutations of a string.
43. Write a trie data structure with insert and search methods.
44. Write a function to serialize and deserialize a binary tree.
45. Write a function to find the most frequent element in an array.
46. Implement Function.prototype.curry that supports partial application.
47. Write a function to convert a number to Roman numerals.
48. Write a function to parse a query string into an object.
jsparseQuery("?name=Alice&age=25") // { name: 'Alice', age: '25' }
49. Write a function to convert an object to a query string.
jstoQuery({ name: 'Alice', age: 25 }) // "name=Alice&age=25"
50. Write a function that finds the longest common prefix among an array of strings.
51. Write a function to validate an email address using regex.
52. Write a function to validate a password (min 8 chars, 1 uppercase, 1 number, 1 special char).
53. Write a publish-subscribe (PubSub) system from scratch.
54. Write a function to perform deep merge of two objects.
55. Implement a queue using two stacks.
56. Write a function that implements lazy evaluation — the function only computes the value when it's needed.
57. Write a function to find all subsets (power set) of an array.
58. Write a function that limits concurrent async operations to n at a time.
59. Write a function to implement virtual DOM diffing (simple version — compare two objects and return the diff).
60. Write a countdown timer using setInterval that logs from 10 to 0 and then stops.
61. Write a function to zip two arrays together.
jszip([1,2,3], ['a','b','c']) // [[1,'a'],[2,'b'],[3,'c']]
62. Write a function to find duplicate values in an array.
63. Write a function to implement matrix multiplication.
64. Write a function to sum all nested values in a deeply nested object.
65. Write a middleware pipeline function similar to Express.js next().
66. Write a function to detect a cycle in a linked list.
67. Write a function to rotate an array by k positions.
jsrotate([1,2,3,4,5], 2) // [4,5,1,2,3]
68. Write a function to find the intersection of two arrays.
69. Write a function to generate a UUID (v4) without any library.
70. Write a function that recursively builds a breadcrumb path from a nested menu structure.
71. Write a function to implement infinite scrolling logic — given a page number and page size, return the correct slice of data.
72. Write a function to auto-retry a fetch request with exponential backoff.
73. Write a function to detect if two objects have circular references.
74. Write a token bucket algorithm for rate limiting.
75. Write a function that accepts a nested array of tasks (some async, some sync) and executes them in order.

🧠 Conceptual / Tricky Questions (76–100)
76. What is the difference between Object.create(null) and {}? When would you use Object.create(null)?
77. What are iterators and iterables in JavaScript? How do you make a custom iterable object?
78. What is function composition vs currying? How are they different and when would you use each?
79. Explain the difference between Promise.all, Promise.allSettled, Promise.race, and Promise.any. Give a use case for each.
80. What is a memory leak in JavaScript? Name 5 common causes and how to prevent each.
81. What is the difference between imperative and declarative programming? How does JavaScript support both?
82. What is structural sharing and how does it relate to immutability in JavaScript?
83. What is the difference between a pure function and an impure function? Why does it matter?
84. Explain lazy loading in JavaScript. How can you implement it for modules and images?
85. What is coercion in JavaScript? Explain implicit vs explicit coercion with examples.
86. What is the difference between Object.keys(), Object.getOwnPropertyNames(), and Reflect.ownKeys()?
87. What are design patterns? Explain the Singleton, Factory, and Module patterns with JavaScript examples.
88. What is the Revealing Module Pattern and how does it differ from the regular Module Pattern?
89. What is tail call optimization (TCO)? Does JavaScript support it? How can you simulate it?
90. What is the difference between new.target and checking instanceof inside a constructor?
91. Explain accessor properties (get/set) vs data properties in JavaScript objects using Object.defineProperty.
92. What is duck typing in JavaScript? How does it relate to TypeScript's structural typing?
93. What is the difference between eval() and new Function()? Why are both considered dangerous?
94. Explain the concept of "functor" in JavaScript. How is Array.prototype.map an example of a functor?
95. What is referential transparency and how does it relate to pure functions in JavaScript?
96. What is the difference between error types in JavaScript — TypeError, ReferenceError, SyntaxError, RangeError? Give an example that triggers each.
97. What are AbortController and AbortSignal? How do you use them to cancel a fetch request?
98. What is the Structured Clone Algorithm? How does it differ from JSON.parse(JSON.stringify(...)) for deep cloning?
99. Explain requestAnimationFrame vs setTimeout. When should you use one over the other for animations?
100. You're building a real-time collaborative document editor. Users type simultaneously and changes must sync across clients. Explain the core JavaScript concepts you'd use (WebSockets, event queues, operational transforms or CRDTs, debouncing) and how they fit together.
