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
