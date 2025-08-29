## 📌 1. What’s the difference between **getElementById**, **getElementsByClassName**, and **querySelector/querySelectorAll?**

✅ **getElementById**
- Finds one single element by its unique ID. It gives you that element or nothing if it’s not there.

✅ **getElementsByClassName**
- Finds all elements that have a certain class. It returns a live list that updates if the page changes.

✅ **querySelector**
- Finds the first element that matches any CSS selector you give it (like a class, ID, or tag).

✅ **querySelectorAll**
- Finds all elements matching a CSS selector, but the list doesn’t update if the page changes.

---
## 📌 2. How do you create and add a new element to the page?

First, I will make a new element with document.createElement(). Then I will add it somewhere on the page using methods like appendChild().

✅ **Example**


const newDiv = document.createElement('div');

newDiv.textContent = 'Hello!';

document.body.appendChild(newDiv);

---

## 📌 3. What is Event Bubbling and how does it work?

Imagine I click on a button inside a box inside a bigger container. The click event happens on the button first, then “bubbles up” to the box, then the container, and all the way up the page.

So, events start at the deepest element and move up through the parents.

---
## 📌 4. What is Event Delegation and why is it useful?

Instead of putting the same event listener on lots of child elements, I will put one listener on a parent element. Then, inside that listener, I will check which child actually got clicked.

This saves me from adding tons of listeners and works even if I add new child elements later on.

---

## 📌 5. What’s the difference between preventDefault() and stopPropagation()?

✅ **preventDefault()** 
- stops the browser’s normal behavior. For example, it stops a link from opening a new page.

✅ **stopPropagation()** 
- stops the event from moving up the chain (bubbling). So, parent elements won’t hear about the event.
---