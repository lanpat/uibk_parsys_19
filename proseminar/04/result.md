# Assignment 4, due November 6th 2019

The goal of this assignment is to extend the 3D heat stencil application of Assignment 3 to include multiple domain decomposition schemes and investigate the effect of non-blocking communication.

Group members: Raphael Gruber, Patrick Lanzinger

## Exercise 1

### Tasks

#### Provide implementations for the 3D heat stencil application that rely on the three domain decomposition variants presented in the lecture.

see ``heat_stencil_3D_cubes.c``, ``heat_stencil_3D_slaps.c`` and ``heat_stencil_3D_poles.c``
Unfortunatly the poles version is not working correctly.s

#### Measure their speedup and efficiency for multiple problem and machine sizes as in the previous exercise.
#### Illustrate the data in appropriate figures and discuss them. What can you observe?

![Image][slaps.png) 
