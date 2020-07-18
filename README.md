# Repeated_interactions_solver
Python libary for studying open quantum systems using the model of repeated interactions. 

1) Run the makefile to generate the file libtime_evolution.so (gcc is required).
2) Copy all the files into the project folder.
3) import repeatedinteractions_c

  The library consists of two classes, one for heat reservoirs and the other for the systems. The heat reservoir has methods for calculating
the thermal state and the thermal state at negative temperature of the reservoir systems. The system class has the system's state, hamiltonian,
energy, heat and work as atributes, and a method for solving the dynamics of several scenarios (open or closed dynamcis, constant or time dependent
hamiltonians). 
  The dynamics is calculated with a Runge Kutta 4th order method. All of the time evolution functions are written in C in order to optimize speed.
 This functions are included in the libtime_evolution.so file, they are wrapped into a python library in the file time_evolution.py, which is included in the repeatedinteractions_c.py file.
 In order to use the library, one only has to import the repeatedinteractions_c.py file. 
  
