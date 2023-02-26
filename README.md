# PHSX815_Week6
contain code pertaining to week 6 homework


First off, this homework contains code and uses information from the following:
https://stackoverflow.com/questions/27115917/gauss-legendre-quadrature-in-python
https://en.wikipedia.org/wiki/Gaussian_quadrature
http://specminor.org/2017/01/05/numerical-integration-python.html
https://keisan.casio.com/exec/system/1329114617   The evaulation points and weights comes from here

Also contains my own previously used code and some of my own tweaks to construct the Gauss-Legendre Method

To run the HW6 code:
1. You will need to put the Int.py into a folder and specify its location in IntCompare.py code, so it is imported correctly. The Int.py contains my Integration class which has all of my integration methods.
2. Run the IntCompare.py code. I used python3 IntCompare.py to run. It should then output the area values for two different numerical integration methods, as well as, their respective errors. It should also output the exact value of the integral last.
3. Some specifics. If you want to change the bounds of integration you will need to go into the code and change a and b. Likewise, you can change the function here as well. The number of rectangles is changed by changing n.
4. To change the gauss quadrature to a new method, or add more subintervals, you will need to go to https://keisan.casio.com/exec/system/1329114617 to gets the weights and eval points you need, then these will need to be inputted into X[i] and W[i] in the Int.py code.


HW 7:
Homework 7 runs exactly the same way as homework 6. The only major difference is I've added the Monte Carlo Integration to my Integration class which averages my function f over N points. N can be changed from the MCcompare.py code
1. You will need to put the Int.py code into a folder and specify its location in MCcompare.py code, so it is imported correctly. The Int.py contains my Integration class which has all of my integration methods.
2. Run python3 MCcompare.py
3. The code should output the numerical integrals of 3 different methods, including Monte Carlo, and their respective errors. Lastly it should output the exact value of the integral, using scipy's built in integration method.
