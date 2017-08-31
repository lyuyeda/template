---
layout: project
type: project
image: images/hexsudoku_preview.png
title: Recursive Sudoku
permalink: projects/recsudoku
date: 2017
labels:
  - Java
  - Sudoku
  - Recursion
summary: A simple program for recursively solving a hexadecimal sudoku puzzle
---

<img class="ui large right spaced image" src="../images/recsudoku.png">

Recursive Sudoku was a project from ICS 211 with the goal of creating a recursive program to solve a hexadecimal sudoku puzzle.

Recursive Sudoku was a solo project, however, much of the test code was provided, as attributed in the top most comments of the java files, by Biagioni, Edoardo, and Cam Moore.

In the end, Recursive Sudoku wound up being a lesson in the danger of overengineering.  Coding it to use more conventional sudoku rules for as long as possible took significant amounts of time to write while creating a rather insignificant difference in performance.  Indeed, the program's reliance on this new structure, which attempted to keep track of remaining available options slowed the program down greatly due to the recursive nature of the project.  While the checks were mostly harmless when applied once, attempting to apply them at every level of recursion bogged it down.  In the end, my solution would take an hour to solve the test problems provided while simple, purely brute-force solutions managed the same in mere minutes.

Source: <a href="https://github.com/lyuyeda/HexSudoku"><i class="large github icon"></i>HexSudoku</a>
