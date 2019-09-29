le# Types Variables Logic and Operations Lab 2

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

let yourGrade:Double = 4.0
var averag = (yourGrade + grade1 + grade2 + grade3) / 4
if yourGrade > averag {
    print("above average")
} else {
    print("below average")
}

```

***
## Question 2

You are given a number. Print even if the number is even or odd otherwise.

```swift
let number = 2
if number % 2 == 0{
    print("even")
} else {
    print("odd")
}

```

***
## Question 3

You are given two numbers `a` and `b`. Print `"divisible"` if `a` isdivisible by `b` and `"not divisible"` otherwise.

```swift
var a = 12
var b = 3
print(a % b == 0 ? "divisible" : "not divisible" )

```

***
## Question 4

You are given three variables `a`, `b` and `c`. Check if at least two variables have the same value. If that is true, print `"At least two variables have the same value"` otherwise print `"All the values are different"`.

```swift
var a = 2
var b = 3
var c = 2
if a == b || b == c || a == c {
print("At least two variables are the same")
} else {
print("All values are different")
}
```

***
## Question 5

You are working on a smart-fridge. The smart-fridge knows how old the eggs and bacon in it are. You know that eggs spoil after 3 weeks (21 days) and bacon after one week (7 days). Given `baconAge` and `eggsAge` (both in days) determine if you can cook bacon and eggs, or which ingredients you need to throw out. If you can cook bacon and eggs, print `"you can cook bacon and eggs"`. If you need to throw out any ingredients, for each one print a line with the text `"throw out"` + bacon or eggs.

```swift
var baconAge = 6 // the bacon is 6 days old
var eggsAge = 12 // eggs are 12 days old

if baconAge <= 7 && eggsAge <= 21{
print("cook bacon and eggs")
} else if baconAge <= 7 && eggsAge > 21 {
print("throwout eggs")
} else if baconAge > 7 && eggsAge <= 21 {
print("throwout bacon")
} else if baconAge > 7 && eggsAge > 21 {
print("throwout bacon and eggs")
}
```

***
## Question 6

You are given a year, determine if it’s a leap year. A leap year is a year containing an extra day. It has 366 days instead of the normal 365 days. The extra day is added in February, which has 29 days instead of the normal 28 days. Leap years occur every 4 years. 2012 was a leap year and 2016 will also be a leap year.
The above rule is valid except that every 100 years special rules apply. Years that are divisible by 100 are not leap years if they are not also divisible by 400. For example 1900 was not a leap year, but 2000 was. Print `"Leap year!"` or `"Not a leap year!"` depending on the year you are provided.

```swift

let year = 2014
if ((year % 4 == 0) && (year % 100 == 0) && (year % 400 == 0)) || (year % 4 == 0) && (year % 100 != 0) {
    print("Leap year!")
} else {
    print("Not a leap year!")
}
```

***
## Question 7

If you use `random()` it will give you a random number within a specified range. Generate a random number and use it to simulate a coin toss. Print `"heads"` or `"tails"`.

```swift
var randomNum = Int.random(in: 0...1)
if randomNum == 0 {
    print("heads")
} else {
    print("tails")
}
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

if a < b  && a < c && a < d{
    print(a)
} else if b < c && b < d {
    print(b)
} else if c < d {
    print(c)
} else {
    print(d)
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


```
Answers: A,B,D,E


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


```
Answers: B,C



***
## Question 11

What is true about Integers in computers?

```swift
a. Integers must have a positive or negative sign always.
b. The maximum value for Integers is +∞.
c. Integer types in computers take up a fixed amount of memory.
d. Integers may contain decimals.

```
Answer: C

***
## Question 12

Select all the code snippets below that will compile.

```swift
a. let numberOfPages: Int = 500
b. let numberOfChapters = "For Whom The Bell Tolls"
c. let nameOfBook: Int = 14
d. let yearPublished = "Nineteen-thirty-five"


```
Answer: All of the above

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


```
Answer: 30

***
## Question 14

let div = 11 / 4

```swift
1. The value of div is ____________________(or write "div1 will not compile")

let div2 = 11.0 / 4.0
2. The value of div2 is ________________________(or write "div2 will not compile")
let isEqual = div == div2

3. The value of isEqual is_____________________ (or write "isEqual will not compile")


```
1: 2
2: 2.75
3: Will not compile

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

```
Answer: B


# Bonus 

***
## Question 1

What are the differences between Double and Int in the numbers they can represent and how they store them?

Answer: Double stores numbers to several decimal places, whereas integers only store as whole numbers, with decimals being rounded to those whole numbers to accomadate the data type.


***
## Question 2 

What are the differences between Float and Double?

Answer: A float is 32 bit and a double is 64 bit. Because of this, doubles can include more decimal places and are more accurate because of it.


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

```

***

## Question 6

You are given 2 Doubles a and b. Print their average

```swift
var a = 2.0
var b = 5.0

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

```
***

## Question 10 

A farmer is harvesting wheat from a number of wheat fields, given in a variable numberOfFields of type Int. Each field produces the same quantity of wheat given in a variable wheatYieldof type Double. Sometimes the harvest is increased by 50% due to favorable weather conditions. You are given this information in a variable weatherWasGood of type Bool.

### Print the total amount of wheat that the farmer will harvest.

<img width="270" alt="Screen Shot 2019-09-12 at 1 50 33 PM" src="https://user-images.githubusercontent.com/43886240/64808175-c03a4180-d564-11e9-8502-4fcade888dc1.png">

```

