PYTHON GUI CALCULATOR:
A simple, user-friendly graphical calculator built entirely in Python using the tkinter library. This project provides a functional on-screen calculator that handles everyday arithmetic with a clean, high-contrast dark theme.

FEATURES:
1.Basic Arithmetic: Supports standard operations like addition (+), subtraction (—), multiplication (x), and division (/).
2.Modern Dark Interface: Designed with a sleek black background, white text for numbers, and vibrant orange accents for the operator buttons.
3.Smart Error Handling: If you try to calculate an invalid equation (like dividing by zero or entering incomplete operators), the screen safely clears and displays ERROR.

CORRECTION TOOLS:
1.AC (All Clear): Instantly wipes the current calculation to start fresh.
2.⌫ (Backspace): Deletes the last character you entered if you make a typo.
3.Percentage & Decimals: Fully supports decimal numbers and percentage operations.
PREREQUISITES:
To run this project, you only need one thing:
Python 3.x: Make sure Python is installed on your computer.
(Note: tkinter is Python's standard GUI library and comes pre-installed with Python. You do not need to install any external libraries using pip!)

How to Run the Calculator:
1.Download or copy the code into a file named calculator.py.
2.Open your computer's terminal or command prompt.
3.Navigate to the folder where you saved your calculator.py file.

Run the following command:
command:"python calculator.py"
A window will pop up, and you can start calculating!

Behind the Code (How It Works):
1.This script uses tkinter to create a main application window (Tk()). The buttons are organized using a simple grid system (rows and columns) to keep everything aligned perfectly.
2.When you click the buttons, the program continuously updates a hidden text string (the expression). Once you click the equals (=) sign, Python's built-in eval() function reads that string, calculates the math, and instantly displays the result in the top entry box.
