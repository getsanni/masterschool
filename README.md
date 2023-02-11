# parameters and arguements using turtle program

import turtle

#defining a function and setting its parameters
def spiral(sides, turn, color, width):
    t = turtle.Turtle()
    t.color(color)
    t.width(width)
    for n in range(sides):
        t.forward(n)
        t.right(turn)
#parameters arguements set
spiral(150, 20, "blue", 6)




#the same code with a little tweak

import turtle
jack = turtle.Turtle()
jack.color("yellow")
jack.speed(0)

def draw_square():
    for side in range(4):
        jack.forward(100)
        jack.right(90)

draw_square()

jack.penup()
jack.back(150)
jack.pendown()

draw_square()
jack.forward(100)
draw_square()
jack.forward(100)
draw_square()

for square in range(80):
    draw_square()
    jack.forward(5)
    jack.left(5)
