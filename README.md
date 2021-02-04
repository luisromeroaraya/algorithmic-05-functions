# Functions
* Type of challenge: **learning**
* Duration: **30 min**
* Team challenge: **solo**

## Learning objectives
At the end of this challenge you should:
* understand the concept of functions
* be able to write custom functions

## The mission
This challenge will have you play around with the concept of [functions](https://en.wikipedia.org/wiki/Subroutine), complete the exercises down below after you’ve read the explanations.

A function is a subroutine, meaning a piece of instructions executed if called within the main code. It can be used multiple times with different sets of value each call. It usually needs to return a value with the return command.

Example
```
// This function returns the square of a number
function square(nbr) {
	return $nbr * $nbr
}

output(square(5))// prints "25"
```

## Exercises

*I will be using [Python3](https://repl.it/languages/python3) to write and test the algorithms*

Instructions
- [x] translate five previous exercises into modular functions
```
def inputNum():
    num=int(input("Enter your number:"))
    return num

def printNum(num):
    print("Your number is:", num)

num=inputNum()
printNum(num)

def inputArr():
    array=[]
    n=int(input("Please write the number of elements you want for your array: (1-10)"))
    for x in range(n):
        element=input("Please enter element:")
        array.append(element)
    return array

def printArr(array):
    print("The elements in the array are:")
    for x in array:
        print("[", x,"]")

array=inputArr()
printArr(array)

def isOrdered(array):
    first=array[0]
    order=True
    for x in array:
        if x < first:
            order=False
        first=x
    if order:
        print("The elements are ordered")
    else:
        print("The elements are not ordered")

isOrdered(array)
```

- [x] detail each and every step

## Resources
* [conventions](https://github.com/becodeorg/BXL-Swartz-4-27/blob/master/1.The-Field/7.Algorithmic/conventions.adoc)
* [function](https://computersciencewiki.org/index.php/Functions)
