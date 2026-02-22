
## Answers to Questions

### 1. What is the difference between getElementById, getElementsByClassName, and querySelector / querySelectorAll?

getElementById: Selects a single element using its unique ID.

getElementsByClassName: Selects all elements with a specific Class. It returns an HTMLCollection (array-like list).

querySelector: Selects the first element that matches a CSS Selector (ID, Class, or Tag).

querySelectorAll: Selects all elements that match a CSS Selector. It returns a NodeList.



### 2. How do you create and insert a new element into the DOM?

 1. Create the element
const newDiv = document.createElement('div');

 2. Add some text
newDiv.innerText = "Hello World!";

 3. Insert it into the body
document.body.appendChild(newDiv);

### 3. What is Event Bubbling? And how does it work?

Trigger: The event starts at the target element (the exact thing you clicked).

Propagation: The event automatically moves up to the parent element.

Finish: It continues moving up through the DOM tree until it hits the window object.

### 4. What is Event Delegation in JavaScript? Why is it useful?

Event Delegation is a design pattern in JavaScript used to handle events efficiently. Instead of adding an event listener to every single child element, you add a single event listener to a common parent element.

### 5. What is the difference between preventDefault() and stopPropagation() methods?

preventDefault() stops the browser’s default action of an element.
For example, it stops a form from submitting or a link from opening.

stopPropagation() stops the event from moving to parent elements.
It prevents event bubbling.

Main Difference:
preventDefault() : Stops the browser’s default behavior.
stopPropagation() : Stops the event from bubbling to parent elements.
