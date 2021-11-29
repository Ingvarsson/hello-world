# hello-world
Just another repository

Пока что побудет здесь:

def to_number(s):
    my_string = [c.upper() for c in s]

    my_dict = {'1':	'.,?!:',
           '2': 'ABC',
           '3': 'DEF',
           '4': 'GHI',
           '5': 'JKL',
           '6': 'MNO',
           '7': 'PQRS',
           '8': 'TUV',
           '9': 'WXYZ',
           '0': ' '}
           
    for c in my_string:
        for values in my_dict:
            if c in my_dict[values]:
                print(values * (my_dict[values].index(c) + 1), end='')
            

print("Please input your request in English")
s = input()
print('Result:')
to_number(s)




И это тоже пока побудет здесь:
import turtle
import random

def snowflake():
  turtle.pendown()
  size = random.randrange(20, 70)
  color = (random.randrange(0, 255), random.randrange(0, 255), random.randrange(0, 255))
  turtle.pencolor(color)
  for _ in range(8):
    turtle.forward(size)
    for _ in range(3):
      turtle.backward(size / 4)
      turtle.right(45)
      turtle.forward(size / 4)
      turtle.backward(size / 4)
      turtle.left(90)
      turtle.forward(size / 4)
      turtle.backward(size / 4)
      turtle.right(45)
    turtle.backward(size / 4)
    turtle.left(45)
  turtle.dot()
  turtle.penup()

turtle.Screen().bgcolor("lightblue")
turtle.pensize(2)
 
turtle.goto(0, 0)
snowflake()
turtle.goto(100, 100)
snowflake()
turtle.goto(-100, 100)
snowflake()
turtle.goto(-100, -100)
snowflake()
turtle.goto(100, -100)
snowflake()
turtle.hideturtle()
