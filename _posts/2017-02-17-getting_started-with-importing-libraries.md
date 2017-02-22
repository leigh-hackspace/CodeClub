---
layout: post
title:  "Turtle Power (or introduction to importing libraries)"
date:   2017-02-17 00:15:00 +0000
categories: CodeUp CodeClub Leigh Hackspace Python
---

Turtle Power
================
So first off ... we need to go to our code club repo and create a `turle` folder and in this folder create a file with your initials in it with the extension of `.py` for example `week9PW.py`

If, like me you're running linux you can do this in the command line by typing the following into a command shell
`$ touch week9PW.py `
but then you wouldn't be following along in atom ;-) so in atom if you need to right click the `2017` folder and select the `new folder` option then name it something like `turtle<yourinitials>` then right click this folder and then select new file this is our file so it will need a `.py` extension (like I mentioned above)
![creating the turtle file]({{ site.url }}/codeclub/images/turtle_power/1.adding_turtle_file.png)

so first thing we need to do is import the [Turtle][4] library

```python
import turtle as t

while 1:
  print("press any key to step")
  input()
  t.fd(100)
  t.right(90)  
```

save this file ... and then run it
`python <whatever you called the file>.py `

you will get a prompt asking you to press any key - when you do it will draw a line it will look something like this after you press any key a couple of times
![creating the turtle file]({{ site.url }}/codeclub/images/turtle_power/2.drawing_a_line.png)

if you check out the [Turtle Docs][4] there's lots of different things to experiment with ... let's see about changing the colour of the line we draw

```python
import turtle as t

while 1:
  print("press any key to step")
  input()
  t.pencolor("red") #added a colour
  t.fd(100)
  t.right(90)  
```

have fun see what else you can come up with

Pw

[1]:https://www.gitkraken.com/
[2]:https://desktop.github.com/
[3]:https://github.com/leigh-hackspace/codeclub
[4]:https://docs.python.org/3.0/library/turtle.html
