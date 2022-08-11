### Say "Hello, World!" With Python

**Task**
Here is a sample line of code that can be executed in Python:

    print("Hello, World!")

You can just as easily store a string as a variable and then print it to stdout:

    my_string = "Hello, World!"
    print(my_string)

The above code will print Hello, World! on your screen. Try it yourself in the editor below!

### Python If-Else

**Task**
Given an integer, _n_, perform the following conditional actions:

- If  is odd, print Weird
- If  is even and in the inclusive range of  to , print Not Weird
- If  is even and in the inclusive range of  to , print Weird
- If  is even and greater than , print Not Weird.

      import math
      import os
      import random
      import re
      import sys

      if __name__ == '__main__':
          n = int(raw_input().strip())
      if n % 2 != 0 :
          print("Weird")
      if n % 2 == 0 :
          if 2 <= n  <= 5 :
              print("Not Weird")
          if 6<= n <= 20 :
              print("Weird")
          if n > 20 :
              print("Not Weird")
              
              
### Arithmetic Operators

**Task**
The provided code stub reads two integers from STDIN,  and . Add code to print three lines where:

- The first line contains the sum of the two numbers.
- The second line contains the difference of the two numbers (first - second).
- The third line contains the product of the two numbers.

      print(a + b)
      print(a - b)
      print(a * b)

### Python: Division

**Task**
The provided code stub reads two integers,  and , from STDIN.

Add logic to print two lines.
- The first line should contain the result of integer division, _a/b_,
- The second line should contain the result of float division, _a/b_.

No rounding or formatting is necessary.

    print(int(a/b))
    print(a/b)


### Loops

The provided code stub reads and integer, `n`, from STDIN. For all non-negative integers `i < n`, print `i^2`.

    for x in range(0, n, 1) :
        print(x**2)

### Write a Function

**Task**

Given a year, determine whether it is a leap year. If it is a leap year, return the Boolean True, otherwise return False.

Note that the code stub provided reads from STDIN and passes arguments to the is_leap function. It is only necessary to complete the is_leap function.

**Note**:
An extra day is added to the calendar almost every four years as February 29, and the day is called a leap day. It corrects the calendar for the fact that our planet
takes approximately 365.25 days to orbit the sun. A leap year contains a leap day.

In the Gregorian calendar, three conditions are used to identify leap years:
- The year can be evenly divided by 4, is a leap year, unless:
- The year can be evenly divided by 100, it is NOT a leap year, unless:
- The year is also evenly divisible by 400. Then it is a leap year.
- This means that in the Gregorian calendar, the years 2000 and 2400 are leap years, while 1800, 1900, 2100, 2200, 2300 and 2500 are NOT leap years. Source

      def is_leap(year):
          leap = False
    
          if year % 4 == 0 :
              if year % 100 == 0 :
                  if year % 400 == 0 :
                      leap = True
                  else:
                      leap = False
              else:
                  leap = True
          else:
              leap = False
    
          return leap

      year = int(raw_input())
      print is_leap(year)

### Print Function

The included code stub will read an integer, `n`, from STDIN.

Without using any string methods, try to print the following:

`1, 2, 3, ..., n`

Note that "..." represents the consecutive values in between.

    for x in range(1, n + 1, 1):
        print(x, end='')




