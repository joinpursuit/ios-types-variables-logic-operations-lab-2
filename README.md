# Types Variables Logic and Operations Lab 2

## Instructions for lab submission

1. Fork the assignment repo
1. Clone your Fork to your machine
1. Complete the lab
1. Push your changes to your Fork
1. Submit a Pull Request back to the assignment repo
1. Paste a link to of your Fork on Canvas and submit

## Question 1

You are given three grades obtained by 3 students, which are stored in variables `grade1`, `grade2`, `grade3` and all of type `Double`.
Create a variable called `yourGrade` of type `Double` and give it a value.
Print `"above average"` if your grade is greater than the class average or `"below average"` otherwise.

```swift
var grade1 = 7.0
var grade2 = 9.0
var grade3 = 5.0

// your code here

_______________________
Answer:

var grade1 = 7.0
var grade2 = 9.0
var grade3 = 5.0
var yourGrade = 9.5

var averageGrade = (grade1 + grade2 + grade3 + yourGrade) / 4  // Output 7.625

if yourGrade < averageGrade {
    print("Below average")
} else if yourGrade > averageGrade {
print("Above average")
} else {
print("Average")
}

// Prints "Above average"
```

***
## Question 2

You are given a number. Print even if the number is even or odd otherwise.

```swift
let number = 2

// your code here
_______________________
Answer:

let number = 2

if number % 2 == 0 {
print("Even")
} else {
print("Odd")
}

// Prints "Even"
```

***
## Question 3

You are given two numbers `a` and `b`. Print `"divisible"` if `a` is divisible by `b` and `"not divisible"` otherwise.

```swift
var a = 12
var b = 3

// code here
______________________________

Answer:

var a = 12
var b = 3

if a % b == 0 {
print("Divisible")
} else {
print("Not divisible")
}

// Prints "Divisible."

```

***
## Question 4

You are given three variables `a`, `b` and `c`. Check if at least two variables have the same value. If that is true, print `"At least two variables have the same value"` otherwise print `"All the values are different"`.

```swift
var a = 2
var b = 3
var c = 2

// your code here

________________________________
Answer:

var a = 2
var b = 3
var c = 2

if a == b || b == c || a == c {
    print("At least two variables have the same value.");
} else {
    print("All the values are different.")
}

// Prints "At least two variables have the same value"

WE COUDL WRITE IT IN OTHER WAY:

var a = 2
var b = 3
var c = 2


if a == b {
    print("At least two variables have the same value.")
} else if b == c {
    print("At least two variables have the same value.")
} else if a == c {
    print("At least two variables have the same value.")
} else {
    print("All the values are different.")
}

// Prints "At least two variables have the same value"
```

***
## Question 5

You are working on a smart-fridge. The smart-fridge knows how old the eggs and bacon in it are. You know that eggs spoil after 3 weeks (21 days) and bacon after one week (7 days). Given `baconAge` and `eggsAge` (both in days) determine if you can cook bacon and eggs, or which ingredients you need to throw out. If you can cook bacon and eggs, print `"you can cook bacon and eggs"`. If you need to throw out any ingredients, for each one print a line with the text `"throw out"` + bacon or eggs.

```swift
var baconAge = 6 // the bacon is 6 days old
var eggsAge = 12 // eggs are 12 days old

// your code here

_____________________________________________

Answer:

var baconAge = 6
var eggsAge = 12

if baconAge <= 7 && eggsAge <= 21 {
print("You can cook bacon and eggs.")
} else if baconAge <= 7 && eggsAge > 21 {
    print("You can cook bacon, but throw out eggs.")
} else if eggsAge <= 21 && baconAge > 7 {
    print("You can cook eggs, but throw out bacon.")
} else {
print("Throw out bacon and eggs.")
}

// Prints "You can cook bacon and eggs"
```

***
## Question 6

You are given a year, determine if it’s a leap year. A leap year is a year containing an extra day. It has 366 days instead of the normal 365 days. The extra day is added in February, which has 29 days instead of the normal 28 days. Leap years occur every 4 years. 2012 was a leap year and 2016 will also be a leap year.
The above rule is valid except that every 100 years special rules apply. Years that are divisible by 100 are not leap years if they are not also divisible by 400. For example 1900 was not a leap year, but 2000 was. Print `"Leap year!"` or `"Not a leap year!"` depending on the year you are provided.

