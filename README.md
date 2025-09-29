# -practice-readline-sync--Jessica----K-
## Assignment: Readline Sync Quiz

**Objective:**  
- Use the `readline-sync` Node.js module to interactively ask users questions and collect their responses.
- Prompt the user for their name and greet them.
- Use `readline-sync.question()` to ask 5 questions that test knowledge of Values, Data Types, and Operations.
    - At least one question should prompt the user for a number.
- Store the user’s answers in variables.
- Print the value of those answers back to the user.

---

### Example Solution

```js
// Import readline-sync for interactive input
const readlineSync = require('readline-sync');

// Prompt for user's name and greet them
const userName = readlineSync.question('What is your name? ');
console.log(`Hello, ${userName}! Welcome to the quiz.`);

// Ask 5 questions
const favoriteColor = readlineSync.question('What is your favorite color? ');
const birthYear = readlineSync.question('What year were you born? (Please enter a number) ');
const isJavaScriptFun = readlineSync.question('Do you think JavaScript is fun? (yes/no) ');
const dataTypeString = readlineSync.question('What data type is "hello"? ');
const operationResult = readlineSync.question('What is the result of 2 + 2? ');

// Print the user's answers
console.log(`\nHere are your answers:`);
console.log(`Name: ${userName}`);
console.log(`Favorite Color: ${favoriteColor}`);
console.log(`Birth Year: ${birthYear}`);
console.log(`JavaScript is fun: ${isJavaScriptFun}`);
console.log(`Data type of "hello": ${dataTypeString}`);
console.log(`Result of 2 + 2: ${operationResult}`);
```