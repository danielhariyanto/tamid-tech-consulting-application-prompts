# Senior Software Engineer Application
For your application, it is highly recommended that you comment your code as
clearly as possible. Make sure to remember important software engineering
principles:
* Methods less than 15 lines of code
* DRY (Don't Repeat Yourself!)
* KISS (Keep It Simple Silly!)

**You may complete the application in any coding language that you would like.**=

## Challenge 1: Sorting & Runtime
Given two sorted arrays (*arr1*, *arr2*) and a number, *k*, create a method,
`sortArrays` that returns a sorted array of the first *k* elements.

> Bonus points if you can comment the space/time complexity of your method.
> Bonus points if you do this in O(n).
> Bonus points if you write this in one line and it runs in O(n*logn)

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

## Challenge 2: Object-Oriented Programming
Congratulations! You are the new owner of the *Brandeis Ice Cream Truck*!
For this challenge, you will be responsible for creating a Object-Oriented
Ice Cream Truck.

**This is purposefully open-ended.** You may code it however you would like. Try
to re-use your code as much as possible. You should make use of
Object-Oriented principles such as Inheritance, Polymorphism, Abstraction, and
Encapsulation (you do not need to use all of them if you do not want to. Just
use them where they make sense!)

Make use of methods as much as possible in order to reuse code.

You should also do as much error-checking as you deem valid.

### Console
The Console class should run your program. You should prompt the user for
a number, which represents the *start-up cash* of the ice cream truck.

You may create customers and employees upon initialization of your ice cream
truck.

Console should have a looped prompt, that prompts the user to do several things:
* Add a new Ice Cream Flavor
* Hire a new Truck Worker
* Hire a new Driver
* Show all Employees
* Show Ice Cream stock
* Purchase more Ice Cream of an existing flavor
* Display # of sales (both the number of ice cream sold, and the cash those sales generated)
* Close for the day (quit the loop)

Every time you enter a prompt, a *single* customer is selected
and tries to purchase a random ice cream flavor.
They can purchase that ice cream if they have enough money, or they are told to
leave. You should store  Customers in a data structure, and remove them after
they attempt to make a purchase. If you have run out of ice cream, close, or
have satisfied all customers, then the program should end.

> You should go through all of these systematically. Complete one thing at a
time, and then move on to the next one.

### Ice Cream
Ice Cream has a name, a price for customers to buy, a cost for the truck to
purchase, and a number of initially bought scoops.

### Customer
A customer has a name, age, and number of dollars in their bank account.

A customer will select a random flavor and number of scoops and purchase it.

If they do not have enough money, they are turned away.

You should create a toString method that prints information about the customer.

### Truck
A truck is responsible for keeping track of what flavors it has in stock,
how much money it has, how many sales it has made, and how much ice cream it
has bought.

### Truck Worker
A Truck Worker has a name, age, and a wage. They must have an employment status.

They must have permission to access the register.

You should create a toString method that prints information about the Truck
Worker.

### Driver
A Driver has a name, age, and a wage. They must have an employment status.

They must have permission to drive the truck.

You should create a toString method that prints information about the Driver.

> Bonus points for any unit testing or clean documentation

### Example Output

```
Congratulations! You have decided to start your own Ice Cream Truck! What is
your new business's name and how much would you like to invest?

Business Name: Liebowitz's Ice Cream Truck
Start-Up Cash: 500

You have created Liebowitz's Ice Cream Truck, and invested $500!

The following customers are in line: [Mitchell, Bob]

Welcome to Liebowitz's Ice Cream Truck!
Please select an option from the menu below:
1. Add a new Ice Cream Flavor
2. Hire a new Truck Worker
3. Hire a new Driver
4. Show all Employees
5. Show Ice Cream stock
6. Purchase more Ice Cream of an existing flavor
7. Display # of sales (both the number of ice cream sold, and the cash those
sales generated)
8. Close for the day (quit the loop)

User Input:
> 1

What flavor would you like to add?
Name: Vanilla
Number of Scoops: 24
Cost to Customer: 1.30
Cost of purchase: 0.50.

CUSTOMER PURCHASE:
Mitchell has $3 in their bank account. They purchased a 2 scoop of Vanilla for
$2.60.

Please select an option from the menu below:
1. Add a new Ice Cream Flavor
2. Hire a new Truck Worker
3. Hire a new Driver
4. Show all Employees
5. Show Ice Cream stock
6. Purchase more Ice Cream of an existing flavor
7. Display # of sales (both the number of ice cream sold, and the cash those
sales generated)
8. Close for the day (quit the loop

User Input:
> 7

Leibowitz's Ice Cream Truck has sold 2 scoops for $2.60:
* 2 Scoops of Vanilla Ice cream

CUSTOMER PURCHASE:
Bob has $1 in their bank account.
They cannot purchase ice cream.

There are no more customers for the day. Goodbye!

```

> Again, you do not need to follow this exact output. I will be looking
mostly at the business-logic of your code. You should have a similar output to
this.

## Challenge 3: Debugging
This program is supposed to calculate how much money you would have left
if you were given a penny and multiplied it by 30 days.

You can find the code in the `Debug.java` file.

Your output should look exactly like the output below.

### Expected Output:
```
After day 1 you have 0.02
After day 2 you have 0.04
After day 3 you have 0.08
After day 4 you have 0.16
After day 5 you have 0.32
After day 6 you have 0.64
After day 7 you have 1.28
After day 8 you have 2.56
After day 9 you have 5.12
After day 10 you have 10.24
After day 11 you have 20.48
After day 12 you have 40.96
After day 13 you have 81.92
After day 14 you have 163.84
After day 15 you have 327.68
After day 16 you have 655.36
After day 17 you have 1310.72
After day 18 you have 2621.44
After day 19 you have 5242.88
After day 20 you have 10485.76
After day 21 you have 20971.52
After day 22 you have 41943.04
After day 23 you have 83886.08
After day 24 you have 167772.16
After day 25 you have 335544.32
After day 26 you have 671088.64
After day 27 you have 1342177.28
After day 28 you have 2684354.56
After day 29 you have 5368709.12
```
