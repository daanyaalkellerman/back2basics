# JavaScript: Back to Basics

A hands-on refresher for getting comfortable with JavaScript again. Work at your own pace. There are no solutions or answer keys in this workbook.

## How to Practice

- Create a file such as `practice.js` in this folder for your attempts.
- Run it with `node javascript/practice.js` from the project root if Node.js is installed, or try individual snippets in your browser's developer console.
- Answer the questions in your own words before looking anything up.
- For prediction questions, write your prediction before running the code.
- Starter code is intentionally unfinished. Replace each TODO with your own code.
- Test more than one input. When something fails, explain why before changing it.

## 1. Variables and Data Types

### Quick Questions

1. What is the difference between `let` and `const`?
2. When might you choose `let` for a variable?
3. How do a number and a string containing digits differ?
4. What are booleans useful for?
5. What is the difference between `undefined` and `null`?

### Predict Before Running

```js
let score = 5;
const bonus = 3;
score = score + bonus;

console.log(score);
console.log(typeof score);
console.log(typeof "5");
```

Write down each output and explain your reasoning.

### Coding Task: Introduce Yourself

Declare variables for your name, your age, and whether you are learning JavaScript. Pick suitable declaration keywords and data types.

```js
// TODO: Declare your three variables.

// TODO: Log each value and its type.

// TODO: Use a template literal to print a sentence about yourself.
```

- [ ] I can explain my choice of `let` or `const` for each variable.

## 2. Operators and Converting Values

### Quick Questions

1. What does the remainder operator `%` do?
2. How do `==` and `===` differ?
3. What can happen when you use `+` with a string and a number?
4. What is `NaN`, and when might you encounter it?

### Predict Before Running

```js
console.log("12" + 4);
console.log("12" - 4);
console.log(17 % 5);
console.log(7 === "7");
console.log(Number("hello"));
```

### Coding Task: Shopping Total

Calculate the subtotal for several identical items, the discount amount, and the final total. Treat `discountPercent` as a percentage of the subtotal. Ignore tax and delivery costs.

```js
const priceText = "45";
const quantity = 3;
const discountPercent = 10;

// TODO: Convert priceText to a number.
// TODO: Calculate the subtotal.
// TODO: Calculate the discount amount and final total.
// TODO: Log a labelled summary of your calculations.
```

Try a quantity of `1` and a discount of `0` as well. Work out the expected totals yourself before checking your code.

- [ ] My calculations use numbers, not accidental string concatenation.

## 3. Strings

### Quick Questions

1. How do you find the length of a string?
2. What index refers to its first character?
3. What is a template literal?
4. Does calling a string method change the original string?

### Coding Task: Clean Up a Username

```js
const rawUsername = "  JavaScriptLearner  ";

// TODO: Remove spaces from the beginning and end.
// TODO: Store a lowercase version of the cleaned username.
// TODO: Log its length and first character.
// TODO: Check whether it contains "script".
```

Repeat with your own username and a string containing only spaces. Think about what the first character means for an empty string.

- [ ] I can explain which operations return strings and which return other types.

## 4. Conditions and Logical Operators

### Quick Questions

1. When would you use `else if`?
2. What do `&&`, `||`, and `!` mean?
3. What does it mean for a value to be truthy or falsy?
4. Why does the order of conditions matter?

### Coding Task: Ticket Price

Use these practice rules:

- Under 5: free entry.
- Ages 5 through 17: R40.
- Ages 18 through 59: R80.
- Ages 60 and above: R50.
- A negative age: print an invalid-age message instead of a price.

Assume `age` is a number.

```js
const age = 17;

// TODO: Use conditions to print the correct price or message.
```

Test `-1`, `0`, `4`, `5`, `17`, `18`, `59`, and `60`. Make your own expected-results list first.

### Extra Task: Access Check

```js
const hasAccount = true;
const isBlocked = false;

// TODO: Print "Access granted" only when the person has an account
// and is not blocked. Otherwise, print "Access denied".
```

- [ ] I have tested every ticket-price boundary and all four combinations of the two booleans.

## 5. Loops

### Quick Questions

1. What are the three parts of a typical `for` loop?
2. When would a `while` loop be useful?
3. What causes an infinite loop?
4. How do `break` and `continue` differ?

### Coding Task: Count and Add

```js
const limit = 10;

// TODO: Print every whole number from 1 through limit.
// TODO: In a separate loop, print only the even numbers in that range.
// TODO: Calculate and print the sum of all numbers from 1 through limit.
```

Try `limit` values of `1`, `2`, and `10`.

### Coding Task: Countdown

Use a `while` loop to count down from `5` to `1`, then print `Go!` once.

```js
let countdown = 5;

// TODO: Write your countdown.
```

- [ ] I can explain why each loop stops.

## 6. Functions and Scope

### Quick Questions

1. What is the difference between a parameter and an argument?
2. How does `return` differ from `console.log()`?
3. What does a function return if it has no return statement?
4. Can you use a variable declared inside a function from outside it?
5. What does block scope mean for `let` and `const`?

### Coding Task: Small Helpers

Complete each function. They should return their results; log the results where you call them.