```swift
let year = 2014

// your code here
________________________
Answer:
let year = 2014

if year % 400 == 0 {
    print("Leap year!")
} else if year % 4 == 0 && year % 100 == 0 {
    print("Not a leap year!")
} else if year % 4 == 0 {
    print("Leap year!")
} else {
    print("Not a leap year!")
}

// Output "Not a leap year!"
```

***
## Question 7

If you use `random()` it will give you a random number within a specified range. Generate a random number and use it to simulate a coin toss. Print `"heads"` or `"tails"`.

```swift
let randomNum = Int.random(in: 0...100)

// your code here
```

Hint: use an if/else block along with the `%` operator

***
## Question 8

You are given four variables `a`, `b`, `c` and `d`. Print the value of the smallest one.

```swift
var a = 5
var b = 6
var c = 3
var d = 4

// your code here

_______________________
Answer:

let randomNumber = Int.random(in: 0...100)

if randomNumber % 2 == 0 {
print("Heads")
} else {
print("Tails")
}

```

***
## Question 9

Which of the following expressions evaluate to true?

```swift
a. 3 == 2 || 9 == 9
b. !(3 > 3)
c. !(true || false)
d. (4 < 3 || 4 > 3) && ("Message: " == "Message: ")
e. !(3 != 3)

__________________________________________________
Answer:
a
b
d
e

```

***
## Question 10

Given the below, which of the following expressions evaluate to true?

```swift
 let x = 5 > 4
 let y = 100 / 10 == 1
 let z = 6
```

```swift
a. x && y
b. x || y || z == 1
c. ("five" == "5" || "FIVE" == "five" || 5 == 3 + 2) && !y
d. (x && y) || z > 6
e. !(z < 6) && !y && !x
____________________________
Answer:
b
c


```


***
## Question 11

What is true about Integers in computers?

```swift
a. Integers must have a positive or negative sign always.
b. The maximum value for Integers is +∞.
c. Integer types in computers take up a fixed amount of memory.
d. Integers may contain decimals.

__________________________________
Answer:
c

```


***
## Question 12

Select all the code snippets below that will compile.

```swift
a. let numberOfPages: Int = 500
b. let numberOfChapters = "For Whom The Bell Tolls"
c. let nameOfBook: Int = 14
d. let yearPublished = "Nineteen-thirty-five"

__________________________________________________
Answer:
a
b
c
d

```

***
## Question 13

What will the code below print?  Complete this exercise without using an IDE (Integrated Developer Environment) or calculator 

```swift
var a = 20
var b = 5
var c = 4

a += b
b -= c
b * (c + a)
(b * c) + a
b %= a
b %= c

print(a + b + c)

________________________
Answer:

var a = 20
var b = 5
var c = 4

a += b  // Equals a + b = newA 20 + 5 = 25
b -= c  // Equals b - c = newB 5 - 4 = 1
b * (c + a)  // 29
(b * c) + a  // 29
b %= a  // Equals newB % newA = newNewB  1 % 25 = 1
b %= c  // Equals newNewB % c = superNewNewB 1 % 4 = 1

print(a + b + c)  // newA + superNewNewB + c = 25 + 1 + 4 = 30



```

***
## Question 14

let div = 11 / 4

```swift
1. The value of div is ____________________(or write "div1 will not compile")

let div2 = 11.0 / 4.0
2. The value of div2 is ________________________(or write "div2 will not compile")
let isEqual = div == div2

3. The value of isEqual is_____________________ (or write "isEqual will not compile")

_____________________________________________________________________________________
Answer:

1. The value of div is 2.

2. The value of div2 is 2.75

3. isEqual will not compile.



```
***
## Question 15
```swift
var n = 7.5

```

What is true about the variable n?

```swift
a. n is a Float
b. n is a Double
c. n is a Decimal
d. In is an Int

________________________
Answer:
b // I think it can be a Float as well but should be assign as var n: Float = 7.5
```

# Bonus 

***
## Question 1

What are the differences between Double and Int in the numbers they can represent and how they store them?

_______________________________________________________________
Answer:
Double reprecent decimals and Int represent whole numbers. Double store numbers more precise and Int store numbers without decimals. 


***
## Question 2 

