# JavaScript Programming Exercises

---

---

## Level Description

### 🟢 Simple Programs

These programs require understanding about variables, conditions.

### 🟡 Intermediate Programs

These programs require understanding about loops, funcions and how to apply logic using them.

### 🔴 Algorithms Programs

These programs require the understanding of how different algorithms work.

### 🔵 DOM Manipulation Programs

These programs require knowledge about DOM events and how to manipulate the DOM.

---

---

## Practice Questions

#### Question 1 🟢

Q: Find the Sum of two predefined numbers where value of num1 = 5 and value of num2 = 7.

```javascript
const num1 = 5;
const num2 = 7;
const sum = num1 + num2;
console.log(sum);
// console.log prints the output in console
```

#### Question 2 🟢

Q: Find the quotient of given two numbers where value of num1 = 28 and num2 = 4 and show in console.

```javascript
const num1 = 28;
const num2 = 4;
const quotient = num1 / num2;
console.log(quotient);
```

#### Question 3 🟢

Q: Find the simple interest when value of Principal amount is 5000, Rate of interest is 8% and Time period is 3 years.

Hint: I = PRT / 100

```javascript
const p = 5000;
const r = 8;
const t = 3;
const i = (p * r * t) / 100;
console.log(i);
```

#### Question 4 🟢

Q: Adding, Subbstracting, Multiply and Divison using assignment Operators. value of num1 = 49, num2 = 10.

```javascript
let num1 = 49;
let num2 = 10;

num1++;
console.log(num1); // short syntax for num1 = num1  + 1

num1 += num2; // this is short syntax for num1 = num1 + num2
console.log(num1); // Output is 60

num1 -= num2; // short syntax  for num1 = num1 - num2
console.log(num1); // Output is 50

num1 /= num2;
console.log(num1); // Output  is 5

num1 *= num2;
console.log(num1); // Output is 50.

num1 %= num2;
console.log(num1);
```

