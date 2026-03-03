CHAPTER 1 - BASICS-1

Ques 1. WHAT IS JAVASCRIPT ? WHAT IS THE USE JAVASCRIPT ENGINE ?
Answer -  Javascript is single threaded and synchronous language that is used for converting static web page to dynamic web page.
Javascript engines in various browsers that executes the javascript code.
Chrome - V8
Firefox - Spider Monkey
Safari - Javascript Chore 
Edge - chakra

Ques 2. WHAT ARE CLIENT AND SERVER SIDE ?
Answer - A client is a device or application that requests and consumes services provided by the server.
A server is a device or computer that provides services provided to clients.

Ques 3. WHAT ARE DIFFERENT TYPES OF VARIABLE ?
Answer - var - function scope , let and const are block scoped variable.

Ques 4. WHAT ARE DIFFERENT STRING METHODS ?
Answer -  let str1 = "Hello", str2 ="World"
          const newStr = str1.concat(str2)
          str1.indexOf(3)
          newStr.substring(6, 11)     // World
          newStr.length()
          newStr.split(" ")  //["Hello", "World"]
          newStr.replace("World", "Rohan")

Ques 5. WHAT IS DOM ? WHAT IS DIFFERENCE BETWEEN HTML AND DOM ?
Answer - static html -----> representation (MEMORY OF BROWSER) -----> DOM
The DOM represents the web page as a tree like structure that allows javascript to access and manipulate the elements.

Ques 6. WHAT ARE SELECTORS IN JAVASCRIPT ?
Answer - document.getElementById("div1")
         document.getElementsByClassName()
         document.querySelector()
         document.querySelectorAll()
         document.getElementsByTagName()

Ques 7. WHAT IS DIFFERENCE BETWEEN getElementsByClassName, getElementById, getElementsByTagName ?
Answer -  getElementByClassName - selects multiple elements with same class name 
          getElementsByTagName - selects multiple elements with same tag 
          getElementById - selects on basis of id
          htmlCollection - array like object but not completely array

           <div id="div1" class="myClass">1</div>
           <div class="myClass">2</div>
           <div class="myClass">3</div>

Ques 8. WHAT ARE TYPES OF DATA TYPES IN JAVASCRIPT ?
Answer - Primitive - nsbun (Number, String, boolean, undefined, null)
        Non-Primitive - oafdr (Object, Array, function, Regex, Date)

Ques 9. WHAT ARE DIFFERENT TYPES OF OPERATORS ?
Answer - Arithmetic, Assignment, Comparison, Logical, String

*************************************************************************************************

CHAPTER 2 - BASICS-2

Ques 1. WHAT IS A FUNCTION ? WHAT ARE TYPES OF FUNCTIONS ?
Answer - It is reusable block of code to perform a specific tasks
         Types of functions - 
         1. ARROW FUNCTIONS - also called fat arrow functions. simpler and shorter way of writing functions

Ques 2. WHAT IS AN OBJECT ?
Answer - allows you to store data in key-value pair.

Ques 3. WHAT IS SCOPE ?
Answer - Scope determines where the varibles are defined and where they can be accessed.

Ques 4. WHAT IS HOISTING ?
Answer - Hositing is a javascript behavior where functions and varible declarations moved at top during compilation phase

QUES 5. WHAT IS ASYNCHRONOUS PROGRAMMING ?
Answer - allows multiple tasks to run concurrently, by not blocking the other tasks

*************************************************************************************************

CHAPTER 3 - BASICS-3

Ques 1. WHAT IS SPREAD AND REST OPERATORS ?
Answer - Spread operator used to expand the elements from an iterable to individual elements.
         Used to copy array, merge array, passing multiple parameters to a function
         Rest opearator used in function parameters to collect the remaining araguments

*************************************************************************************************

CHAPTER 4 - BASICS-4

Ques 1. DIFFERENT METHODS OF ARRAY ?
Answer -  find - returns the first matching element of array
          filter - returns the array of elements that matches the conditions
          slice - this method returns the array of elements from start to end index(end element is not included)
          
Ques 2. DIFFERNCE BETWEEN PUSH AND CONCAT ?
Answer - push modifies the original array, whereas concate does not modifies the original array and creates a new array

Ques 3. WHAT IS SPLICE METHOD IN ARRAY ? 
Answer - used to add, remove and delete the elements
         array1.splice(startIndex, deleteCount, ...newItems)

Ques 4. WHAT IS DIFFERENCE BETWEEN FOREACH AND MAP ?
Answer - forEach is used to iterate over the array and perform some operation on each element, it does not modify the original array and does not return anaything.
map method modifies the original array and returns a new array with the modified elements.

Ques 5. WHAT IS ARRAY DESTRUCTURING ? 
Answer - allows you to unpack values from array into the individual elements

Ques 6. WHAT IS DIFFERENCE BETWEEN MAP AND WEAKMAP ?
Answer - Map allows you to store key-value pairs where keys can be of any type, including 

Ques 7. WHAT IS DIFFERENCE BETWEEN SET AND WEAKSET ?
Answer - Set is a collection of unique values where values can be any type, including primitive and object types. Weakset is a collection of unique values where values must be objects and are held weekly, meaning they can be garbage collected if ther are no other regerences to them

Ques 8. WHAT IS DIFFERENCE BETWEEN FOR IN AND FOR OF LOOP ?
Answer - for in loop used to iterate over the enumerable properties of object, including arrays and strings. for of loop used to iterate over the iterable objects like arrays, strings, maps etc.

Ques 9. WHAT IS DIFFERENCE BETWEEN NULL AND UNDEFINED ?
Answer - null represents the intentional absence of value, while undefined represents a varible that is declared but has not been assigned a value yet.

Ques 10. WHAT ARE ARRAY LIKE OBJECTS ?
Answer - Array like objects are the objects that are indexed and have the methods and functions used by the array but they do not have all methods like push and pop.
example- html collection, arguments, object, string etc.
sum(1,2,3)
function sum(){
        console.log(arguments[0])
}

Ques 11. HOW TO CONVERY ARRAY LIKE OBJECT TO ARRAY ?
Answer - 1. Array.from(arrayLikeObject)
        2. Using spread operator - [...arrayLikeObject]

Ques 12. FOR EACH VS FOR OF ?
Answer - use for of when need more control over loop and want to break or continue the loop, use for each when you want to iterate over array and perform some operation on each element without modifying original array and do not need break and continue

******************************************************************************************************

CHAPTER 5 - BASICS-5

Ques 1. WHAT IS FUNCTION EXPRESSION ?
Answer - assigning an anonymous function or a named function to a variable