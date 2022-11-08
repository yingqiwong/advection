# advection

MATLAB function and demo scripts to calculate the advection of a quantity 
with a velocity field. This is applicable to models using a 2D staggered 
grid discretisation, where the quantity is defined at the cell center, and 
velocities are defined at cell faces. All schemes use a flux-conservative 
approach, such that the advected quantity is approximated at the 
respective cell face using these schemes, and is then combined with the 
velocity already defined there in a staggered grid.

Seven advection schemes are programmed here:
+ central difference, 2nd order (baseline)
+ upwind, 1st order (baseline)
+ QUICK, equivalent to 3rd order upwind (Leonard, 1995)
+ Fromm (Trompert \& Hansen 1996)
+ Total Variation Diminishing (TVD) scheme (Harten 1983)
+ 3rd order Weighted Essentially Non-Oscillatory (WENO) scheme (Jiang \& Shu 1996)
+ 5th order Weighted Essentially Non-Oscillatory (WENO) scheme (Jiang \& Shu 1996)