To learn more about these Operators visit [MDN Operators](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Expressions_and_Operators#Assignment "Assignment Operators")

#### Question 5 🟢

Q: Take name input from user using prompt and print their name and surname on console.

```javascript
// prompt takes an input from the user
const name = prompt("Please enter your name");
const surname = prompt("Please enter your surname");
console.log(name + " " + surname);
```

#### Question 6 🟢

Q: Take two numbers from a user and find maximum number out of those two.
Ex: no1 = 5 and no2 = 10 then no2 is greater

Hint: use if else condition and comparison operator.

```javascript
// parseInt converts the digits into numbers
const num1 = parseInt(prompt("Please enter only digits"));
const num2 = parseInt(prompt("Please enter only digits"));
if (num1 > num2) {
  console.log("num1 is greater no");
} else {
  console.log("num2 is greater no");
}
```

#### Question 7 🟢

Q: Find minimum out of 3 numbers whose values are given by user.
Ex: no1 = 6, no2 = 8, no3 = 4 then no3 is smallest no.

Hint: Use nested If Else and comparison operator.

```javascript
const num1 = parseInt(prompt("Please Enter no1"));
const num2 = parseInt(prompt("Please Enter no2"));
const num3 = parseInt(prompt("Please Enter no3"));

if (num1 < num2) {
  if (num1 < num3) {
    console.log("number 1 is the smallest no.");
  } else {
    console.log("number 3 is the smallest no.");
  }
} else {
  if (num2 < num3) {
    console.log("number 2 is the smallest no.");
  } else {
    console.log("number 3 is the smallest no.");
  }
}
```

#### Question 8 🟢

Q: Make a Grading System in which User gets grade on screen based on their mark input.
Ex: If marks = 85 then Grade is A-, marks = 65 then grade is B-.

Hint: use if and else if condition.

```javascript
const marks = parseInt(prompt("Enter marks in Digits"));

if (marks > 90) {
  console.log("You got A+");
} else if (marks > 80) {
  console.log("You got A-");
} else if (marks > 70) {
  console.log("You got B+");
} else if (marks > 60) {
  console.log("You got B-");
} else if (marks > 50) {
  console.log("You got C");
} else if (marks > 40) {
  console.log("You got D");
} else {
  console.log("You have failed the exam");
}
```

#### Question 9 🟡

Q: Take a number input from user and find the factorial of that no.
Ex: no = 3, factorial = 1 + 2 + 3 which is 6.

Hint: Use For loop.

```javascript
let no = parseInt(prompt("Please enter a digit"));
let factorial = 1;
for (let i = 1; i <= no; i++) {
  factorial *= i;
  console.log(factorial);
}
console.log("Factorial is", factorial);
```

#### Question 10 🟡

Q: Star Pattern

\*
\*\*
\*\*\*
\*\*\*\*
\*\*\*\*\*

Hint: Using For loop

```javascript
let i;
let star = " ";

for (let i = 1; i <= 5; i++) {
  star = star + "*";
  console.log(star);
}
```

#### Question 11 🟡

Q: Print 100 numbers but print "Fizz" for multiples of 3, "buzz" for multiples of 5 and "FizzBuzz" for multiples of both 3 & 5.
Ex: 1 , 2, Fizz, 4, Buzz, 6, ..... 13, 14, FizzBuzz.

Hint: Use For and if else.

```javascript
for (let i = 1; i <= 100; i++) {
  if (i % 15 == 0) console.log("FizzBuzz");
  else if (i % 3 == 0) console.log("Fizz");
  else if (i % 5 == 0) console.log("Buzz");
  else console.log(i);
}
```

**Note**: This can be done with shorter syntax using [Ternary Operator](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Conditional_Operator).

#### Question 12 🟡

Q: Make a Multiply function which takes three numbers and returns the ans.
Ex: multiply(3,5,8) returns 120.

```javascript
function multiply(no1, no2, no3) {
  sum = no1 * no2 * no3;
  return sum;
}
```

#### Question 13 🟡

Q: Make a Function which takes an input N number from user and returns the cube of every number from 1 to N in an array.
Ex: n = 4. arr = [1, 8, 27, 64]

Hint: Use for loop and array.push method.

```javascript
const arr = [];
let no = parseInt(prompt("Please Enter a no"));
let cube;

function cubeMaker(number) {
  for (let i = 1; i <= number; i++) {
    cube = i * i * i;
    arr.push(cube);
  }
  return arr;
}

cubeMaker(no);
```

#### Question 14 🟡

Q: Take a no from User and Generate a fibonacci series for that no.
Ex: number = 3, output -> 0,1,1,2,3

Hint: Use for Loop

```javascript
let no = parseInt(prompt("Please Enter a no"));
let n1 = 0;
let n2 = 1;
let n3 = 0;

function fibonacci(number) {
  for (let i = 0; i <= number; i++) {
    console.log(n3);
    n1 = n2;
    n2 = n3;
    n3 = n1 + n2;
  }
  console.log(n3);
}

fibonacci(no);
```

#### Question 15 🟡

Q: Take string input from the user and then reverse the string.
Ex: "Javascript" -> "tpircsavaJ"

Hint: Use for loop and access string Charachters using index.

```javascript
const string = prompt("Enter the String");

function reverseStr(str) {
  let reverse = "";
  for (let i = str.length - 1; i >= 0; i--) {
    reverse += str[i];
  }
  return reverse;
}

reverseStr(string);
```

#### Question 16 🟡

Q: Take a string Input from user and find the longest word in the String.
Ex: "hello everyone, i am here" -> everyone is longest word.

Hint: Use for loop and split the string into the arrays.

```javascript
const stringInput = prompt("Enter your String");

function longestWord(str) {
  let splitString = str.split(" ");
  let longestLength = 0;
  let longestWord = "";
  for (let i = 0; i < splitString.length; i++) {
    if (splitString[i].length > longestLength) {
      longestLength = splitString[i].length;
      longestWord = splitString[i];
    }
  }
  return longestWord;
}

longestWord(stringInput);
```

#### Question 17 🟡

Q: Take a string Input from user and verify if that string is palindrome or not.
Ex: "kayak" in reverse is "kayak" so it is a palindrome. "hello" in reverse is "olleh" and hence its not a palindrome.

Hint: use for loop and check the if characters are same from both sides

```javascript
const inputStr = prompt("Please enter your Word");
function palindrome(str) {
  let string = str.toLowerCase();
  let len = string.length;
  for (let i = 0; i < len; i++) {
    // for reverse order characters -> console.log(str[len - 1 - i]);
    if (str[i] !== str[len - 1 - i]) {
      return false;
    }
  }
  return true;
}
palindrome(inputStr);
```

#### Question 18 🟡

Q: Take Input From User and Determine weather it is an armstrong Number or not.
Ex: 153 is an armstrong no. because 1^3 + 5^3 + 3^3 = 153 which is equal to the digit itself.

Hint: Use For loop and if else, use modulo and division.

```javascript
const inputNo = parseInt(prompt("Please Enter No"));

function armstrong(no) {
  let remainder;
  let cube;
  let sum = 0;
  for (no1 = no; no1 > 0; no1 / 10) {
    remainder = no1 % 10;
    cube = remainder * remainder * remainder;
    no1 = parseInt(no1 / 10);
    sum = sum + cube;
  }

  if (no === sum) {
    console.log("Yes it is an armstrong no");
  } else {
    console.log("No it is not an armstrong no");
  }
}

armstrong(inputNo);
```

#### Question 19 🔴

Q: Make a function which can sort the numbers in a given array in ascending order using Bubble Sort.
Ex: [5,3,8,2] -> [2,3,5,8]

Hint: use for Loop, swap the values using an extra variable.

```javascript
const arr = [35, 28, 69, 12, 6, 87, 45];

function bubbleSort(arr) {
  let len = arr.length;
  for (let i = 0; i < len; i++) {
    for (let j = 0; j < len; j++) {
      if (arr[j] > arr[j + 1]) {
        let temp = arr[j];
        arr[j] = arr[j + 1];
        arr[j + 1] = temp;
      }
    }
  }
  return arr;
}

bubbleSort(arr);
```

**Note**: This can be improved by making a Swap Function.

#### Question 20 🔴

Q: Make a function which can sort the numbers in a given array in descending order using Selection Sort.
Ex: [5,3,8,2] -> [8,5,3,2]

Hint: use for Loop, swap the values using an extra variable.

```javascript
const arr = [35, 28, 69, 12, 6, 87, 45];

function selectionSort(arr) {
  for (let i = 0; i < arr.length; i++) {
    let lowest = i;
    for (let j = i + 1; j < arr.length; j++) {
      if (arr[j] > arr[lowest]) {
        lowest = j;
      }
    }
    if (i !== lowest) {
      let temp = arr[i];
      arr[i] = arr[lowest];
      arr[lowest] = temp;
    }
  }

  return arr;
}

selectionSort(arr);
```

**Note**: This can be improved by making a Swap Function.
