# Program, Programming, and Programmer

## 1. Program

A **program** is a set of instructions written in a specific language that tells a computer how to perform a task. It can range from simple scripts to complex applications and operating systems.

- **Example**: A calculator app or a web browser like Google Chrome is a program.

## 2. Programming

**Programming** is the process of writing, designing, testing, and maintaining the code (instructions) that make up a program. It involves using programming languages like Python, JavaScript, or C++ to create software that solves a problem or performs a specific task.

- **Example**: Writing code to create a website or to automate repetitive tasks in an organization.

## 3. Programmer

A **programmer** is an individual who writes and develops programs using programming languages. They use logic, problem-solving skills, and creativity to build and maintain software, whether for web development, mobile apps, video games, or data analysis.

- **Example**: A person who writes code for creating an e-commerce website is a programmer.

---

These concepts are interconnected, with the **programmer** being the person who engages in **programming** to create a **program**.

# Types of Web Pages

## 1. Static Web Pages

A **static web page** is one whose content does not change with time. These web pages do not need to be interactive and are often used to display static information such as:

- Company name
- Goals
- Mission and vision
- Address

The content of static web pages remains the same for all users over time.

## 2. Dynamic Web Pages

A **dynamic web page** is one that is constantly updated. These web pages interact with servers, and their content changes based on data sent by the servers. Dynamic web pages are useful for displaying information that changes over time or for different users.

- **Example**: A news website that updates continuously with the latest news.

## Website Overview

A **website** is a collection of interlinked web pages, which can be either static or dynamic.

A website is built using three key components:

- **HTML**: Defines the structure and content of the page.
- **CSS**: Adds styling to make the web page visually appealing.
- **JavaScript**: Provides interactivity and dynamic behavior to the web page.

---

# How JavaScript Works

JavaScript is a single-threaded, interpreted programming language that runs in the browser's **JavaScript engine** (like V8 in Chrome or SpiderMonkey in Firefox). JavaScript can perform both **synchronous** and **asynchronous** operations. Here's how it works step by step:

### 1. **Execution Context**

- Every time a JavaScript file is loaded or a script is executed, an **Execution Context** is created. The global scope (usually the browser window) is called the **Global Execution Context**, where all code is first run.
- Inside this execution context, there are two phases:
  1.  **Creation Phase**:
      - The JavaScript engine scans the code and allocates memory for variables and functions.
      - Variables are initialized with `undefined`, and functions are fully stored.
  2.  **Execution Phase**:
      - The code is executed line by line, and variables are assigned actual values.

### 2. **Call Stack**

- JavaScript uses a **call stack** to keep track of function calls. Every time a function is called, a new execution context is added to the stack. When the function completes, it is removed from the stack.
- This **stack** structure ensures that the last function called is the first to finish execution (LIFO – Last In, First Out).

### 3. **Memory Heap**

- JavaScript manages data in a **memory heap**, where objects and variables are stored.
- **Garbage collection** automatically frees up memory that's no longer needed, ensuring memory-efficient performance.

### 4. **Single Threaded and Non-blocking**

- JavaScript is **single-threaded**, meaning it can only execute one task at a time. However, it is **non-blocking**, thanks to asynchronous features like `setTimeout()`, `Promises`, and `async/await`.
- The event loop (explained below) allows JavaScript to handle multiple tasks without blocking the main thread.

### 5. **Event Loop**

- The **event loop** enables asynchronous execution in JavaScript by checking the **call stack** and the **callback queue**.
- When asynchronous tasks (like fetching data, timers, or event listeners) are completed, their callbacks are pushed to the **callback queue**. The event loop constantly checks the call stack and processes callbacks once the stack is empty.

### 6. **Asynchronous Operations**

- **Promises** and `async/await` are used to handle asynchronous tasks like network requests.
  - **Promises** represent future values and allow chaining actions once a task completes (`.then()` and `.catch()`).
  - **async/await** simplifies working with promises, allowing the code to wait for a task to finish before continuing.

---

# Workflow of JavaScript on the Browser

When JavaScript is executed in the browser, the following steps occur:

### 1. **Loading the Web Page**

- The browser fetches the HTML, CSS, and JavaScript files.
- The HTML is parsed to build the **DOM (Document Object Model)**, and the CSS is applied to style the page.

### 2. **JavaScript Execution**

- JavaScript execution begins after the HTML is parsed and the **DOM** is partially or fully constructed, depending on where the script is located (either in the `<head>` or at the bottom of the `<body>` tag).
- If the script is at the bottom, the page content will load first before executing JavaScript. If in the `<head>`, the script might block the page rendering until the JavaScript is loaded and executed.

### 3. **Execution Context**

- JavaScript runs inside the **JavaScript Engine** provided by the browser (e.g., V8 engine in Chrome, SpiderMonkey in Firefox).
- The browser creates a **Global Execution Context**, where the JavaScript code runs. Every function call creates a **new execution context** that is placed on the **call stack**.

### 4. **Interaction with the DOM**

- JavaScript can access and modify the **DOM** using methods like `document.getElementById()` or `querySelector()`.
- It can manipulate HTML content, attributes, and styles dynamically.

### 5. **Event Loop and Asynchronous Code**

- JavaScript uses an **event-driven** model. Asynchronous operations such as network requests (AJAX), timeouts, and event listeners do not block the main thread.
- The **event loop** checks if there are any events or callbacks (like `setTimeout()` or `fetch()` responses) in the **callback queue** to be executed after the main code execution is completed.

### 6. **Rendering Updates**

- After JavaScript modifies the DOM or CSS, the browser re-renders the affected parts of the web page to reflect those changes.

### 7. **Handling User Interactions**

- JavaScript listens for user interactions such as clicks, form submissions, and keyboard events through **event listeners**.
- These events trigger JavaScript functions to respond dynamically, updating the web page without needing to reload.

---

This workflow explains how JavaScript operates inside the browser and enables interactivity, real-time updates, and dynamic content rendering.
This version includes a section that explains how JavaScript works internally, covering key concepts

# JavaScript Functions Overview

## 1. `alert()`

The `alert()` function opens a dialog box displaying the value that you have passed to the function. This is commonly used to show messages or notifications to the user.

### Example:

```
alert("Hello, World!");
```
