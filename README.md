# UniformColoring
AI Project to develop a classifier model that takes a grid problem written by hand and to execute a search algorithm such as UCS and A* and compares the different heuristic functions 

Google Colab Notebook: https://colab.research.google.com/drive/1zSfgYlWx896W3d-Y7IcQ7J1ZAMthWl_C?usp=sharing


Uniform Coloring is a game where you have a few cells to color, and various colors
available. 
For simplicity, let's imagine a rectangular grid in which you can move one dye head between adjacent cells according to the 4 cardinal directions (N, S, E, W), without leaving the grid.
All cells have a starting color (B = blue, Y = yellow, G = green) except for the one in which the head indicated with T is located (starting point). 
The head can color the cell in which it is located with one of the colors available at different costs (cost (B) = 1, cost (Y) = 2, cost (G) = 3),
while displacements all have a uniform cost equal to 1. 
The goal is to color all the cells of the same color (no matter what) and return the head to its starting position.
The coding of the whole domain (topology of the grid, definition of actions etc.) is done extending the Problem class of aima-python. 
Starting from the initial position of the head and combining move actions and coloring, the aim is to find the agent's sequence of actions to achieve the goal state.

The initial position of the head, the structure of the grid and the initial coloring of the cells are given to the system via an image (that can also be drawn by hand).
