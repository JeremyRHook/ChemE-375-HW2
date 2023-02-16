# ChemE-375-HW2
# ChemE 375 HW2

## Problem 1 (5 points)

Solve the following systems of linear algebraic equations using Matrix calculations

*Hint*: Remember to click and hold down ctlr+shift+enter when applying matrix math formulas:

<img src="https://latex.codecogs.com/gif.latex?11x_1&space;&plus;&space;3x_2&space;&plus;&space;x_4&space;&plus;&space;2x_5&space;=&space;45" title="11x_1 + 3x_2 + x_4 + 2x_5 = 45" />
<img src="https://latex.codecogs.com/gif.latex?4x_2&space;&plus;&space;2x_3&space;&plus;&space;x_5&space;=&space;30" title="4x_2 + 2x_3 + x_5 = 30" />
<img src="https://latex.codecogs.com/gif.latex?3x_1&space;&plus;&space;2x_2&space;&plus;&space;7x_3&space;&plus;&space;x_4&space;=&space;15" title="3x_1 + 2x_2 + 7x_3 + x_4 = 15" />
<img src="https://latex.codecogs.com/gif.latex?4x_1&space;&plus;&space;4x_3&space;&plus;&space;10x_4&space;&plus;&space;x_5&space;=&space;20" title="4x_1 + 4x_3 + 10x_4 + x_5 = 20" />
<img src="https://latex.codecogs.com/gif.latex?2x_1&space;&plus;&space;5x_2&space;&plus;&space;x_3&space;&plus;&space;3x_4&space;&plus;&space;14x_5&space;=&space;92" title="2x_1 + 5x_2 + x_3 + 3x_4 + 14x_5 = 92" />

## Problem 2 (5 points)

Determine **one** solution for x and y to the following equations (there are 4 possible solutions).  *(You may want to graph the equations to see where the equations intersect and find a good guess value for solver. If you do make a plot, note that for the first equation you can only solve for y for x values between -0.7 and 0.7.  For the second equation you can only solve for y with x values between -1 and 3.  Also remember that when solving y2=x for y, the solution is y = ±√𝑥.)*

<img src="https://latex.codecogs.com/gif.latex?2x^2&space;&plus;&space;y^2&space;=&space;1" title="2x^2 + y^2 = 1" />
<img src="https://latex.codecogs.com/gif.latex?(0.5x&space;-&space;0.5)^2&space;&plus;&space;2(y-0.25)^2=1" title="(0.5x - 0.5)^2 + 2(y-0.25)^2=1" />


## Problem 3 (5 points)

The Redlich/Kwong equation of state is

<img src="https://latex.codecogs.com/gif.latex?P&space;=&space;\frac{RT}{V-b}&space;-&space;\frac{a}{\sqrt{T}V(V&plus;b)}" title="P = \frac{RT}{V-b} - \frac{a}{\sqrt{T}V(V+b)}" />

where T is the temperature, V is the molar volume, R is the universal gas constant, and a and b are compound-specific constants.  Find the molar volume of ethane for each phase that is present at T = 77 °C and P = 1 bar.  For ethane, a = 2.877×108 cm6 bar K0.5 mol-2 and b = 60.211 cm3 mol-1.

*Hints*:

* Use the ideal gas law to obtain the guess of the vapor volume and 1.1*b to obtain the guess for the liquid volume.  (Graphing helps find good guesses for solver).
* You may need to include some constraints.
* IF YOU ARE STUCK ask a friend, the TA OR the instructor!  Don’t spent so much time feeling lost that you become discouraged.
* You should obtain something around 28637 cm3/mol for the vapor volume and 82.477 cm3/mol for the liquid volume. The middle root (not required but for you information) is in between.

## Problem 4 (5 points)

Imagine mixing liquid benzene (species 1) and toluene (species 2) together in an initially empty container. At equilibrium, some of the liquid from both species will evaporate into the vapor phase and some will be left liquid phase for certain temperatures and pressures. For the specific example mentioned above, Raoult’s law gives the following two expressions describing the equilibrium state:

<img src="https://latex.codecogs.com/gif.latex?y_1P&space;=&space;x_1&space;P_1^{sat}(T)" title="y_1P = x_1 P_1^{sat}(T)" />
<img src="https://latex.codecogs.com/gif.latex?y_2P&space;=&space;x_2&space;P_2^{sat}(T)" title="y_2P = x_2 P_2^{sat}(T)" />

where yi is the mole fraction of species i (either 1 or 2) in the vapor phase, xi is the mole fraction of species i in the liquid phase, Pisat(T) is the vapor pressure of species i at the system temperature T, and P is the system pressure.

The vapor pressures of benzene and toluene can be found using the Antoine Equation.

<img src="https://latex.codecogs.com/gif.latex?\ln{\frac{P_i^{sat}(T)}{kPa}}&space;=&space;A_i&space;-&space;\frac{B_i}{T/^\circ&space;C&space;&plus;&space;C_i}" title="\ln{\frac{P_i^{sat}(T)}{kPa}} = A_i - \frac{B_i}{T/^\circ C + C_i}" />

Note that you cannot take the natural log of a number with units.  Therefore, Pisat is divided by kPa or we take the log of Pisat as it would be if it had units of kPa.  Note that Pisat(T) is not Pisat times T, but is simply showing that Pisat is a function of T.  Also note that T/oC means that a dimensionless form of temperature is inputted as the temperature would be if it had units of oC.  Do not confuse oC (degrees Celsius) with Ci which is the constant given in the table below.  The constants A, B, and C are compound specific and are found in the table below.

| Compound | A       | B       | C       |
| -------- | ------- | ------- | ------- |
| Benzene  | 13.7819 | 2726.81 | 217.572 |
| Toluene  | 13.9320 | 3056.96 | 217.625 |

If a mixture of benzene (species 1) and toluene (species 2) has y1 = 0.33 and P = 120 kPa, find x1 and T. Remember that the mole fractions of each phase must sum to 1. (Hint:  Follow the steps outlined in the handout from class.   

*Hints*:

* First figure out what you are solving for.  Then figure out how many equations you have.
* You might want to set up a cell for Psat1 and Psat2 that reference your cell containing T.
* SEE THE TA OR THE INSTRUCTOR IF YOU ARE STUCK!  Don’t spent so much time feeling lost that you become discouraged.
* There are many right ways to do this.
* You should get about 0.17 for x1 and 109 °C for T.
