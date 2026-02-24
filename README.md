1. What is the difference between getElementById, getElementsByClassName, and querySelector / querySelectorAll?

Answer: 
getElementById is used to get a single element by its unique id. It returns only one element.
getElementsByClassName is used to get elements by class name. It returns a collecttion of elements.
querySelector is used to select the first element that matches a CSS selector like id, class, or tag. It returns only one element.
querySelectorAll is used to select all elements that match a CSS selector. It returns a NodeList.

2. How do you create and insert a new element into the DOM?

Answer:
Create a new element, set its content, and attach it to a parent.
Example:
<script>
  const h1 = document.createElement('h1'); 
  h1.textContent = "Hello World"; 
  document.getElementById('container').appendChild(h1); 
</script>

3. What is Event Bubbling? And how does it work?

Answer:
Event bubbling is a process where an event starts from the target element and then moves upward to its parent elements.
When we click an element, the event first happens on that element, then it goes to its parent, then the parents parent, and continues up to the top of the page.

5. What is Event Delegation in JavaScript? Why is it useful?

Answer:
Event delegation is a technique where we add an event listener to a parent element instead of adding it to many child elements.
It is useful because It saves time and keeps our code clean and it improves performance.

6. What is the difference between preventDefault() and stopPropagation() methods?

Answer:
preventDefault() is used to stop the default behavior of an element. It can stop a form from submitting or a link from opening.
stopPropagation() is used to stop the event from bubbling to parent elements.
