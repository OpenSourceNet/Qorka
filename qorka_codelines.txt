#!/usr/bin/env python
# -*- coding: utf8 -*- 
# This is my canvas. This is my art.
"""
// Information //
Name : Qorka
Description : This is Qorka. A python interface for developers to easily create
				and execute simple interpreters that allow simulation of simple
				programs.
Version : 1.0
Supporting OS : Mac OSX
Created by : Nirman Dave
Licensed to : SourceNet.in
Website : qorka.sourcenet.in
Built on : Python 2.7.6 (Pre-Requisite for Qorka)

// Copyright notice, terms & conditions//
(c) Copyrights 2015 by Nirman Dave. All rights reserved.
This work may be modified, reproduced, distributed, performed, and displayed for any purpose but 
must acknowledge "Nirman Dave", "SourceNet" and "Qorka". Copyright is retained and must be 
preserved. The work is provided as is; no warranty is provided, and users accept all the liability.
"""

# The program begins hereon.
# The program has been divided into two distint arenas.
# First arena is named - The imports arena : Here you can import all the important APIs you might need.
# Second arena is named - The functions' arena : Here you can define all the functions you need later.
# Third arena is named - The codelines arena : Here you mention the conditions, parameters and codes of execution.
#						 This is the arena where the major part of development will take place.

# ----- First arena -------
"""
This is the imports arena.
This is where you can import different liberaries and use different APIs specific to python language.
The default imports consist of date and time. All imports happen in a list.
The following are some dummy lists, they are for understanding of the layout.
"""

# Import list 1 - Date and time
import datetime
import time

# Import list 2 - Systems and administrations
import os
import string
import random

# Import list 3 - UI
from Tkinter import *
from PIL import ImageTk, Image
import os

# ----- Second arena -------
"""
The functions' arena.
This is the place where all the functions are defined. The functions are defined in the 'Function Block'.
The default functions given are 'add', 'multi', 'div' and 'sub'.
You can add your own functions as and when needed.
"""

# Funtion Block 1 - Number addition

# Defining 'add' with the variable 'x'
def add(x):
	# Removing the letters 'add' from the code_line and assigning it to the string variable 'equation'.
	equation = x[4:]
	# Searching for the location of '+' sign.
	sign_location = equation.index('+')
	# Dividing the code_line in two parts. 
	# First part before the sign. Second part after the sign.
	cut = int(sign_location)
    # Defining the two parts with string variable 'first_integer'.
   	first_integer = equation[:cut]
    # Defining the two parts with string variable 'first_integer'.
   	second_integer = equation[(cut+1):]
    # Returning the addition of the two values.
   	print (int(first_integer) + int(second_integer))
# The similar logic goes for the rest of the math-function blocks.
# These other blocks have been defined by default.

# Function Block 2 - Number subtraction

def sub(x):
    equation = x[4:]
    sign_location = equation.index('-')
    cut = int(sign_location)
    first_integer = equation[:cut]
    second_integer = equation[(cut+1):]
    print (int(first_integer) - int(second_integer))

# Function Block 3 - Number multiplication

def multi(x):
    equation = x[4:]
    sign_location = equation.index('x')
    cut = int(sign_location)
    first_integer = equation[:cut]
    second_integer = equation[(cut+1):]
    print (int(first_integer) * int(second_integer))

# Function Block 4 - Number division

def div(x):
    equation = x[4:]
    sign_location = equation.index('/')
    cut = int(sign_location)
    first_integer = equation[:cut]
    second_integer = equation[(cut+1):]
    print (int(first_integer) / int(second_integer))


# ----- Third arena -------
"""
This is the codelines arena.
This is where the executive code starts. The executions and aligning of functions through codelines happens here.
"""
# ================================
# =========== UI Code ============
# ================================

# This is the User Interface code which is tailored for the Qorka window.
# You will not be working with this area of code often.

# Defining the main root (Qorka window) using Tkinter, Python.
# In the following block, the window's specifications have been addressed.
root = Tk()
root.title("Qorka")
root.geometry("500x300")
root.resizable(0,0)

# The Qorka window comprises of a background image which is displayed in the panel created below.
img = ImageTk.PhotoImage(Image.open("qorkadisplay.jpg"))
panel = Label(root, image = img)
panel.pack(side = "bottom", fill = "none", expand = "no")

# The Qorka window menu buttons and their functions have been defined below.
qorkaMenu = Menu(root)
root.config(menu = qorkaMenu)
qorkaSubMenu = Menu(qorkaMenu)
qorkaMenu.add_cascade(label = "File", menu = qorkaSubMenu)
qorkaSubMenu.add_command(label = "New Project")

qorkaSubMenu2 = Menu(qorkaMenu)
qorkaMenu.add_cascade(label = "Try", menu = qorkaSubMenu2)

# Looping the main root (Qorka window) so that it stays on the screen until closed.
root.mainloop()

# ================================
# ======== Execution Code ========
# ================================

# This is the Execution code which is tailored for the functioning of the basic Qorka interpreter.
# This is an area you will be playing with.

# Defining the Qorka Code File (QCF). The 'QCF_location' is the location of the text file which encompasses the Qorka's code file.
# 'OCF_open' opens up the Qorka code file for Mac.

QCF_location = raw_input ("Code Address : ")
QCF_open = open(r"/"+str(QCF_location))

# Executing all the blocks repeatedly through the wile loop.
# Each line is read using the 'code_line = str(QCF_open.readline())[:-1]' fucntion.
# Then each line undergoes a piece of 'Block'. Every 'Block' contains a fucntion.
# If the conditions and parameters of the functions align, the 'Block' is excuted.

while 1:
    code_line = str(QCF_open.readline())[:-1]

    # Block 1 - The default 'Print' fucntion.
    if "gab" in code_line:
        print code_line[4:]

    # Block 2 - The default 'Add' function.
    elif "add" in code_line:
    	# Instead of rewriting the whole function, now we just call the function we previously defined.
        add(code_line)

    # Block 3 - The default 'Sub' function.
    elif "sub" in code_line:
    	sub(code_line)

   	# Block 4 - The default 'Mul' function.
    elif "mul" in code_line:
    	multi(code_line)

    # Block 5 - The default 'Div' function.
    elif "div" in code_line:
    	div(code_line)

    # Block 6 - The default 'Comment' function.
    #			This allows you to comment in the code lines you write.
    elif "!!#" in code_line:
    	pass

    # Block 7 - The default function to end the code and the program.
    elif code_line == "//end":
    	break
    
    # Block 8 - The default 'Ping' functions for getting information.
    # Looks for the word 'Ping'.
    elif code_line[0:4] == "ping":
    	# If the word 'Ping' exists in the code_line, then looks for the word 'date' and/or 'time'.
    	if "date" in code_line:
    		# If the word 'date' is present, outputs the current date.
    		print datetime.datetime.now().strftime("%d-%m-%Y")
        elif "time" in code_line:
        	# If the word 'time' is present, outputs the current time.
        	print datetime.datetime.now().strftime("%H:%M")

# The Qorka framework ends here. 
# You can start adding your code blocks from hereon.


