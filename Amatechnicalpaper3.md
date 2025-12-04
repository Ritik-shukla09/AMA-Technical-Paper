## 1. States of Promises in JS
- Pending
- Fulfilled (Resolved)
- Rejected

---

## 2. What is a Function Expression?
A function stored inside a variable.

Example:
const add = function(a, b) {
  return a + b;
};

---

## 3. What is Recursion?
A function that calls itself until a base case is reached.

Example:
function countdown(n) {
  if (n === 0) return;
  countdown(n - 1);
}

---

## 4. Common String Methods
- length
- toUpperCase()
- toLowerCase()
- slice()
- substring()
- includes()
- indexOf()
- trim()
- split()
- replace(), replaceAll()

---

## 5. Microtasks vs Macrotasks
### Microtasks
- Promise.then(), catch(), finally()
- queueMicrotask()
- Runs before macrotasks (higher priority)

### Macrotasks
- setTimeout
- setInterval
- DOM events
- Runs after all microtasks

---

## 6. var vs let vs const
### var
- Function-scoped
- Hoisted (initialized with undefined)
- Can redeclare

### let
- Block-scoped
- Hoisted but not initialized (TDZ)
- Cannot redeclare

### const
- Block-scoped
- Cannot reassign
- Objects/arrays can still mutate

**Best practice:**  
- Avoid var  
- Use let when value changes  
- Use const by default

---

## 7. What is Hoisting?
JavaScript moves declarations to the top before execution.

Hoisted:
- var (initialized as undefined)
- function declarations
- let & const (hoisted but in TDZ)

---

## 8. Difference Between == and ===
==  → compares value (performs type conversion)  
=== → compares value + type (strict)

Example:
"5" == 5  → true  
"5" === 5 → false  

---

## 9. Prototypal Inheritance
Objects inherit from other objects using the prototype chain.

Example:
const parent = { greet() { console.log("Hello"); } };
const child = Object.create(parent);
child.greet(); // inherited from parent

---

## 10. What Are Closures? (With Example)
A closure is when a function remembers variables from its outer scope even after the outer function has completed.

Example:
function counter() {
  let count = 0;
  return function() {
    count++;
    console.log(count);
  };
}

const c = counter();
c(); // 1
c(); // 2

---

## 11. Synchronous vs Asynchronous JavaScript
### Synchronous
- Executes line by line
- Blocks the thread

### Asynchronous
- Non-blocking
- Uses callbacks, promises, async/await

---

## 12. Arrow Functions vs Regular Functions
const add = (a, b) => a + b;

Differences:
- No own "this"
- No "arguments" object
- Cannot be used with "new"
- Shorter and cleaner syntax
