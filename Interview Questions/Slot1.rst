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


CHAPTER 2 - BASICS-2

Ques 1. What