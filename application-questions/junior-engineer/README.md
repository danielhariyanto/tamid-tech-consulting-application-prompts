# Junior Software Engineer Application
For your application, it is highly recommended that you comment your code as
clearly as possible. Make sure to remember important software engineering
principles:
* Methods less than 15 lines of code
* DRY (Don't Repeat Yourself!)
* KISS (Keep It Simple Silly!)

**You may complete the application in any coding language that you would like.**
# Challenge 1: Sorting
Given two sorted arrays (*arr1*, *arr2*) and a number, *k*, create a method,
`sortArrays` that returns a sorted array of the first *k* elements.

> Bonus points if you write this in one line - it's possible!

### Examples
```
Array 1: [1, 3, 5, 8]
Array 2: [1, 2, 3]
Number (k): 5

sortArrays(arr1, arr2, k) returns:
[1, 1, 2, 3, 3]
```

```
Array 1: [2, 8, 15, 30]
Array 2: [1, 2, 3]
Number (k): 2

sortArrays(arr1, arr2, k) returns:
[1, 2]
```

```
Array 1: [1, 3, 5, 8]
Array 2: [1, 2, 3]
Number (k): 0

sortArrays(arr1, arr2, k) returns:
[]
```

```
Array 1: [1, 3, 5, 8]
Array 2: []
Number (k): 10

sortArrays(arr1, arr2, k) returns:
[1, 3, 5, 8]
```

# Challenge 2: Calculator
Create a program that acts as a calculator.

This program should prompt the user for two numbers, and a function
(+, -, \*, /, and %). It should then print out the result.

You should keep prompting the user to do more calculations until they enter
`"n"`.

You *must* have error handling.

## Examples

```
  Welcome to the TAMID Calculator!

  Would you like to calculate something (y/n): y

  Please enter the first number: 1
  Please enter the second number: 2
  Please enter your function: *

  Your result was: 2!

  Would you like to calculate something (y/n): n

  Thanks for coming!
```

```
  Welcome to the TAMID Calculator!

  Would you like to calculate something (y/n): y

  Please enter the first number: 1
  Please enter the second number: 0
  Please enter your function: /

  You cannot divide by 0!

  Would you like to calculate something (y/n): n

  Thanks for coming!
```

# Challenge 3: Boxed Strings
Write a function that takes a list of strings an prints them, one per line,
in a rectangular frame.

> Helpful hint: The longest word will dictate the width of the box.

## Example
For example the list `["TAMID", "IS", "THE", "COOLEST"]`
gets printed as:

```
***********
* TAMID   *
* IS      *
* THE     *
* COOLEST *
***********
```

# Challenge 4: Palindrome
Write a function, `isPalindrome?` that tests whether a string is a palindrome.
A palindrome is defined as a word that is the exact same forwards as it is
backwards.

> Bonus points if you can make the function body one line!

## Example
```
Please enter a string: wow

"Wow" is a palindrome!

```

```
Please enter a string: TAMID

"TAMID" is not a palindrome!

```
