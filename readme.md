# yanee brain 01

## basics

- datatypes (int, str, float, boolean), list(array)
- variables 
- loops(for, each, while)

``` python
# basic for loop
for i in range(start,end,step):
    print ('i')
# each example
nameOfDays = ['saturday','sunday','monday']
start = 0
end = len(nameOfDays)

for i in range(start,end):
    print(namneOfDays[i])

for eachDay in nameOfDays:
    print(eachDay)

i = 25
while i > 20 do:
    print (i)
    i = i-1
```

- conditional statement

``` python
a = 10
for i in range (5,15):
    if i < a:
        print ('i am small')
    else:
        print ('i m big')

```

- function and procedures
  - set of task , group
  - can take input arguments
  - can return value to some other variable

``` python

# create a function that calc area of rectangle
def rectAreaCalc (length, width):
    area = length * width
    print ("Area of rect is:", area)
    return area

```

- exception handling

``` python

# basic mindset for exception planning
def rectAreaCalc (length, width):
    if type(length) != [int,float]:
        print ("Exception: length should be some math value")
    elif type(width) != [int,float]:
        print ("Exception: width should be some math value")
    else:
        area = length * width
        print ("Area of rect is:", area)
    return area

```

``` python
# second best official way
import sys

randomList = ['a', 0, 2]

for entry in randomList:
    try:
        print("The entry is", entry)
        r = 1/int(entry)
        break
    except:
        print("Oops!", sys.exc_info()[0], "occurred.")
        print("Next entry.")
        print()
#print("The reciprocal of", entry, "is", r)
```

- 1D and 2D arrays
  - days = ('monday','tuesday')
  - students = ['yani','ibi','abd','qasim']
  - results = {'stu':['yani','ibi','abd','qasim'],'physics':[50,20,4,2314],'chemistry':[32,45,54,5]}
  - key,value
- string manipulation

## algorithms

- Binary

```python
def binarySearch(array, x, low, high):

    # Repeat until the pointers low and high meet each other
    while low <= high:

        mid = low + (high - low)//2

        if array[mid] == x:
            return mid

        elif array[mid] < x:
            low = mid + 1

        else:
            high = mid - 1

    return -1
array = [3, 4, 5, 6, 7, 8, 9]
x = 4

result = binarySearch(array, x, 0, len(array)-1)

if result != -1:
    print("Element is present at index " + str(result))
else:
    print("Not found")
```

- linear search
- Sorting algorithm
- Bubble and insertion sort

## OOP

- Defining classes and instantiating objects
  - declaring attributes and defining methods
  - inheritance (skip)
  - polymorphism (skip)
  - containment
- File handling:
  - Opening and closing files
  - reading writing or appending to a file
  - searching files
  - checking if a file exists