What are the differences between Float and Double?
Float has 6 digits after the period and uses 32 bits to store their data.
Double has 15 digits after period and uses 64 bits to store their data.
I read that in app that does requares speed vs. exact numbers Floats would be preferable to use. Ans vise versa.


***

## Question 3

What will happen when the code below is run?

```swift

var width: Double = 49.8
var extraWidth: Float = 10.1
let totalWidth = width + extraWidth
print(totalWidth)

a. It will print 48.9
b. It will print 50.0
c. It will print 50
d. It will give a compile-time error

__________________________________
Answer:
d

```
***
## Question 4 

You are given a number a. 
Print the last digit of a.

var a = 123

```swift

Example 1
Input: 
var a = 123

Output:
3

Example 2
Input: 
var a = 337

Output:
7


_________________________
Answer:

Example 1:
var a = 123

a %= 10

print(a) // Output 3

Example 2:
var a = 337

a %= 10

print(b) // Output 7

```

***

## Question 5 

Given an int, determine and print whether it is even or odd.

```swift
var number = 5

Example 1
Input: 
var number = 6

Expected Output: 
Even

-------------------
Answer:
var number = 5

if number % 2 == 0 {
print("Even")
} else {
print("Odd")
}

// Output Odd

Example 1:
var number = 6

if number % 2 == 0 {
print("Even")
} else {
print("Odd")
}
 
 // Output Even
```

***

## Question 6

You are given 2 Doubles a and b. Print their average

```swift
var a = 2.0
var b = 5.0

________________
Answer:

var a = 2.0
var b = 5.0

var average = (a + b) / 2

print("average")  // Output 3.5

```


***

## Question 7 

You are given 3 grades stored in 3 variables of type Double finalsGrade, midtermGrade, projectGrade. These grades are used to compute the grade for a class. finalsGrade represents 50% of the grade. midtermGrade represents 20% of the grade. projectGrade represents 30% of the final grade.

### Print the grade for the class.

```swift

var finalsGrade = 2.0
var midtermGrade = 4.0
var projectGrade = 3.0

```
Answer:
var finalsGrade = 2.0
var midtermGrade = 4.0
var projectGrade = 3.0

var finalGradeToTotal = 2.0 * 0.5
var midtermGradeToTotal = 4.0 * 0.2
var projectGradeToTotal = 3.0 * 0.3

var gradeForTheClass = finalGradeToTotal + midtermGradeToTotal + projectGradeToTotal

// Output 2.7

***

## Question 8 

You have the cost of a meal at a restaurant stored in a variable mealCost of type Double. You would like to leave a tip of a certain percentage. The percentage is stored in a variable tip of type Int.

### Print the total cost of the meal.
```swift

Input: 
var mealCost:Double = 3.5
var tip:Int = 20


Output:
4.2

```
---------------------------------------
Answer:
I don't know how to solve since there are different types of data. Did I miss something?

***

## Question 9

You are given three grades obtained by 3 students in a class stored in variables grade1, grade2, grade3 of typeDouble. You are also given your grade in the class stored in a variable yourGrade of type Double. Print above average if your grade is greater than the class average or below average” otherwise.

### Note: the average of the class includes your grade.
```swift

Input: 
var grade1 = 7.0
var grade2 = 9.0
var grade3 = 5.0
var yourGrade = 8.0

Output:
"above average"
____________________________
Answer:

var grade1 = 7.0
var grade2 = 9.0
var grade3 = 5.0
var yourGrade = 8.0

var average = (grade1 + grade2 + grade3 + yourGrade) / 4

if yourGrade > average {
print("above average")
} else if yourGrade == average {
print("average")
} else {
print("below average")
}

```
***

## Question 10 

A farmer is harvesting wheat from a number of wheat fields, given in a variable numberOfFields of type Int. Each field produces the same quantity of wheat given in a variable wheatYieldof type Double. Sometimes the harvest is increased by 50% due to favorable weather conditions. You are given this information in a variable weatherWasGood of type Bool.

### Print the total amount of wheat that the farmer will harvest.

---------------------------------------
Answer:
I don't know how to solve it without changing Int to Double. Did I miss something?

<img width="270" alt="Screen Shot 2019-09-12 at 1 50 33 PM" src="https://user-images.githubusercontent.com/43886240/64808175-c03a4180-d564-11e9-8502-4fcade888dc1.png">

```

