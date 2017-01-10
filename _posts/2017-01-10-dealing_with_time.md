---
layout: post
title:  "Dealing with time(not like Dr. Who)!"
date:   2017-01-10 00:00:00 +0000
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
hour = 60
def convert_mins_to_hours(mins):
    remaining_mins = mins % hour
    full_hours = (mins-remaining_mins)/60
    return full_hours

total_mins = int(input("please enter an amount of minutes: "))
total_hours = convert_mins_to_hours(total_mins) #this gets us the hours
remainder_mins = total_mins - (total_hours*hour)#this gets us the remaining mins

print("{0} hours and {1} minute(s)".format(int(total_hours),int(remainder_mins)))

```
Pw

[1]:https://www.python.org/
[2]:https://atom.io/
[3]:https://www.codecademy.com/
[4]:https://leigh-hackspace.github.io/codeclub/codeup/codeclub/leigh/hackspace/2016/12/15/getting-started-with-python.html
[5]:https://github.com/leigh-hackspace/codeclub
[6]:https://leigh-hackspace.github.io/codeclub/codeup/codeclub/leigh/hackspace/2016/10/17/gitting-started.html
