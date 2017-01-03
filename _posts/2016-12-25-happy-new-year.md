---
layout: post
title:  "Happy new year!"
date:   2016-12-25 00:00:00 +0000
categories: CodeUp CodeClub Leigh Hackspace
---

Making Python Calculator
================

Happy new year! - we're going to dive right in with writing out own calculator

Below is an example Calculator

I've saved the file name as calc.py
(as mentioned in the [previous post][4] we'll be using the [Atom][2])
 you'll need to clone the [code club repo][5] if you don't know how to clone a repo there was [a previous post][6] covering this if you need to get started...back to Python:


```python
class Calculator:

    def Add (x, y):
        return x + y

    def Subtract (x, y):
        return x - y

    def Multiply (x, y):
        return x * y

    def Divide (x, y):
        return x / y

    def Modulo (x):
        return x % y

    def Factorial(x):
      retval = x
      x = x-1
      while x > 0:
        retval = retval * x
        x = x-1
      return retval

    menu_options = {
     1: Add,
     2: Subtract,
     3: Multiply,
     4: Divide,
     5: Modulo,
     6: Factorial,
    }

    def Menu(self):
        print('1) Add \n2) Subract\n3) Multiply \n4) Divide\n5) Modulo\n6) Factorial')
        choice = input("Select option:")
        x = float(input("enter first number:"))
        if choice != 6:
          y = float(input("enter second number:"))
          func = self.menu_options.get(choice)
          return func(x, y)
        else:
          func = self.menu_options.get(choice)
          return func(x)

while True:
    calc = Calculator()
    print(calc.Menu())

```
So the next thing we're going to do is introduce a Modulo function

```python

  result = 88 % 60

```

  one thing you may notice about the code above is that there is no error trapping which is a problem if you enter anything but numbers in the number prompt... adding error trapping will be out _second_ task

hopefully this will be enough to tide you over ... if not try adding _factorial_ ;-)

```python
   def Factorial(p):
     retval = p
     p = p-1
     while p > 0:
       retval = retval * p
       p = p-1
     return retval

```
Pw

[1]:https://www.python.org/
[2]:https://atom.io/
[3]:https://www.codecademy.com/
[4]:https://leigh-hackspace.github.io/codeclub/codeup/codeclub/leigh/hackspace/2016/12/15/getting-started-with-python.html
[5]:https://github.com/leigh-hackspace/codeclub
[6]:https://leigh-hackspace.github.io/codeclub/codeup/codeclub/leigh/hackspace/2016/10/17/gitting-started.html