```js
function greet(name) {
  // TODO: Return a greeting that includes name.
}

function isEven(number) {
  // TODO: Return a boolean indicating whether number is even.
}

function getLarger(first, second) {
  // TODO: Return the larger number. If equal, return either one.
}

// TODO: Call each function with at least three sets of inputs.
// TODO: Store one returned result in a variable and use it later.
```

Include zero, negative numbers, and equal numbers where relevant.

- [ ] My functions return values that other code can use.

## 7. Arrays

### Quick Questions

1. What is an array useful for?
2. How do you access its first and last elements?
3. How do `push()` and `pop()` affect an array?
4. Can you change the contents of an array declared with `const`?
5. What happens when you access an index that does not exist?

### Coding Task: Learning List

```js
const topics = ["variables", "conditions", "loops"];

// TODO: Add "functions" to the end.
// TODO: Print the first and last topics.
// TODO: Print each topic with a human-friendly number starting at 1.
// TODO: Check whether "arrays" is already in the list.
```

### Coding Task: Number Summary

Use loops for this exercise.

```js
const numbers = [8, 3, 12, 5, 2];

// TODO: Find the total.
// TODO: Find the largest number without using Math.max().
// TODO: Build a new array containing only numbers greater than 5.
```

Repeat with `[4]` and `[-8, -3, -12]`. Then try an empty array: decide how your program should report that there is no largest number.

- [ ] My largest-number logic also works when every number is negative.

## 8. Objects

### Quick Questions

1. How does an object differ from an array?
2. What are keys and values?
3. How do dot notation and bracket notation differ?
4. How do you add or update a property?

### Coding Task: Learner Profile

```js
const learner = {
  name: "Sam",
  lessonsCompleted: 2,
  isActive: true,
  skills: ["variables", "strings"],
};

// TODO: Print a sentence using the learner's name and lesson count.
// TODO: Increase lessonsCompleted by 1.
// TODO: Add "arrays" to skills.
// TODO: Add a goal property with a value of your choice.

const propertyToRead = "name";
// TODO: Read the property named by propertyToRead.
```

- [ ] I can read and update the array stored inside the object.

## 9. Array Methods

### Quick Questions

1. What is a callback function?
2. How do `map()`, `filter()`, and `find()` differ?
3. How does `forEach()` differ from `map()`?
4. What does `find()` return when nothing matches?

### Coding Task: Product List

```js
const products = [
  { name: "Notebook", price: 25, inStock: true },
  { name: "Pen", price: 10, inStock: false },
  { name: "Backpack", price: 180, inStock: true },
];

// TODO: Use map() to create an array of product names.
// TODO: Use filter() to get only products that are in stock.
// TODO: Use filter() to get products costing less than R50.
// TODO: Use find() to look up "Pen".
// TODO: Look up a missing product and handle that result before
// attempting to read its price.
```

- [ ] I can explain the kind of result returned by each method.

## 10. Debugging Practice

Each snippet has a problem. Explain it, fix it in your practice file, and run your corrected version.

### A. The Counter

The intention is to increase the count by one.

```js
const count = 0;
count = count + 1;
console.log(count);
```

### B. The Total

The intention is to print a numeric total.

```js
function add(a, b) {
  const total = a + b;
}

console.log(add(4, 6));
```

### C. The List

The intention is to print each name exactly once, with no extra output.

```js
const names = ["Asha", "Ben", "Chris"];

for (let index = 0; index <= names.length; index++) {
  console.log(names[index]);
}
```

### D. The Age Check

The intention is to check whether the age is exactly 18, without changing it.

```js
let age = 16;

if (age = 18) {
  console.log("You are 18.");
}

console.log(age);
```

- [ ] I can explain each bug in my own words.

## 11. Mini Challenge: Study Tracker

Combine the basics into a console-based study tracker. No webpage, libraries, or user-input system needed: call your functions directly to try them out.

```js
const studySessions = [
  { topic: "variables", minutes: 20, completed: true },
  { topic: "loops", minutes: 30, completed: false },
  { topic: "functions", minutes: 25, completed: true },
];

function addSession(topic, minutes) {
  // TODO: Add a session with completed initially set to false.
}

function completeSession(topic) {
  // TODO: Mark the first matching session as completed.
  // Return true if a match exists, or false if none exists.
}

function getTotalCompletedMinutes() {
  // TODO: Return the sum of minutes for completed sessions only.
}

function getPendingTopics() {
  // TODO: Return an array of topic names for unfinished sessions.
}

// TODO: Call your functions and print a readable progress summary.
```

### Requirements

- [ ] Add at least two sessions using your function.
- [ ] Complete a session by its topic.
- [ ] Handle a topic that does not exist without crashing.
- [ ] Calculate completed minutes without including pending sessions.
- [ ] Return pending topics as an array of strings.
- [ ] Check the behavior when there are no sessions.
- [ ] Check the behavior when all sessions are completed.

Optional stretch: make `addSession()` reject an empty or whitespace-only topic and a minutes value that is not a positive finite number. Choose a clear return value to indicate whether a session was added.

## Reflection

After each section, write a few lines:

1. What could I do from memory?
2. What did I need to look up?
3. What mistake did I make, and why did it happen?
4. Can I solve a similar task tomorrow without looking at today's code?

Revisit the tasks that felt awkward. Getting comfortable with the basics is the goal; speed can come later.
