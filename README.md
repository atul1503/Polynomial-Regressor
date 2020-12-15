# Polynomial-Regressor
------------------------
v1.5 is more reliable than the others.



Purpose:
----------
This is a custom function regressor or curve fitter algorithm using least squares optimisation technique.


Prerequisites:
---------------
Python.
A csv file ending with an 'eof' character.



Usage:
-------
type your function inside the custom() function block where w[0] is the first parameter,w[1] is the second parameter etc.
set the weights variable to the no. of parameters your function contains.
execute the script in your python installed computer.
provide the csv data file's name or location.
Output will be the paramter array which contains the best fit paramter values for the given data.


Examples for using a custom function inside the script:
--------------------------------------------------------
for a linear function having 2 parameters:-

def custom(x,w):
//for now dont care what x and w are.

  return w[0]*x+w[1]        //in other words, return ax+b where a is w[0],b is w[1]

For a sine() function having 4 paramters:-

def custom(x,w):
  return x[0]*sin(w[1]*x+w[2])+w[3]
  

Finally before the custom() function there is a weights variable.
For 1st example set:-

weights=2

For 2nd example:-

weights=4

