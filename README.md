# Drag-and-drop
This is a simple drag-and-drop project built with **HTML**, **CSS**, and **JavaScript**.  
It allows users to drag list items from one box (left) to another box (right) and vice versa.

---
## 🚀 Demo

### 🌐 Live demo: [click here](https://draganddrop01.netlify.app/)

#### or, 

### link: https://draganddrop01.netlify.app/

>
---

## 📸 Preview

![Digital Clock Preview](images/screenshots/Screenshot_4.png)


---


## 🧩 Features

- Drag and drop list items between two boxes  
- Smooth and responsive movement  
- Simple and clean code using vanilla JavaScript  
- Works on all modern browsers

---

## 🛠️ Technologies Used

- **HTML5** – For structure  
- **CSS3** – For styling  
- **JavaScript (ES6)** – For drag & drop functionality  

---

## 💡 How It Works

1. Each list item (`div.list`) has `draggable="true"`.  
2. When a drag starts, JavaScript stores the selected element.  
3. `e.preventDefault()` is used inside `dragover` events to allow dropping.  
4. On `drop`, the selected element is appended to the new box (`left` or `right`).

🧠 Learning Purpose

- This project is perfect for beginners who want to learn:

- Drag & Drop API in JavaScript

- DOM manipulation

- Event handling

## 📜 JavaScript Explanation

```js
rightBox.addEventListener('dragover', function(e) {
  e.preventDefault(); // Allows dropping in the right box
});

rightBox.addEventListener('drop', function(e) {
  rightBox.appendChild(selected);
  selected = null;
});

